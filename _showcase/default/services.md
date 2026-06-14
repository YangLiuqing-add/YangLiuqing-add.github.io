---
show: true
width: 12
date: 2020-01-12 00:01:00 +0800
group: default
---

<h6>Professional Services</h6>

<ul class="list small pl-3 mb-1">
{% for item in site.data.profile.services %}
<li>
    <div class="d-flex">
        <div>{{ item.name }}</div>
        <div class="ml-auto mt-auto no-break">
            <em>{{ item.date }}</em>
        </div>
    </div>
</li>
{% endfor %}
</ul>
