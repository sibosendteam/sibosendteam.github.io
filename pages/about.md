---
layout: page
title: About
description: 聪明在于勤奋，天才在于积累
keywords: sibosend,sibosend team,思博欣达
comments: true
menu: 关于
permalink: /about/
---

聪明在于勤奋，天才在于积累。

Sibosend Team

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
