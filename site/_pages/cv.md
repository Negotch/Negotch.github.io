---
title: CV
permalink: /cv/
subtitle: Education, experience, and academic activities
---

{% if site.cv_pdf != '' and site.cv_pdf %}
{% if site.cv_pdf contains '://' %}

<p class="connect-links"><a href="{{ site.cv_pdf | escape }}">Download my CV (PDF) →</a></p>
{% else %}
<p class="connect-links"><a href="{{ site.cv_pdf | relative_url }}">Download my CV (PDF) →</a></p>
{% endif %}
{% endif %}

## Education

<p class="placeholder">[Degree, institution, and dates. Add your advisor or thesis title if relevant.]</p>

## Experience

<p class="placeholder">[Position, institution or organization, and dates.]</p>

## Awards and service

<p class="placeholder">[Add awards, professional service, and other academic activities.]</p>
