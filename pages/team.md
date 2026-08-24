---
layout: page
title: "Team"
permalink: "/team"
---

{% for group in site.data.team %}
<section class="sec-ruled">
  <h2 class="sec-label">{{ group.name }}</h2>
  <div class="team-grid">
    {% for m in group.members %}
      <div class="team-cell">
        <div class="team-name">{{ m.name }}</div>
        <div class="team-pos">{{ m.position }}</div>
        <div class="team-exp">{{ m.expertise }}</div>
        <a class="small-link" href="mailto:{{ m.email }}">{{ m.email }}</a>
      </div>
    {% endfor %}
  </div>
</section>
{% endfor %}
