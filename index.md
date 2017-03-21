---
layout: page
title: Zxdposter's Blog
---


{% include JB/setup %}


{% for post in site.posts %}
<div class="article-card">
    <div>
        <section>
            <h3 class="title"><a href="{{ BASE_PATH  }}{{ post.url }}" >{{ post.title }}</a></h3>
            <summary class="desc">{{  post.desc}}</summary>
        </section>
        <div>{{ post.content | strip_html | truncate:20 }}</div>
        <span>{{ post.date }}</span>
    </div>
</div>
{% endfor %}

