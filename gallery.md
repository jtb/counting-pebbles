---
layout: page
title: Gallery
---

{% for image in site.data.images %}
<div>
<p>
  ![]({{site.baseurl}}/assets/img/{{image.img}}){:height="100px"}
</p>
<p>
  <i>{{image.caption}}</i> [{{image.short}}, {{image.page}}](/counting-pebbles/bibliography#{{image.source}})
</p>
</div>
{% endfor %}
