+++
title = "Using Org-Mode with Hugo"
author = ["Jack"]
date = 2024-06-27T00:00:00+01:00
lastmod = 2024-06-28T10:04:34+01:00
tags = ["hugo", "emacs"]
draft = false
+++

## Summary {#summary}

This page is a summary of stuff I've learnt about using org-mode with Hugo to publish webpages.
It is still very much in flux.


## Starting Points {#starting-points}

I use emacs a fair bit and org-mode a bit so I'm interested in using an org-mode flow.
Because I use hugo to generate my website at the moment, use of a package called [ox-hugo](https://ox-hugo.scripter.co/) seemed the most convenient.


### Links {#links}

Some resources I've found so far are:

-   [Andrey Listopadov's setup](https://andreyor.st/posts/2022-10-16-my-blogging-setup-with-emacs-and-org-mode/)
    -   Got me up and running initially.
-   [Diego Vicente's setup](https://diego.codes/post/blogging-with-org/)
-   [Dr. Peter Prevos' setup](https://lucidmanager.org/productivity/create-websites-with-org-mode-and-hugo/)
    -   Handy details on front matter.
    -   Nice snippet on setting up a lastmod timestamp.
    -   Note that he doesn't use ox-hugo.


## Adding a new post {#adding-a-new-post}

1.  Go to the home directory and add a new file 'post_XX.org'.
2.  Add a preamble of #commands that can be copied from an old post.
3.  Write your post.
4.  Use of the command C-c, C-e, H, H.
    -   This invokes ox-hugo that will generate the markdown file.
5.  Go to a terminal and invoke 'hugo server -D' from the home directory.
6.  Marvel at the results located at 'https://localhost:1313'.


## Adding Images and PDFs. {#adding-images-and-pdfs-dot}

1.  Put the images you're interested in, in the _static_ directory.
2.  Then you can reference them using the file: prefix and various square brackets.


### Links {#links}

-   [Ox-Hugo Image Links](https://ox-hugo.scripter.co/doc/image-links/)


## Adding Tables {#adding-tables}

Firstly we can add a table by use of comma seperated values.

-   <https://orgmode.org/worg/org-tutorials/tables.html>


## Themes {#themes}

I'm currently using the [hello-friend-ng](https://github.com/rhazdon/hugo-theme-hello-friend-ng/) theme.


## Things to figure out {#things-to-figure-out}

1.  How do I add little hover notes?
2.  How do I change the theme properly?
