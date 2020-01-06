---
layout: post
title: "Being a developer beyond simply coding"
description: "An overview of what it means to be a developer and why it is not simply production code"
thumb_image: "documentation/sample-image.jpg"
tags: [developer, philosophy]
---

What is like to be a developer in 2020. When we think about it, coding is more and more accessible, everyone can create their own website for their business or personal branding. Services delivers pre-made solution for basically every digital needs.

Today, it is quite easy to develop. You do not need a lot of knowledge to deliver a working product. And, as there is a lot of job in the domain, many reconvert as a developer.

So, what makes the difference between a wannabe coder and an experienced one.

# Develop, does'nt start by writing code

So, you have a project, and your first step is to open your favorite text editor to write the entry point of your program. And step by step add every feature needed to achieve your goal. Bad idea! This is how you typically create a tentacular unreadable and unmaintanble piece of software. The result will likely :

* be unreadable, only you will be able to navigate amongst the maze created, and even, if you will be lost if you have to go throw the code you have written six month ago.
* full of technical flows and lacking optimisation
* hard to debug
* impossible to test

## How to split

The first step when you want to tackle a project is to start by decomposing, whether you use an oriented object language, a functional language or whatever, the first step to design a software of any kind, is to determine the pieces that it compose. Generally, after this step you should notice the emeregence of some [design pattern](https://en.wikipedia.org/wiki/Software_design_pattern). Good news, you can now refere to a well documented legacy of software designer.

So far, you have not written a single line of code but your software have all its structure. Half the job is done

## Thinking ahead on how and where it will run

Knowing a bit more on what the code will look like, you can figure out your needs, what library will it depends on, does it lie on database, of what kind? A relation based one or a document one, how you will test. 

Once this questions answered, you can figure out the architectural schema needed. It can be quite simple, for instance, a simple webapp will only need an application server and a database, to more complicated, if you need a micro service applications with an asynchron message passing service.

## What you need?

It is time to setup your dev environment. Generally it is about taking your architecture schema an figure out how to run them locally. You can either run them all or use some mock to simulate there behavior. Also, how to setup a test environment and a continuous integration.

## Time to code!

Yes, about time, there you will see that it is just a translation of what you planned in previous steps.

# Develop, doesn't end once delivered

The deadline of a project, or the time it is delivered can been seen as the end of a journey, when we can now move to another one, with fresh new idea. It is not :) Your product is now used, visible, you my have some feedback, and if you want your baby to stay alive, you have to take care of it.

## You should have tested

I didn't put the emphasis on this before, but test is essential, and make sense once in production. Why? Because now you will use them to make sure the tiny modification you make will not crash the whole application. At this moment you will get the reward of the extra time you spend writing your tests. Thanks to them you avoid spending your weekend bringing back your service trying to limit the amount of money lost by a production failure.

## There will be bug and not only bugs

When you are young and confident developer, you think you are good enough to produce a flawless code elegantly design. It never append, worst, you rarely deliver a perfect code. Or if you do so, it means that you should have delivered earlier. 

Modern project management imply a lot of back and forth, with evolution, meaning you will break you perfect creation, the last unexpected feature can deeply break you fine tuned code landscape. 
Either it is the old [waterfall](https://en.wikipedia.org/wiki/Waterfall_model), the [V cycle](https://en.wikipedia.org/wiki/V-Model) or the controversial [agile](https://en.wikipedia.org/wiki/Agile_software_development)

With the years, there are several basic rules I learned :

* Do not make your code perfect, focus on covering MVP code of your project first
* Unitary tests! You will be rewarded, and thank you past self for that
* Do not anticipate features, they are unlikely to happen and you will produce code for nothing.
* Be [SOLID](https://en.wikipedia.org/wiki/SOLID) or if you are not in OO, split your code, and make sure that each part do only one thing. Thus it is easy to add or drop part of your code.
* Communicate with the user if you can. He can tell you if the complicate demand can be simpler if you slightly address it differently, and you can propose some behavior it would not think possible.

In a word, your code must be design to be flexible, able to be remodel, redesign. Able to welcome code to fix bug or new feature without loosing its maintainability.

## It can be a time bomb

Depends on what your career will be, what path you take, but one day you will have to go back to a piece of software you have done years ago. So if your code go ugly, not tested or unmaintained, it will blow on your own face. 

Because now you have to update libraries, connect to a new service, or whatever. As a developer, you want to grow knowing and testing new technologies, not stuck in your old project. Yet as the sole and only specialist of your code, you will be skipped from interesting project to take care of your burden. Trust me, you have better to make your code readable and easy to transmit for your own sake.

# It is not only about your code

You will not work alone, in a team in your job, on open source project among a community. If you want to last, you must fit to a common coding style, and accept the tiny default of other developer. You will not be able to focus or criticize the tiny line of code or you lost the very interest of working with a team. You must accept other and be constructive on your criticize so you are not the [talented jerk](https://jobs.netflix.com/culture) we put aside.
