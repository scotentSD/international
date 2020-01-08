---
title: Research timeline
---

<section id="timeline">
<h1>Research timeline</h1>
 {% include key.html %}


<ul class="timeline_ul">
  {% for post in site.posts %}
      <li class="timeline_card">
        <div class="timeline_head {{post.type}}">
           <a href="{{site.url}}/{{site.github.repository_name}}{{post.url}}">
            <div class="date_{{post.type}}" > {{ post.display_date }} </div>
            <!-- <br>  -->
            <div class="title_{{post.type}}" >{{post.title}} </div>  
          </a>
        </div>
        <div class="timeline_body">
           {{ post.excerpt }}
        </div>
        <!-- <span class="initials">{{ post.initials }}</span> -->
     </li>
  {% endfor %}
</ul>
</section>
