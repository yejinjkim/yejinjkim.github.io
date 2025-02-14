---
layout: page
title: "Team"
permalink: "/team"
---

## Antibody Design Team

Meet the researchers working at the intersection of AI and immunology.
![alt text](assets/images/antibody-group.png)

<div class="team">
  {% for member in site.data.team %}
    <div class="team-member">
      <img src="{{ member.headshot }}" alt="{{ member.name }}">
      <h3>{{ member.name }}</h3>
      <p>{{ member.position }}</p>
      <p><a href="mailto:{{ member.email }}">{{ member.email }}</a></p>
    </div>
  {% endfor %}
</div>

---

## LLM for Scientific Discovery Team

| Headshot | Name | Role | Contact |
|----------|------|------|---------|
| ![Name](/assets/images/team_member3.jpg){: width="100px" } | Emily Chang, PhD | Research Scientist | emily.chang@university.edu |
| ![Name](/assets/images/team_member4.jpg){: width="100px" } | Michael Brown | PhD Student | michael.brown@university.edu |

*(Add more team members as needed.)*
