---
layout: page
title: About
description: 好好改变自己就好了
keywords: coder, Jerry
comments: true
menu: 关于
permalink: /about/
---

一个不宅略骚的技术党，喜欢社交。

目前喜欢研究的方向为计算机视觉方向、智能人机交互。

平时副业的兴趣爱好是历史和大国外交，思想上是一个合格的社会主义接班人。

本博客站点是建立在Github Pages之上的用于深度学习方面的学习博文以及论文摘记和相关项目的博文发表平台

针对LeetCode算法题刷题的题解发表在博客园的个人博客里。

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'mazhuang.org' %}
<li>
微信公众号：<br />
<img style="height:192px;width:192px;border:1px solid lightgrey;" src="{{ assets_base_url }}/assets/images/qrcode.jpg" alt="暂未开放" />
</li>
{% endif %}
</ul>


## Skill Keywords

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
