---
title: Home
permalink: /
---

## Welcome.

I'm Yukai Tang. Welcome to my personal website.

<p class="placeholder">[Add a short biography: your current role, affiliation, and the questions that motivate your research.]</p>

<p class="placeholder">[Share a little about your background, interests, or life outside research.]</p>

## What I'm working on

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
</div>

## Selected work

<ul class="selected-list">
  <li class="selected-item">
    <h3><a href="{{ '/publications/' | relative_url }}">[Selected publication or project title]</a></h3>
    <p class="placeholder">[Summarize the main result and its significance in one or two sentences.]</p>
  </li>
</ul>

## Let's connect

<p class="placeholder">[Add a short invitation to connect and your preferred contact information.]</p>

<div class="connect-links">
  {% if site.social_links.email != '' and site.social_links.email %}<a href="mailto:{{ site.social_links.email | escape }}">Email me</a>{% endif %}
  <a href="{{ '/cv/' | relative_url }}">View my CV</a>
  <a href="{{ site.social_links.github | escape }}">GitHub</a>
  {% if site.social_links.scholar != '' and site.social_links.scholar %}<a href="{{ site.social_links.scholar | escape }}">Google Scholar</a>{% endif %}
</div>
