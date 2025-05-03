---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

# Memory Leaks
*A collection of devlogs by a game student for tracking progress.*

Welcome to my development logs - a place where I document some of my side projects in order to track my progress.

<div class="content-separator"></div>

<div class="projectscontainer">
  {% for post in site.posts %}
  <a href="{{ site.baseurl }}{{ post.url }}"  class="project">
    <h2>{{ post.title }}</h2>
    <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
  </a>
  {% endfor %}
</div>