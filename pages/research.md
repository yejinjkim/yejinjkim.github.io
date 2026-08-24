---
layout: page
title: "Research"
permalink: "/research"
---

<p class="page-lead">Four active directions, from method development to prospective experimental validation.</p>

{% for area in site.data.research %}
<section class="area">
  <div>
    <div class="area-num">{{ forloop.index | prepend: '0' | slice: -2, 2 }}</div>
    <h2 class="area-title">{{ area.title }}</h2>
    <p>{{ area.blurb }}</p>
    <div class="area-work">{{ area.work }}</div>
    {% if area.url %}<a class="small-link area-more" href="{{ area.url | relative_url }}">Details &rarr;</a>{% endif %}
  </div>
  {% if area.image %}
  <figure>
    <img class="grayscale area-img" src="{{ area.image | relative_url }}" alt="{{ area.title }}">
    <figcaption>{{ area.caption }}</figcaption>
  </figure>
  {% endif %}
</section>
{% endfor %}

<section class="sec-ruled">
  <h2 class="block-title">Funding</h2>
  <p class="page-lead">More than $8M in extramural funding as principal investigator over the past five years.</p>
  {% for g in site.data.funding %}
    <div class="grant">
      <div>
        <div class="grant-id">{{ g.id }}</div>
        <div class="grant-meta">{{ g.role }} &middot; {{ g.duration }}</div>
      </div>
      <div>
        <div class="grant-title">{{ g.title }}</div>
        <p>{{ g.description }}</p>
      </div>
    </div>
  {% endfor %}
</section>
