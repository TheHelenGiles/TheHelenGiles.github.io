---
layout: default
title: Blog
permalink: /blog/blog-archive
---

<body>
   <!-- <div class="container" style="display: flex;"> -->
       <!-- <div style="margin: 5px; width: 70%;">
           <h2>Posts</h2>
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
       </div> -->
       <!-- <div style="margin: 5px; flex-grow: 1;"> -->
       <h2>Archive</h2>
           {% for tag in site.tags reversed %}
             <h3>{{ tag[0] }}</h3>
             <ul>
               {% for post in tag[1] %}
                 <li>{{ post.date | date: "%B %e"}}: <i><a href="{{ post.url }}">{{ post.title }}</a></i></li>
               {% endfor %}
             </ul>
           {% endfor %}
       <!-- </div>
   </div> -->
</body>
