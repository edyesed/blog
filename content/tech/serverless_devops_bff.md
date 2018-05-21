---
title: "#serverless + #devops = 💖bff💖"
date: 2018-05-07T21:08:54-07:00
draft: true
tags: ["devops", "speaking", "ignite", "serverless"]
---

# Cloud Computing, in 300 words or less
There are a few things that I like about [my job](https://www.realself.com/about/jobs). One of them is that [we](https://instagr.am/realselflife) are willing to take some managed risks. Another is that we are happy and willing to learn from failure.

![spongebob thumbsup](https://media.giphy.com/media/3o7abKhOpu0NwenH3O/giphy.gif)

One of the changes that we went through over 2017 and 2017 was getting *very* familiar with [#serverless](/tags/serverless/). For those of you that aren't in the Cloud Computing Business, #serverless is this **terrible** word that we're using to describe a computing model where an *event* ( like a web request ) triggers *an execution* ( aka causes some code to run ). Relatively boring stuff, and to the uninitiated, it may seem very much like the way computer 💩 has always worked. There are two major differences, though. First: **you only pay for what you use.** Second: **you explicitly offload transportation concerns to your cloud, and you only handle "business logic".**

\#serverless is the first truly Cloud Native implementation for computing. For most of every moment in history, you had to pay for the privilege of having a computer sitting by, _idle_. The computer would just wait to receive traffic from users ( commonly called `heating air`). Once that traffic was received, we'd execute some code. There's usually _also_ code surrounding the code that you want to execute to handle your user's intent. Code that must be patched on a regular basis. **In #serverless, you mananage _NONE_ of that surrounding layer. No Operating Systems, No Webservers, No Message Busses. Only the code that handles your _already deserialized_ user request.**

Is this #serverless thing really big deal, you ask? **YES.**

Are there really servers in #serverless? **Yes, and it doesn't matter**

![jeff goldblum change the world](https://media.giphy.com/media/l0MYHQ87FqZPumhI4/giphy.gif)

----
# So, I wrote an [ignite](http://www.ignitetalks.io/) talk.
I wrote this talk because of all of the following:

* I think **[our story](https://instagr.am/realselflife)** is one that other people can at least relate to, possibly learn from.
* I'm excited about what #serverless represents for **[Development](https://en.wikipedia.org/wiki/Software_development)** & **[Operations](https://en.wikipedia.org/wiki/Computer_operator)**
* Public speaking is a personal goal I'm persuing to work on my **[Communication Skills](https://en.wikipedia.org/wiki/Communication)**

![little girl with cotton candy much excite](https://media.giphy.com/media/xTiN0CNHgoRf1Ha7CM/giphy.gif)

----

## our story
[realself](https://www.realself.com) builds a product where human beings share stories of, and seek trusted informtion about, their personal journeys of transformation. It's a big deal for our users, who are engaged in these life changing journeys, and it's a big deal for us to be entrusted with those stories.

When I was interviewing at realself, one moment really stood out for me. It was my first indication that realself was doing things differently from other places that I had worked. A dramatic recreation follows. 

>VP of Engineering> **\(describes a world where developers don't need to understand anything about operations\)** what do you think about that vision? 

>Me> **\(uncomfortable laughter\)** oh boy, I've heard that one before. I've built some opinions on it that you may not care to hear.

>VP of Engineering> Tell me more, we hire people for their opinions

![Jeff Goldblum leaning over, saying tell me more](https://media.giphy.com/media/10bDoTtJhtcHu0/giphy.gif)

The VP of Engineering had been shooting me straight. I do have [agency](https://www.merriam-webster.com/dictionary/agency) in my capacity as a team member at realself. ( We're almost always [hiring](https://www.realself.com/about/jobs), if you're looking and into that sort of thing. ) We've built a variety of different types of systems



## Changes for Development & Operations

## Personal Changes


Historically, our major knob for controlling utilization has been [AutoScaling](https://aws.amazon.com/autoscaling/). Autoscaling is when you adjust your computing capacity up or down based on some metric ( like number of requests ). Autoscaling is sort of like a road that gets wider as more cars traverse it. There's all kinds of disclaimers and caveats to using it, including some **occasionally harrowing** relationships to how automotive traffic works in [the real world](https://en.wikipedia.org/wiki/Induced_demand#Elasticity_of_transport_demand).



1. Cloud libraries are a first class citizen
1. Execution time is limited
1. There's an `at least once` invocation semantic, which is in itself a big change

