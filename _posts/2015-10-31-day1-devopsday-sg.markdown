---
layout: post
title:  "Day 1 - DevOps Day SG"
date:   2015-10-31
categories: devopsady sg
---

Recently I had the priviledge to attend and present at DevOps day singapore. The following are some of my afterthought and notes that I took.

Trent Hornibrook - 7 years of devops
============================
Trent's talk focus on the importance of people and organisation structure during a DevOps transformation. He shared his idea of DevOps - culture, value stream as well as toolings. 

* He shared his tips and trick for hiring the right people with the right culture fit, not just about the technical skills. 
* Organisation structure is equally important as Trent pointed out an insufficient organisation structure promote silos, as a result reduce the amount of collaboration between teams - which is the reverse of the core idea of DevOps. His suggestion is a transformation from silo team to squards with cross functional focus which include tooling focus, infra focus and delivery focus. 
* Another interesting challenge Trent has is working with remote team. He used the Hofsede culture study by IBM as a starting point to understand the cultural difference between different country in order to reduce the culture gap and be able to collaborate in a more effective way. 
* Last but not least, he suggested a clear defined goal will motivate team

#### My Afterthought
This is a talk where Trent shared his journey in REA focusing in tranformation into DevOps. He defined what constitue to DevOps and putting focus on people and organisation restructuring. There was interesting idea about working with remote team and how they made it work. The idea of Hofsede study worth looking at to gain a better insight for culture difference.

Anjkur Trivedi  - How a payroll processing company turned into a software release factory
========================================================================================
Anjkur shared his experience introducing CI/CD to a payroll processing company.

* The challenges he had with the payroll processing company was multiple tools, multiple integration point, lack of visibility and no or outdated metrics
* He oberved a reduce in maintance after consolidation of tool set
* Automation is also an important aspect in his journey to reduce the feedback loop between code checkin to production

#### My Afterthought
This is a talk about sharing the journey of a project optimization. There was a lot of mention about tools and about how standardize tools can inprove feedback time. It also touched on the requirement of doing "DevOps" like scm, getting metrics, CI/CD, artefact factory, org structure. There was also mentioned of the importance of empowering people and improve visibility revolve around the use of tools. 

Kiran Inampudi - Agile Service Provider Transformation
======================================================
Kiran from Cisco delivered a talk about the next thing after automating infrastructure - software defining networking.

* Kiran pointed out that with the increase of voice and video consumption for the past few years, the data usage around the world had increase by at least 10 folds. The demand will continue as contents become more accessible via different medium. Therefore the tradition way of overbuild for the peak hour will not work for the modern world anymore.
* He suggested that in the future, there will be a hybrid of software and hardware managed networking where we will have pipeline that create software managed network
* The notion of being able to test your network changes before rolling it out is very encouraging
* Traditionally networking is a very specialise skills but with the DevOps movement and the rise of software defining networking, it should reduce the knowledge gap and allow better collaboration between networking engineers and the rest of the organisation. 
* Some of the challenges that Kiran pointed out was the notion of managing hybrid networking infrastructure and the skill gop, in particular networking programming

#### My Afterthought
This talk focus on the concept of software defining networking which was an interetsing way of looking at networking. He predicted that the networking engineers will go through the same journey as how we transformed infra operations. He pointed out a few chanllenges like skill gaps, managing hybrid networking system and cultural changes required as traditionally networking had always been a very specialise skills. It was quite an interesting talk touching on this new topic that I found quite inspiring. There is still issue regarding to security, auditing and testing when going forward with this transition.

Siriam Narayanan & Prasanna K - Security and CD
===============================================
Sriram and Prasanna from ThoughtWorks shared their experience with working at a client where they are required to embedded security in the continuous delivery environment.

* Everyone in the industry are aware that security is a scary issue as it will lead to finanacial and reputation risk as well as legal ramifications but the fact that we always leave it till the end just doesn't make sens. They questioned - where is security not embedded as part of the development?
* They shared some of the thing we should look out for during development
    * tracebility and auditbility of packages to make sure who created it, when it was created and whether it had been tampered or not
    * keeping track of third party software to make sure the team is making sensible choice for the third party software they are using as there is risk involved for every third party software that we included in a project
* They also talked about how to ensure we have a secure infrastructure which included automating environment creation, automating hardening steps, GPG signed packages, tech stack scan and  using tools like brakemand and ZAP in the build pipeline to detect all the low hanging fruit issues so that we can utalize the pen tester to find more obscure security issue
* They also pointed out the importance of including the pen tester early in the development process as they have deep domain knowlege that not everyone have.

#### My Afterthought
We should make security as part of the development process. Security automation should be part of the development pipeline and it should be embedded in the team early in the engagament but automation cannot replace pen tester as there are a lot of special domain knowledge required in security testing.

Ignite talk
===========
HP

* Large organisation dont believe they can be agile or agile is about buying specific tools or getting certified.
* It is not true as a successful transition will involved sensible architecture decision and a culture change
* Core idea
   * talent and diversity and making it works
   * common culture
   * customer focus i.e. understand what they want hackerthon with customer
* integrate everyone together for collaboration
* build for failure - chaotic monkey to drive culture change
* monitoring and metrics

Kimble Ngo - amplfiying influence

* With the popularity of mobile devices, we often forgot the importance of connecting with real people
* connect with people to build relationship and get a better understanding of the person

Yue Lin

* defining what is agile
* as takes 21 days to get used to somethings therefore we should ask for feedback before 21 days as people are not use to the changes yet
* trust the team, empower them to innovate
* in order to make change stick, make the change consistent, stop switching between working practises and ideas too often

Jason Man Crawl before you run when implementing devops

* create an unified process to reduce barrier
* use automation to automate process and bring us together
* leave traditionally legacy applications alone and just focus on the new applications
* metrics is important
    * deployment frequency
    * value added
    * how often you failed and meantime to recovery

immutable image

* to solve the configuration drift
* there was question regarding to how to embedded secret
* another problem people might face is the need to update image for every changes

Open Space
==========

A lot of the open space topic was about containatisation as well as security.

* most people agree that docker is useful for testing and running ci slaves but in production, the lack of orchestration support just doesnt worth it
* some people end up running a container in an individual machine and load balancer the machine itself in order to keep all the environment consistent
* the idea of having ide integrated checks for security is very good for fail fast
