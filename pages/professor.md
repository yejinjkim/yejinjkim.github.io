---
layout: page
title: "Yejin Kim, PhD"
permalink: "/professor"
---

<div class="prof-head">
  <div class="prof-lines">
    <div>Associate Professor (tenured)</div>
    <div>Associate Director, Center for Secure Artificial Intelligence for Healthcare</div>
    <div>Department of Health Data Science and Artificial Intelligence</div>
    <div><a href="https://sbmi.uth.edu/">McWilliams School of Biomedical Informatics</a></div>
    <div><a href="https://www.uth.edu/">University of Texas Health Science Center at Houston</a></div>
    <div class="prof-contact">
      <div>{{ site.address_line1 }}<br>{{ site.address_line2 }}</div>
      <div><a href="mailto:{{ site.email }}">{{ site.email }}</a><br><a href="{{ site.linkedin }}">LinkedIn</a></div>
    </div>
  </div>
  <img class="grayscale prof-photo" src="{{ site.headshot | relative_url }}" alt="Yejin Kim, PhD">
</div>

<div class="prose" markdown="1">
Yejin Kim is a tenured Associate Professor and Associate Director of the Center for Secure Artificial Intelligence for Healthcare in the Department of Health Data Science and Artificial Intelligence. She received her Ph.D. in Applied Machine Learning from Pohang University of Science and Technology (POSTECH), South Korea.

Her research focuses on developing artificial intelligence algorithms for therapy development and biomedical discovery. Her work has advanced the field of biomedical AI through innovative machine learning methods and a strong record of externally funded research. Over the past five years, as principal investigator, she has secured more than $8 million in extramural research funding, including two NIH R01 grants. She has published more than 60 peer-reviewed papers in leading biomedical informatics journals, including *npj Digital Medicine*, *JAMIA*, *JMIR*, *Bioinformatics*, and the *Journal of Biomedical Informatics*, as well as premier artificial intelligence and machine learning conferences such as SIGKDD, ACL, and IJCAI.

Beyond her research, she has made substantial contributions to the scientific community through leadership and professional service. She has served on multiple NIH grant review panels and study sections, including CSR CDMA and HSS, and has reviewed research proposals for funding agencies in the United Kingdom, Canada, Israel, and Luxembourg. She serves as an Academic Editor for *PLoS Biology*, reviews manuscripts for leading journals including *Nature Communications* and *npj Digital Medicine*, and has served on the program committees of major AI conferences, including ICLR, NeurIPS, ACL, and AAAI.
</div>

{% for sec in site.data.cv %}
<section class="sec sec-ruled">
  <h2 class="sec-label">{{ sec.title }}</h2>
  <div class="rows">
    {% for row in sec.rows %}
      <div class="row"><div class="row-when">{{ row.when }}</div><div>{{ row.what }}</div></div>
    {% endfor %}
  </div>
</section>
{% endfor %}

<section class="sec sec-ruled">
  <h2 class="sec-label">Teaching</h2>
  <div class="rows">
    {% for c in site.data.courses %}
      <div class="row">
        <div class="row-when">{{ c.term }}</div>
        <div>{{ c.course }}{% if c.type %}<div class="row-note">{{ c.type }}</div>{% endif %}</div>
      </div>
    {% endfor %}
  </div>
</section>
