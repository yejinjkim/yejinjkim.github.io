---
layout: page
title: "Research Opportunities"
permalink: "/opportunities"
---

<p class="page-lead">As a PhD student or postdoc in our group, you will work in a high-impact research environment, collaborate with scientists across disciplines, and contribute to advancements in biomedical AI.</p>

<section class="sec-ruled">
  <h2 class="sec-label">Why join our research group</h2>
  <div class="cells-2">
    {% for r in site.data.opportunities.reasons %}
      <div class="cell">
        <div class="cell-title">{{ r.title }}</div>
        <p>{{ r.body }}</p>
      </div>
    {% endfor %}
  </div>
</section>

{% for o in site.data.opportunities.openings %}
<section class="opening sec-ruled">
  <h2 class="opening-title">{{ o.title }}</h2>
  <div>
    <p>{{ o.body }}</p>
    {% if o.steps %}
      <ol class="steps">
        {% for s in o.steps %}<li>{{ s }}</li>{% endfor %}
      </ol>
    {% endif %}
    <a class="small-link" href="mailto:{{ site.email }}">Email me with your CV &rarr;</a>
  </div>
</section>
{% endfor %}
