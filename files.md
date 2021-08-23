---
title: File List
---
<h1>Static File List</h1>
  <ul>
    {% for files in site.static_files %}
        <li class="timeline_card">
        {{ files.path }}
       </li>
    {% endfor %}
  </ul>
