---
layout: default
permalink: /en/blog/
---

# Posts

(For a directory of blog posts, click [here]({{ site.baseurl }}/en/blog/directory))

---
<div class="posts">
    {% for post in site.posts limit:50 %}
        <article class="post">
            <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
            <div class="entry">
                {{ post.excerpt }}
            </div>
            <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">(continue reading...)</a>
        </article>
    {% endfor %}
</div>
