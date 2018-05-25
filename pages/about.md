---
layout: page
title: About
description: Keep Learning, Keep Thinking
keywords: Fengchong Wang
comments: true
menu: 关于
permalink: /about/
---
Hi there, I am a data scientist. I am interested in all types of machine learning, i.e., traditional statistical machine learning and modern deep learning.

I love learning new stuffs, sleeping, cooking and appreciating Chinese traditional caligraphy (unfortunately, I do not have much time to practice it).

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
