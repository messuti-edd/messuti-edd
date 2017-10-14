---
layout: page
title: Portfolio
permalink: /portfolio/
---

<div class="container portfolio_projects">
  <div class="portfolio-items">
    {% for project in site.projects %}
      <div class="project_container">
        <a class="project_img" href="{{ project.url | relative_url }}" style="background-image:url({{ project.images | first }})" />
        <a class="project_name" href="{{ project.url | relative_url }}">{{ project.title | escape }}</a>
      </div>
    {% endfor %}
  </div>
</div>
