+++
title = "Using Org-Mode with Hugo"
author = ["Jack"]
lastmod = 2024-06-27T21:15:00+01:00
tags = ["hugo", "emacs"]
draft = false
+++

## Starting Points {#starting-points}

Still learning how to use this.

I use emacs a fair bit and org-mode a bit so I'm interested in using an org-mode flow.
It's unclear yet if it's worth the effort for me but I'll give it a go anyways.

I'm currently working my way through a post by a guy called Andreyor.

A list of stuff in this area:

-   <https://andreyor.st/posts/2022-10-16-my-blogging-setup-with-emacs-and-org-mode/>
-   <https://diego.codes/post/blogging-with-org/>


## Adding a new post {#adding-a-new-post}

1.  Go to the home directory and add a new file 'post_XX.org'.
2.  Add a preamble of #commands that can be copied from an old post.
3.  Write your post.
4.  Use of the command C-c, C-e, H, H.
    -   This invokes ox-hugo that will generate the markdown file.
5.  Go to a terminal and invoke 'hugo server -D' from the home directory.
6.  Marvel at the results at 'https://localhost:1313'.


## Adding Images {#adding-images}

This was the first stumbling block for me.

-   [Ox-Hugo Image Links](https://ox-hugo.scripter.co/doc/image-links/)
    -   Reading over this, put the images you're interested in, in the _static_ directory.
    -   Then you can reference them using the file: prefix and various square brackets.
