---
layout: post
title: "Being a developer beyong simple code"
description: "Meaning of being a developer and tackle mythologies"
thumb_image: "documentation/sample-image.jpg"
tags: [developer, philosophy]
---


What it means beeing a developer? What can we expected from him/her? The question is worst asking as there is many confusions. The mythical figure was, a long time ago the geeky genius, living in the dark, socially disabled, and evolved to the cool start up west cost millenials, but still staring at its screen, doing mystical things.

This image is conveyed by pop-culture by the simple equation, develop = producing code. Most of the time he is a bit hacker too. But ask him/her something and it will furiously type on its keyboard making its magic and creating the service that now worth millions, during the night.

<div class="embed-responsive embed-responsive-16by9">
<iframe src="https://www.youtube.com/embed/uxKmDWDUZ5A?modestbranding=1&autohide=1&showinfo=0&controls=0"  allowfullscreen></iframe>
</div>

Truth is, the magic is not that complicated, language and framework make development less and less complicated. So many people become developers, as it is, in the end, not so mystical. And, in the end, still bear this romantic representation.

This misconception engender some problems, when developer try to stick to this cliché we can see the emergence of frustration, from the developer itself frustrated to have to do somthing else, and frustration from the users who end-up using the engineer tools only understable by its creator.

# Coding is mere 20% of a project

One frequent mistake is to rush writing code, thinking that productivity is directly related to the number of lines written. Mistake because starting to code to fast is likely to give the following result :

* Unreadable code, only the creator will be able to navigate amongst the maze created, and forgot six month later.
* Lots of technical flows and lacking of optimisation
* Hard to debug
* Impossible to test

First thing to do is to plan and think ahead. The first tool to use is not an IDE, but the one that help to plan, either it is pen and paper, a white board, a post-it or any project management software.

Starting a project or a feature, I personally like to answer the following questions sequentially :

1. What is the logical sequence to make it works ?
2. How to decompose this sequence in smallest pieces (Object/Module/Libraries) ?
3. How will it run in production? What architecture?
4. How can I build a dev environment close to this architecture ?
5. How do I deploy and test? To make sure it works when used.

## 1. Think ahead how it will work

This first step is to outline the global behavior of the product, what are the inputs, the outputs. It is to translate the need expressed in common words into a need into technical solutions. Needs are not generally directly expressed with obvious statements like "I need to save this fields into a database", they are more likely like "I need to setup a site to sell my products". The developer is the one to propose implementation to a problem.

## 2. Decompose

With experience, one of the instinct a developer grow is to detect code smells, meaning piece of code that should not be this way. A block with too much conditions, or a methods doing to many things.

The key is to split into smallest methods, decompose the code into logical modules. Every methods should do only and only one thing as the [SOLID principles recommends](https://en.wikipedia.org/wiki/SOLID).
Done well, it should emerge some well known [design pattern](https://en.wikipedia.org/wiki/Software_design_pattern). Indeed, a design should fit to a need, and not to force a code to a design pattern

## 3. What will it be in production

Knowing and thinking where and how the code would run i production. Some would tell it is a sysadmin one, but in the end developing is also responsible to ask or build the architecture under. The [DevOps](https://en.wikipedia.org/wiki/DevOps) principle is mainly the formalization of that. 

I have seen many project failing because of a lake of communication between production team and developer, because of a setup notice to compicated and not suited to production needs, or production constraints that make a development to painfull and end up having an impact on user experience. 
Best projects are when dev and operator understand each other, and worked alongside.

## 4. Building dev environment

Stick close to the running environment while developing is a good way to avoid bad surprise when going into production. 

Fortunately most framework and languages provides everything, therefore it is easy to have a close to production setup thanks to [docker](https://en.wikipedia.org/wiki/Docker_(software)).

## 5. Create and tests

Last part is to have a good test suite to the development. I will not lie, tests runner are according to me still a work in progress, and quite painful to setup. And first tests are quite hard to setup. But once done, it ensure that the code is and remain perfectly working.

There are many steps to build a sustainable system. To avoid any headache, [Keep It Simple Stupide](https://en.wikipedia.org/wiki/KISS_principle) , the system should not be complicated, and easy to maintain.

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

The productivity of a developer is often measure using the number of line of code produce. It is a false and dangerous consumption. Sometime, the develpre impose itself this kind of pressure, afraid to be view as a slacker on review or at the end of the sprint. Truth is, the number of line is not important, what it mater, it is to cover feature with the fewer place of bug or case not treated. It need experience to understand that is take time to produce the perfect, yet small, piece of code. The goal is to have the fewer line of code as a small code has the benefits :

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
