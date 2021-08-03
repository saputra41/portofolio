---
layout: page
title: About
permalink: /about/
weight: 3
---

# **About Me**

Hi I am **{{ site.author.name }}** :wave:,<br>
Fresh graduate of Diploma 3 Informatics Engineering, Dian Nuswantoro University Semarang. Have experience in developing Web and Mobile App for jasTukang. I have an interest in a career as an Developer in the field of Websites and Android application and improve my skills to be better than before.

<div class="row">
<div class="row col-12" style="margin-bottom: -25px;">
{% include about/skills.html title="Programming Skills"%}
</div>
{% include about/skills.html source=site.data.programming-skills %}
{% include about/skills.html source=site.data.other-skills %}
</div>

<div class="row">
{% include about/timeline.html %}
</div>
