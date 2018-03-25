---
layout: page
title: Artifacts
---

<table>
  <tbody>
    <tr>
      <th>Image</th>
      <th>Name</th>
      <th>Region</th>
      <th>Inscriptions</th>
      <th>Details</th>
    </tr>
{% for artifact in site.data.artifacts %}
{% assign photo = site.data.images | where:"id", artifact.photo  | first %}
    <tr>
      <td><a href="{{site.baseurl}}/assets/img/medium/{{photo.img}}" data-lightbox="{{artifact.id}}" data-title="{{artifact.name}}">
            <img src="{{site.baseurl}}/assets/img/medium/{{photo.img}}" alt="{{artifact.name}}" width="100">
      </a></td>
      <td>{{artifact.name}}</td>
      <td>{{artifact.region}}</td>
      <td>
{% for inscript in artifact.inscriptions %}
        <p class="gfs">{{inscript}}</p>
{% endfor %}
      </td>
      <td>{{artifact.details}}</td>
    </tr>
{% endfor %}
  </tbody>
</table>
