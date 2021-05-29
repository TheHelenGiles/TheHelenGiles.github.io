---
layout: default
title: Blog
permalink: /blog/
---

# Posts

(For a directory of blog posts, click [here]({{ site.baseurl }}/blog/directory))

---
<div class="posts">
    {% for post in site.posts limit:50 %}
        <article class="post">
            <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
            <div class="entry">
                {{ post.excerpt }}
            </div>
            <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">...</a>
        </article>
    {% endfor %}
</div>
