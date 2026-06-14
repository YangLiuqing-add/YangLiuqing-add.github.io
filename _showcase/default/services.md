---
show: true
width: 12
date: 2020-01-12 00:01:00 +0800
group: default
---

<h2>Professional Services</h2>

<ul>
{% for item in site.data.profile.services %}
  <li>
    {{ item.name }}
    <span style="float:right"><em>{{ item.date }}</em></span>
  </li>
{% endfor %}
</ul>
