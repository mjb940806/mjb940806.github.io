---
layout: default
work: true
main: true
title: Etc.
description: 그 외 기록하고 싶은 내용
project-header: true
header-img: "img/project_bg.jpg"
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.etcs == true %}

     {% include post-list.html %}

{% endif %}
{% endfor %}
</div>