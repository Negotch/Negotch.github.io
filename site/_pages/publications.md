---
title: Publications
permalink: /publications/
subtitle: Papers, preprints, and selected work
---

## Publications

<ul class="selected-list">
  {% assign selected_work = site.data.selected_work | sort: 'date' | reverse %}
  {% for work in selected_work %}
  <li class="selected-item">
    <h3><a href="{{ work.url | escape }}">{{ work.title | escape }}</a></h3>
    <p class="work-meta">{{ work.authors | join: ', ' | escape }} · {{ work.venue | escape }} · {{ work.year }}</p>
  </li>
  {% endfor %}
</ul>

{% if site.social_links.scholar != '' and site.social_links.scholar %}

<p><a href="{{ site.social_links.scholar | escape }}">See all publications on Google Scholar →</a></p>
{% endif %}
