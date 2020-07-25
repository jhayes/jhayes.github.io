---
layout: page
title: Toolbox
permalink: /toolbox/
---

Collection of things I find useful.
<br><br>

# Unix commands #
* How To Find The Size Of A Directory In Linux
{% highlight ruby %}
du -sh
{% endhighlight %}

* Comparing the differences between two directories of files that are almost the same.
{% highlight ruby %}
diff -bur folder1/ folder2/
{% endhighlight %}

* Finding a particular file in a folder in linux. This will look in the current folder (and sub-directories) for that string in a name of a file.
{% highlight ruby %}
find . -name '*default_setup.use'
{% endhighlight %}

* How To Find Out My Linux Distribution Name and Version - nixCraft
{% highlight ruby %}
cat /etc/*-release
{% endhighlight %}

* Useful if you want to keep the folder hierarchy when you're copying.
(For instance, if you have two files called 'temp_calib0.inc' and they're in different folders. If you copy them over to one location, you need to either rename or put them in different folders).

The following command might do:

{% highlight ruby %}
xargs -a copy_files.txt cp --parents -t /net/10.xx.xx.xx/XXX/XXX/XXX/copied_files/
{% endhighlight %}

1. Note that this uses a txt file to feed in the files you want to copy.
2. Note the direct path used for the location to copy to (use npwd to get this, handy for passing between different locations, Bangalore/Limerick/etc).

* Handy for watching the output of certain commands.
{% highlight ruby %}
watch bhappy
{% endhighlight %}

# Emacs

### [Deleting the first 'x' characters from every line in a region with Emacs - Stack Overflow](https://stackoverflow.com/questions/15929872/deleting-the-first-x-characters-from-every-line-in-a-region-with-emacs) ##
You use your mark tool ('C-Spc') to highlight a box area and then use the command 'C-x r k' to remove this square/rectangle.

Don't worry about the mark tool highlighting the edges of lines in between, they won't be clipped.



#### Handy way to append a flag to the end of a line.

Command: M-< M-x replace-regexp RET $ RET a RET

This will place an 'a' at the end of all lines. The $ matches the end-of-line character.

Also one of the other answers shows how to use key-macros so could be handy later.



