{{ define "main" }}

<section id="main">
  <h1 id="title">{{ .Title }}</h1>
  <div>
    <article id="content">
      {{ .Content }}
    </article>
  </div>
</section>
<aside id="meta">
  <div>
  <section>
    <h4 id="date"> {{ .Date.Format "Mon Jan 2, 2006" }} </h4>
    <h5 id="wordcount"> {{ .WordCount }} Words </h5>
  </section>
    {{ with .GetTerms "topics" }}
      <ul id="topics">
        {{ range . }}
          <li><a href="{{ .RelPermalink }}">{{ .LinkTitle }}</a></li>
        {{ end }}
      </ul>
    {{ end }}
    {{ with .GetTerms "tags" }}
      <ul id="tags">
        {{ range . }}
          <li><a href="{{ .RelPermalink }}">{{ .LinkTitle }}</a></li>
        {{ end }}
      </ul>
    {{ end }}
  </div>
  <div>
    {{ with .PrevInSection }}
      <a class="previous" href="{{ .Permalink }}"> {{ .Title }}</a>
    {{ end }}
    {{ with .NextInSection }}
      <a class="next" href="{{ .Permalink }}"> {{ .Title }}</a>
    {{ end }}
  </div>
</aside>
{{ end }}
