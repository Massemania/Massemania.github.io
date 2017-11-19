--- 
layout: default 
---

<div class="home">

    <h1>Welcome to my tiny site!</h1>
    <hr><br>
    <blockquote>You want to follow an older student on his way to become a senior front-end developer? Than follow me on my ups and downs during the whole process. It's gonna be a lot of fun and it will include a lot of hard work. But who doesn't love a challenge? You have to love the process to accomplish your goals!`</blockquote>
    <br><hr><br><br>
    <h1 class="page-heading">Latest Posts</h1>

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