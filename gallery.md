---
layout: page
title: Gallery
---

{% for image in site.data.images %}
  ![{{image.short}}]({{site.baseurl}}/assets/img/{{image.img}}){:width="200px"}
  {{image.caption}} ([{{image.short}}, {{image.page}}](/counting-pebbles/bibliography#{{image.source}}))
{% endfor %}
