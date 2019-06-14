---
layout: page
title: 잠실새내역에서 서울S치과 가는 법
permalink: /metro/
category1: 찾아가기
category2: 잠실새내역에서
published: true
---

<div id="info">
{% for item in site.data.direction %}
<div class="row">
<div class="col-lg-4">{{ forloop.index }}. {{item.caption}}</div>
<div class="col-lg-8 p-2 d-flex justify-content-center"><img src="{{site.url}}/img/{{item.photo}}"></div>
</div>
{% endfor %}

</div>
