---
show: true
width: 12
date: 2020-01-12 00:01:00 +0800
group: default
---

<h2>Professional Services</h2>

{% if site.data.profile.services.editorial %}
<h6>Editorial Roles</h6>
<ul class="list-unstyled mb-3">
{% for item in site.data.profile.services.editorial %}
<li class="mb-1">
    <div class="d-flex">
        <div>{{ item.title }}</div>
        <div class="ml-auto no-break"><em>{{ item.date }}</em></div>
    </div>
</li>
{% endfor %}
</ul>
{% endif %}

{% if site.data.profile.services.membership %}
<h6 class="mt-3">Professional Memberships</h6>
<ul class="list-unstyled mb-3">
{% for item in site.data.profile.services.membership %}
<li class="mb-1">
    <div class="d-flex">
        <div>{{ item.title }}</div>
        <div class="ml-auto no-break"><em>{{ item.date }}</em></div>
    </div>
</li>
{% endfor %}
</ul>
{% endif %}

{% if site.data.profile.services.reviewing %}
<h6 class="mt-3">Journal Reviewing</h6>
<p class="small mb-0">
{{ site.data.profile.services.reviewing }}
</p>
{% endif %}
