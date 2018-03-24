---
layout: page
title: Gallery
---

{% for image in site.data.images %}
<p>
  ![]({{site.baseurl}}/assets/img/{{image.img}}){:height="100px"}  
  <i>{{image.caption}}</i> [{{image.short}}, {{image.page}}](/counting-pebbles/bibliography#{{image.source}})
</p>
{% endfor %}
