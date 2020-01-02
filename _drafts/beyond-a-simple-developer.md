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
So far, you have not written a single line of code but your software have all its structure. Half th job is done

## Thinking ahead on how and where it will run

Knowing a bit more on what the code will look like, you can figure out your needs, what library will it depends on, does it lie on database, of what kind? A relation based one or a document one, how you will test. 
Once this questions answere, you can figure out the architectural schema needed. It can be quite simple, for instance, a simple webap will only need an application server and a database, to more complicated, if you need a micro service applications with an asynchron message passing service.

## What you need?

It is time to setup your dev environement. Generally it is about taking your architeur schema an figure out how to run them locally. You can either run them all or use some mock to simulate there behavior. Also, how to setup a test environment and a continuous integration.

## Time to code!

Yes, about time, there you will see that it is just a translation of what you planned in previous steps.

# Develop, doesn't end once delivered

The deadline of a project, or the time it is delivered can been seen as the end of a journey, when we can now move to another one, with fresh new idea. It is not :) Your product is now used, visible, you my have some feedback, and if you want your baby to stay alive, you have to take care of it.

## You should have tested

I did't put the emphasis on this before, but test is essential, and make sense once in production. Why? Because now you will use them to make sure the tiny modification you make will not crash the whole application. At this moment you will get the reward of the extra time you spend writting your tests. Thanks to them you avoid spending your weekend bringing back your service trying to limit the amount of money lost by a production failure.

## There will be bug and not only bugs

## It can be a time bomb

# It is not only about your code
