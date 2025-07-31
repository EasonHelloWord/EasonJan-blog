---
layout: page
title: About
description: 打码改变世界
keywords: EasonJan, 蒋羿淳
comments: true
menu: 关于
permalink: /about/
---

我是蒋羿淳。

不怕犯错，努力创造人生。

## 社交平台

<ul>
{% for website in site.data.social %}
<li>{{ website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
</li>
{% endif %}
</ul>


## 技能清单

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
