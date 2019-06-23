---
title: Docker as a virtual Environment
author: Shan Islam
date: '2019-06-23'
slug: docker-as-a-virtual-environment
categories: []
tags: [docker, data science]
toc: no
---

There are loads of posts out there about Docker on how it works and building pipelines.

This post is more about Docker from a data science point of view. Docker can be great when you need to deploy a pipeline,API and models to be run.

However in my work I've come across situations where colleagues can't use a package because they don't have java installed or they do but the version is incompatible with their needs. This means then cants use some packages because of r or python on their machine.

This is my approach on creating a docker environment that everyone can work out. 


This may not be best practice and you may not have issues in your team like these. 

The point is people are able to set up the environment and run the scripts without any issues. This allows them to contribute and work on it.

Ok, you may have a project like this already. I'll do this in 3 parts. Python environment, Java

Src
data
Requirements.txt
Jaydebeapi

Set up the dockerfile. Install git
Credentials file
Explain each step,

Pycharm editor

Docker build
Docker run
And you should be able to do everything else