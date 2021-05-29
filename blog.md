---
layout: default
title: Blog
permalink: /blog/
---

<body>
   <div class="container" style="display: flex;">
       <div style="width: 70%;">
           <div class="posts">
              {% for post in site.posts limit:5 %}
                 <article class="post">
                    <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
                    <div class="entry">
                       {{ post.excerpt }}
                    </div>
                    <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
                 </article>
              {% endfor %}
           </div>
       </div>
       <div style="flex-grow: 1;">
           Right Div
       </div>
   </div>
</body>
