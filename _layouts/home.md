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
  
    <section id="page-content">
  <div class="jumbotron">
    <div class="post-list">
  {%  for post in site.posts %}
  <div class="post-box">
    <div class="post-title">
    <a class="post-title" href="{{post.url | prepend:site.baseurl }}" > {{ post.title }}</a>
    </div>
    <div class="post-excerpt">
      {{ post.content | strip_html | truncatewords:20}}
    </div>
    <div class="posted">
      posted on
      <span class="posted-on">

        {{ post.date | date: "%A, %B %-d, %Y" }}
      </span>
      <span class="in">
        in
      </span>
      <span class="categories-on">
        {% for category in post.categories%}
        {{category}} &nbsp;{% if forloop.last %}{% else %},{% endif %}
        {% endfor %}
      </span>
    </div>
  </div>
  {% endfor %}
  </div>
</section>

    <p class="rss-subscribe">subscribe <a href="{{ " /feed.xml " | relative_url }}">via RSS</a></p>

</div>