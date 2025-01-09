---
title: "News"
layout: textlay
excerpt: "ECQOS Lab at the University of São Paulo."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br> {{ article.headline | markdownify}}</p>
{% endfor %}
