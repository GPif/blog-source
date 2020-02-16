---
layout: post
title: "Quick preview of nohup command"
description: "Nohup is a command line to start a program from a terminal, and be able to quit the terminal without exiting your program"
thumb_image: "documentation/linux.jpg"
tags: [linux, command line]
---

# Nohup, to get out of the terminal

If you like to run script or program to your desktop from a terminal, but you want to be able to close your terminal without closing your program, you can use the ```nohup``` command.

{% highlight bash %}
nohup <command> &
{% endhighlight %}

The ```&``` is to run the process in bacground.

Only thing, it create a ```nouhp.out``` file to record the ```stderr```.

To avoid that, you can redirect it to ```stdout```.

{% highlight bash %}
nohup <command> >/dev/null 2>&1 &
{% endhighlight %}

Do not forget the 
```&``` in the end.


The process will still be a child process of your terminal. Just, it won't be killed with it (when the ```SIGUP``` signal is sent).
It is gloabally fine with most use, but if you need to make it is own process, you can combine your command with the ```disown```

{% highlight bash %}
nohup <command> >/dev/null 2>&1 & disown -h "$!"
{% endhighlight %}

I personnaly use it to run in one script every tool I need for a specific task (start db, run a couple of browser with specific profile, run my IDE etc ...)