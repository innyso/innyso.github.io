---
layout: post
title:  "Repository as an artefact"
date:   2015-05-01
categories: aptly repositoryAsArtefact
---

## Oh dear, yet another buzz word...
Well, yes maybe but hopefully you will be convince that this is an interesting concept after reading this blog post. Although repository and artefact are something that we are very familiar with but have we ever consider putting them together? There is a reason I am suggesting this and lets have a look at some of the scenarios trigger me to consider such approach in management the packages.

## In a normal world
In a typical development environment, we have developers, testers and ops working together developing and creating packages that are used as a deployable. As a lot of applications are moving towards a microservices architecture, an applications typical made up of a lot of packages each representing an indivdual microservice. In addition, usually third party packges are required to order to provide additional function for the applications. The following diagram represent a typical development environment.

## The Dependency hell...
Normally the above would work until we would like to have control on what we would like to deploy in each environment but 

_Do you remember the time that you practise continuous deployment and thinking that everything went smoothly in staging and nothing would go wrong in production._

_Do you remember you spent hours trying to figure out whats wrong and realised nginx got upgraded and you cant downgrade because the mirror doesnt provide old version of ngnix_

## Here come the auditing

## Rolling back and forward

## Signing Signing Signing

## Everyone like simpler code



