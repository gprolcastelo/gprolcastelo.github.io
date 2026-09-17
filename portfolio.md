---
layout: page
title: Portfolio
---
<p class="section-intro">A selection of projects and repositories I'm proud of.</p>

<ul class="portfolio-list">
{% for project in site.data.portfolio %}
  <li class="portfolio-item">
    <img src="{{ project.image | relative_url }}" alt="{{ project.name }} figure" class="portfolio-figure">
    <div class="portfolio-body">
      <h2><a href="{{ project.repo_url }}" target="_blank" rel="noopener">{{ project.name }}</a></h2>
      {% if project.stack %}<p class="portfolio-stack">{{ project.stack }}</p>{% endif %}
      <p>{{ project.description }}</p>
      {% if project.attribution %}<p class="portfolio-attribution">{{ project.attribution }}</p>{% endif %}
    </div>
  </li>
{% endfor %}
</ul>
