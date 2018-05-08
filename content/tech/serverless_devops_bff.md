---
title: "#serverless + #devops = 💖bff💖"
date: 2018-05-07T21:08:54-07:00
draft: true
tags: ["devops", "speaking", "ignite", "serverless"]
---

# Cloud Computing, in 200 words or less
There are a few things that I like about my job. One of them is that [we](https://instagr.am/realselflife) are willing to take some managed risks. Another is that we are happy and willing to learn from failure.

One of the changes that we went through over 2017 was getting *very* familiar with [#serverless](/tags/serverless/). For those of you that aren't in the Cloud Computing Business, #serverless is this **terrible** word that we're using to describe a computing model where *an event* ( like a web request ) triggers *an execution* ( aka causes some code to run ). Relatively boring stuff, and to the unitiatied, it may seem very much like the way computer 💩 has always worked.

Is this #serverless thing really big deal you ask? **YES.** IMO, #serverless is the first truly Cloud Native implementation for computing. For most of every moment in history, you had to pay for the privilege of having a computer sitting by idle, waiting to receive traffic from users ( commonly called `heating air`). Once that traffic was received, we'd execute some code. There's usually also code surrounding the code that you want to execute to handle your user's intent. In #serverless, you mananage **NONE** of that surrounding layer. No Operating Systems, No Webservers, No Message Busses. Only the code that handles your **already serialized** user request.  

Hi 20 year old me. Your SysAdmin job is going to eventually disappear 👋. 

# So I wrote this talk...







Historically, our major knob for controlling utilization has been [AutoScaling](https://aws.amazon.com/autoscaling/). Autoscaling is when you adjust your computing capacity up or down based on some metric ( like number of requests ). Autoscaling is sort of like a road that gets wider as more cars traverse it. There's all kinds of disclaimers and caveats to using it, including some **occasionally harrowing** relationships to how automotive traffic works in [the real world](https://en.wikipedia.org/wiki/Induced_demand#Elasticity_of_transport_demand).



1. Cloud libraries are a first class citizen
1. Execution time is limited
1. There's an `at least once` invocation semantic, which is in itself a big change



# I wrote an [ignite](http://www.ignitetalks.io/) talk.