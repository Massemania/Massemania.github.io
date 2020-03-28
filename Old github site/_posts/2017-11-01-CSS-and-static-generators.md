---
layout: post
comments: true
title:  "CSS and static generators"
date:   2017-11-01 17:42:23 -0500
categories: jekyll
author: Mats Magnusson
permalink: "/:title/"
---


#### What do I think of pre-compiling your CSS?
I think it's good there a several advantages. For example you have the ability to define variables and mathematical functions.
#### Compare to regular CSS Which techniques did I use? 
I used SCSS or SASS to make my CSS better. I used variables, nested syntax and mixins.
#### Pros and cons? 
There is mostly pros, the only con I can think of that you have to compile SCSS.
#### What do you think of static site generators?
Well I've only worked with Jekyll, but I like what I see. It's fast, it's smart and it's easy to learn. You can do great things with little effort.
#### What type of projects are they suitable for? 
Static sites, like a presentation of a company or a blog. It's not suited if you want to have a lot of interactions, like a database or complex javascript.
#### What is robots.txt and how have you configure it for your site?
It's a text file containing information about pages on your website for crawlers. It creates a sitemap that tells the crawlers the structure and pages it should index.
I read a guide to implement it, first I installed a plugin called `jekyll-sitemap` and then I added a standard robots.txt file where I specify the to my sitemap.