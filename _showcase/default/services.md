---
show: false
width: 12
date: 2020-01-12 00:01:00 +0800
group: default
---

<h2>Professional Services</h2>

<h6>Editorial Roles</h6>

<ul class="list-unstyled">
{% for item in site.data.profile.services.editorial %}
<li>
    <div class="d-flex">
        <div>{{ item.title }}</div>
        <div class="ml-auto">
            <em>{{ item.date }}</em>
        </div>
    </div>
</li>
{% endfor %}
</ul>

<h6 class="mt-3">Professional Memberships</h6>

<ul class="list-unstyled">
{% for item in site.data.profile.services.membership %}
<li>
    <div class="d-flex">
        <div>{{ item.title }}</div>
        <div class="ml-auto">
            <em>{{ item.date }}</em>
        </div>
    </div>
</li>
{% endfor %}
</ul>

<h6 class="mt-3">Journal Reviewing</h6>

<p class="small">
{{ site.data.profile.services.reviewing }}
</p>
