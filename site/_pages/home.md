---
title: Home
permalink: /
---

<!-- ## Welcome. -->

Hi! I'm Yukai Tang, a third-year PhD student in the Department of Operations Research and Financial Engineering at Princeton, where I'm fortunate to be coadvised by Prof. [Amir Ali Ahmadi](https://aaa.princeton.edu/home) and Prof. [Pravesh K. Kothari](https://www.cs.princeton.edu/~kothari/). I am broadly interested in optimization, particularly semidefinite programming.

Before coming to Princeton, I received my B.Eng. in Electrical Engineering from Tsinghua University. In 2023, I had a great time working with Prof. [Heng Yang](https://hankyang.seas.harvard.edu/) at Harvard.

<!-- ## What I'm working on

<div class="work-grid">
  <article class="work-card">
    <h3>Research direction 1</h3>
    <p class="placeholder">[Introduce a research question and why it matters.]</p>
    <a href="{{ '/research/#research-direction-1' | relative_url }}">Learn more →</a>
  </article>
  <article class="work-card">
    <h3>Research direction 2</h3>
    <p class="placeholder">[Describe another area of your current work.]</p>
    <a href="{{ '/research/#research-direction-2' | relative_url }}">Learn more →</a>
  </article>
  <article class="work-card">
    <h3>Research direction 3</h3>
    <p class="placeholder">[Highlight a project or an emerging interest.]</p>
    <a href="{{ '/research/#research-direction-3' | relative_url }}">Learn more →</a>
  </article>
</div> -->

## Selected work

<ul class="selected-list">
  {% assign selected_work = site.data.selected_work | sort: 'date' | reverse %}
  {% for work in selected_work %}
  <li class="selected-item">
    <h3><a href="{{ work.url | escape }}">{{ work.title | escape }}</a></h3>
    <p class="work-meta">{{ work.authors | join: ', ' | escape }} · {{ work.venue | escape }} · {{ work.year }}</p>
  </li>
  {% endfor %}
</ul>

<!-- ## Let's connect

<p class="placeholder">[Add a short invitation to connect and your preferred contact information.]</p>

<div class="connect-links">
  {% if site.social_links.email != '' and site.social_links.email %}<a href="mailto:{{ site.social_links.email | escape }}">Email me</a>{% endif %}
  <a href="{{ site.social_links.github | escape }}">GitHub</a>
  {% if site.social_links.scholar != '' and site.social_links.scholar %}<a href="{{ site.social_links.scholar | escape }}">Google Scholar</a>{% endif %}
</div> -->
