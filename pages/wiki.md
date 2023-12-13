---
layout: page
title: Wiki
description: The more I learn, the less I k
keywords: 维基, Wiki
comments: false
menu: Wiki
permalink: /wiki/
---

<ul class="listing">
{% for wiki in site.wiki %}
{% if wiki.title != "Wiki Template" %}
<li class="listing-item"><a href="{{ site.url }}{{ wiki.url }}">{{ wiki.title }}</a></li>
{% endif %}
{% endfor %}
</ul>
