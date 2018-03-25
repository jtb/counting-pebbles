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
      <td><img src="{{site.baseurl}}/assets/img/medium/{{photo.img}}" alt="{{artifact.name}}" width="100"></td>
      <td>{{artifact.name}}</td>
      <td>{{artifact.region}}</td>
      <td>
        <ul>
{% for inscript in artifact.inscriptions %}
          <li>{{inscript}}</li>
{% endfor %}
        </ul>
      </td>
      <td>{{artifact.details}}</td>
    </tr>
{% endfor %}
  </tbody>
</table>
