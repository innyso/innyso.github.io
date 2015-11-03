---
layout: post
title:  "Repository as an artefact"
date:   2015-05-01
categories: aptly repositoryAsArtefact
---

Microservice architecture is a great idea which allow us to create simplier and more flexible application but the raise of such architecture also create other problems.

## So What is the problem
In a typical development environment, we have developers, testers and ops working together developing and creating packages that are used as a deployable. An application typical made up of a lot of packages each representing an indivdual microservice, along with a bunch of third party packages. 

Sounds pretty good right? What can possibly go wrong. Along with all the infrastructure automation and CI/CD, nothing can possibly go wrong!

## So there is no problem right?
Well, just imagine the following:

_Deployment went through smoothly in development and staging, you thought nothing can possibly go wrong, and then you found out nginx roll out a new version and they remove the old version_

Sounds familiar right? Now you are in a position where you are forced to upgrade and fix the problem. 

## Repository as an artefact come for rescue
The idea is to create a snapshot of your current repository, version it, test it and then promote it to the next environment.

Lets have a look at an example:


## Aptly
I had been using aptly for the last 6 months to achieve the above. Without any of the features, aptly is just a good old debian repository. What make it different is the ability to take snapshot and cherrypick particular packges to go into the final snapshot. 

Lets have a look at the following example together:

## What does it mean now?
The act of deployment is just a matter of serving the correct version of repository using your favoriate web server. Your infrastructure code dont need to pin to a particular version of package but at the same time developers still have the opportunity to try the latest and greatest tools by creating their own custom repository artefact. 

Along with all the automation, by treating your repository as an artefact can ensure the consistency during deployment. No one like surprises! 

## But we have this thing call container...
Using container is actually the next step to achieve consistency and make deployment simplier. Although it is a really hot topic at the moment, in reality there are a lot of companies that are not willing to jump onto the container wagon due to its immaturity like lack of orchestration support, security concern etc. So treating your repository as an artefact can be an inbetween solution to your current infrastructure.

##Useful links

