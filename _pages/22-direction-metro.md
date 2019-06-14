---
layout: page
title: 잠실새내역 → 서울S치과 가기
permalink: /metro/
category1: 찾아가기
category2: 잠실새내역에서
published: true
frontpage: true
---

<div id="info">

{% for item in site.data.direction %}
<div class="card mb-3">
  <div class="card-body">
    <div class="row">
      <div class="col-lg-8 p-2 "><img class="shadow" src="{{site.url}}/img/{{item.photo}}"></div>
      <div class="col-lg-4 mb-4 ">{{ forloop.index }}. {{item.caption}}</div>
    </div>
  </div>
</div>
{% endfor %}

<div class="mb-4">길 찾기 어려우시면 언제든지 전화 주세요~ <i style="width: 1.5em;" class="fa fa-phone"></i><a href="tel:+82222027528">02-2202-7528</a><a href="tel:+82222027529">~9</a></div>

</div>
