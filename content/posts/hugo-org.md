+++
title = "Using Org-Mode with Hugo"
author = ["Jack"]
lastmod = 2024-06-18T21:30:38+01:00
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


## Adding Images {#adding-images}

This was the first stumbling block for me.

-   [Ox-Hugo Image Links](https://ox-hugo.scripter.co/doc/image-links/)
    -   Reading over this, put the images you're interested in, in the _static_ directory.
    -   Then you can reference them using the file: prefix and various square brackets.