---
layout: post
title: "Being a developer beyond simply coding"
description: "An overview of what it means to be a developer and why it is not simply production of code"
thumb_image: "documentation/sample-image.jpg"
tags: [developer, philosophy]
---


What is like to be a developer in 2020? The question is worst asking as I see many confusions, long time ago it was the geeky genius, living in the dark, socially disabled, to the cool start up west cost millenials, still facing its screen, still doing mystical things.

There the confusion convey by pop-culture, develop is producing code. Ask him/her something and it will furiously tip on its keyboard making its magic and creating the service that now worth millions, and in less than an hour.

Truth is, the magic is not that complicated, language and framework make it less and less complicated. Many become a developer, as it is not so mystical and thee is still this romantic representation.

The reality is quite different

# Coding is not 100% of your project

Many time we tend to rush writing code, thinking that our productivity is directly related to the number of line produced. This conception is harmfull and must be tackle. Start coding to fast is likely to give the following result :

* Unreadable code, only the creator will be able to navigate amongst the maze created, and even, you will be lost if you have to go throw the code you have written six month ago.
* Lots of technical flows and lacking optimisation
* Hard to debug
* Impossible to test

First thing to do is to plan and think ahead what to do, the first tool is not an IDE, but the one that help to plan, either is a pen and paper, a white board, a post-it or any project management software.

I like to answer the following questions sequentially :

1. What is the logical sequence to achieve the project ?
2. How to decompose this sequence in smallest pieces (Object/Module/Libraries) ?
3. How it will run in production? What architecture
4. How can I build a dev environment close to this architecture ?
5. How do I deploy and test, make sure it works when used

## 1. Think ahead how it will work

This first step is to outline the global behaviour of the product, what are the input, the output. It is to translate a common words of a need into technical solutions. The question is generally asked with the obvious statements like "I need to save this fields into a database", they are more likely to be "I need to setup a site to sell my products". The developer is the one to provide solutions to a problem.

## 2. Decompose

With experience, one of the instinct a developer grow is to detect code smells, meaning piece of code that should not be this way. A block with to much conditions, a methods doing to many things.

The key is to split into smallest methods, decompose the code into logical modules. Every methods should do only and only one thing as the [SOLID](https://en.wikipedia.org/wiki/SOLID) principles recommends.
If done well it should emerge some well known  [design pattern](https://en.wikipedia.org/wiki/Software_design_pattern).

## 3. What will it be in production

As part of the solution a developer must provide, explaining how it run is also part of the job. Some wold tell it is a sysadmin one, but in the end developing is also responsible to ask or build the architecture under. The [DevOps](https://en.wikipedia.org/wiki/DevOps) principle is mainly the formalization of what works in project, dev and operator that understand each other.

## 4. Building dev environment

Stick close to the production environment while developing is a good way to avoid bad surprise when going into production. 

Fortunately most framework, language provide every thing, therefore it is easy to have a close to production setup thanks to [docker](https://en.wikipedia.org/wiki/Docker_(software)).

## 5. Create and tests

Last part is to have a good test framework suited to our languages. I will not lie, tests runner are according to me still a work in progress, and quite painful to setup. And the first test is quite hard to make it works. But once done, it ensure that the code is and remain perfectly working, split into separated tasks.

There is many steps to build a sustainable system. To avoid any headache, [KISS](https://en.wikipedia.org/wiki/KISS_principle) , the system should not be complicated, and easy to maintain.

# The work is not finish after the last line

Other cliché, is the genius working all night long and with the first beam of the morning sun, look delighted to its screen of a finished work. Unfortunately, the limit is not that net. Result is that people are often reluctant to deliver, as the code is never perfect enough. And this for two reasons :

* Fear of being judge, there some part of the code a developer is ashame of and do not want to be seen by there peers.
* The fear to deliver something that is not working. As a homework we are reluctant to give as it will not give us good grades.

In fact, it took me time to realize that the delivery is not the end of the road, far from that. It is better to deliver fast, as soon as the [MVP](https://en.wikipedia.org/wiki/Minimum_viable_product) is working. Getting feedback as fast as possible allow a projet to stay align with the user need, especially if it tend to change with time.

Indeed, once the code is becoming concrete, the user will find bug, even if it is not bug according to its author, or ask for improvement. It is something a developer should embrace, as it is the very sign a product is used and appreciated.

That is why modern project management imply a lot of back and forth, either it is the old [waterfall](https://en.wikipedia.org/wiki/Waterfall_model), the [V cycle](https://en.wikipedia.org/wiki/V-Model) or the controversial [agile](https://en.wikipedia.org/wiki/Agile_software_development).

So that is why it is useless to wait for a code to be perfect before delivery. In fact a developer should focus to make it as modular and well designed as possible so that the entropy induce by the addition and evolution is as small as possible.
Sometime it even means rebuild the whole thing from scratch when realized that the need has evolved to much.

# Make something that works is easy, make something that last is hard 

Nowdays, let face it, it is kind of easy to learn to code, there is plenty of course on the internet, and, modern framework make it easy to attracts new developer. Indeed, what it used to be an obscure witchcraft is now quite accessible. The thing is, the expertise is now on making something good enough to be used on large scale and lasting long.

## Less code is better

One big pleasure of a developer, is actually to remove a big chunk of smelling code, by a simple set of one line functions, good enough to handle every limit conditions.
Simple code are easy to test, with a set of simple inputs expecting a simple outputs.

A big inpiration is [the beautifull code of doom 3](http://fabiensanglard.net/doom3/index.php), the code is simple and clean, even if there is a lot of model to handlei.


* Easier to maintain
* Elegant and robust
* Sign of a good design (sens of code smell)

* To be easy to maintain, only a glimps is needed to understand the code.
* Elegant and robust, it is plesant to read and leave a small place to errors
* Sign of a good design, a the library to do exactally what the code, without any wierd twist to the framework, meens that the developer and whoever is the creator of the lead, rich to the same conclusion, confirming that the design is a good one.

# You will and must not keep your code for yourself

The image of the sole developer to a program, guardian of the good behavior of the piece of software is a dangerous and wrong myth.

Of course there is some script used to help on some specific task, file coded in few minutes for a specific task. But this is not development. A developer create program or service to be used.

Also, one man argue that their is situations where there is only one developer, kng of the code, but it is a double edge blade.
First, if we are speaking about profesionnal world, a company should never let the knowledge to only one person, this is a high risk if the employee to leave, go on vacation, or maybe even have some medical issue.

So, this the problem of the company, right? Not only. We can thing that the developer in this situation has the higher ground. Only if it want to be stuck with is work. Beeing a guardian of a legacy code is also giving up on the possibility to grow.

But if a developer want to evolve, learn new thing and keeping up with the pace of technology, it have to give up its creation, pass it to a padawane, or anyone willing to continue the project.

Therefore we learn beeing open to criticism, to remarks. No developer, and especialy the good one are perfect. Avoid to become  the [talented jerk](https://jobs.netflix.com/culture) company put aside.

Finally, a developer must keep in mind that most of the tools or language, it manipulate is available because a community give it freely. If we want our ecosystem to stay alive we need to give on our turn. That is why some company are know [cheking the activity in open source technology](https://opensource.com/article/19/5/how-get-job-doing-open-source).

# The new face of a developer

Belonging to a community, thinking ahead, sharing, eager to learn new thing, that is the new vision of a developer I would like to give. far from being a loner, but more like a craftsman, moving from new project to ne project, from masterpiece to masterpiece.
