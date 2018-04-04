---
layout: page
title: Lined Tablets
---

<table>
  <tbody>
    <tr>
      <th>Image</th>
      <th>Name</th>
      <th>
        <div>Inscriptions</div>
        <div><small><sup>x</sup> Xs on lines</small></div>
        <div><small><sup>⟂</sup> vertical line</small></div>
        <div><small><sup>◗</sup> semi-circle</small></div>
      </th>
    </tr>
{% for artifact in site.data.artifacts %}
{% assign photo = site.data.images | where:"id", artifact.photo  | first %}
    <tr>
      <td><a href="{{site.baseurl}}/assets/img/Cargill/{{photo.img}}" data-lightbox="{{artifact.id}}" data-title="{{artifact.name}}">
            <img src="{{site.baseurl}}/assets/img/Cargill/{{photo.img}}" alt="{{artifact.name}}" width="100">
      </a></td>
      <td>{{artifact.name}}</td>
      <td>
{% for line in artifact.lines %}
        <div>{{line.number}} lines{% if line.broken %} (broken){% endif %}
          {%- if line.hasXs -%}<sup>x</sup>{%- endif -%}
          {%- if line.hasVert -%}<sup>⟂</sup>{%- endif -%}
          {%- if line.hasSC -%}<sup>◗</sup>{%- endif -%}
        </div>
{% endfor %}
{% for inscript in artifact.inscriptions %}
        <div class="gfs">{{inscript}}</div>
{% endfor %}
      </td>
    </tr>
{% endfor %}
  </tbody>
</table>
