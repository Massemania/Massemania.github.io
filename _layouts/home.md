--- 
layout: default 
---


<div class="home">
  Welcome to my site the home of ME. My name is Mats Magnusson and I'm training to be a frontend developer. I'm a student at Linnaeus University in Sweden.
    The purpose of this site is to publish assignments in the course Clientbased webpgrogramming.  



    <h1 class="page-heading">Posts</h1>

    {{ content }}
  
    <ul class="post-list">
        {% for post in site.posts %}
        <li>
            {% assign date_format = site.minima.date_format | default: "%b %-d, %Y" %}
            <span class="post-meta">{{ post.date | date: date_format }}</span>

            <h2>
                <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
            </h2>
        </li>
        {% endfor %}
    </ul>

    <p class="rss-subscribe">subscribe <a href="{{ " /feed.xml " | relative_url }}">via RSS</a></p>

</div>