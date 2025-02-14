---
layout: page
title: "Team"
permalink: "/team"
---

## Antibody Design Team

Meet the researchers working at the intersection of AI and immunology.
![alt text](assets/images/antibody-group.png)

<div class="team">
  {% for member in site.data.team.antibody %}
    <div class="team-member">
      <img src="{{ member.headshot }}" alt="{{ member.name }}">
      <h3>{{ member.name }}</h3>
      <p>{{ member.position }}</p>
      <p>{{ member.expertise }}</p>
      <p><a href="mailto:{{ member.email }}">{{ member.email }}</a></p>
    </div>
  {% endfor %}
</div>

---

## LLM for Scientific Discovery Team

<div class="team">
  {% for member in site.data.team.llm %}
    <div class="team-member">
      <img src="{{ member.headshot }}" alt="{{ member.name }}">
      <h3>{{ member.name }}</h3>
      <p>{{ member.position }}</p>
      <p>{{ member.expertise }}</p>
      <p><a href="mailto:{{ member.email }}">{{ member.email }}</a></p>
    </div>
  {% endfor %}
</div>



