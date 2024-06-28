+++
title = "Emacs modifications"
author = ["Jack"]
date = 2024-06-28T00:00:00+01:00
lastmod = 2024-06-28T10:14:10+01:00
tags = ["emacs"]
draft = false
+++

## Summary {#summary}

This is a list of some niggles and how I deal with them as a reference.


## Deleting the first ‘x’ characters from every line in a region with Emacs. {#deleting-the-first-x-characters-from-every-line-in-a-region-with-emacs-dot}

You use your mark tool (‘C-Spc’) to highlight a box area and then use the command ‘C-x r k’ to remove this square/rectangle.

Don’t worry about the mark tool highlighting the edges of lines in between, they won’t be clipped.

[Link](https://stackoverflow.com/questions/15929872/deleting-the-first-x-characters-from-every-line-in-a-region-with-emacs)


## Handy way to append a flag to the end of a line. {#handy-way-to-append-a-flag-to-the-end-of-a-line-dot}

Command: M-&lt; M-x replace-regexp RET $ RET a RET

This will place an ‘a’ at the end of all lines. The $ matches the end-of-line character.

Also one of the other answers shows how to use key-macros so could be handy later.


## Reload configurations without restarting Emacs {#reload-configurations-without-restarting-emacs}

A quick way to reload your .emacs after making changes, to save a restart.

\`\`\` html
// M-x eval-buffer
\`\`\`

[Link](https://stackoverflow.com/questions/167705/reload-configurations-without-restarting-emacs)


## Finding location of .emacs file. {#finding-location-of-dot-emacs-file-dot}

C-h v 'user-init-file'

[Link](https://stackoverflow.com/questions/864892/how-do-i-find-which-emacs-file-has-been-loaded)
