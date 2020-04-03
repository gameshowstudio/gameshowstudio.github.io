---
layout: page
title: Game Show Studio Updates
permalink: /updates/
---

{% assign pages = site.pages | where: "layout", "update" | sort: "updateversion" | reverse %}
{% for page in pages %}

<div class="content-automerged-on-one-page">
<h2>Version {{page.updateversion}}</h2>
<p>{{page.content}}</p>
</div>

<br>

----

<br>

{% endfor %}
