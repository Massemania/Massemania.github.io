---
layout: post
comments: true
title:  "Comments and open graph"
date:   2017-11-05 17:42:23 -0500
categories: jekyll
author: Mats Magnusson
permalink: "/:title/"
---

#### What is humans.txt and how have you configure it for your site?
Humans.txt is a way to show that the site is made by humans. It is a text file with information about the different people who have contributed to the site.
The file is located at the root of the site. I have filled my humans.txt with info including who built the site and which softwares I've used.

#### How did you implements comments to blog posts
I've used the include disqus tool to make comments possible. You create an account on disqus and follow the steps on the website to configure data and appearance. Then you add a variable called _comments_ to the front matter and set it to true. Then you add {% raw %}`{% if page.comments %}`{% endraw %} and a  
{% raw %}`{{% endif}}`{% endraw %} where you want the disqus to load and paste the universal embeded code in your template.

This is done for interacting with the readers of your blog. Disqus supports rich media commenting to let readers add images and video to have a lively discussion.

#### What is Open Graph and how do you make use of it?
Open graph is a standard for marking which content should be showed, including an image and text. It is used on Facebook to have the same functionality as any other object on the page. You add basic metadata to your page, to turn into open graph objects. You use it for different object types including: text, images, music and video. I use it so when i add a link to my blog on facebook it will formatted in the right way.