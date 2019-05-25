---
layout: page
title: 서울S치과의원 찾아가기
permalink: /direction/
category1: 찾아가기
---

<div class="row d-flex justify-content-center" id="info">

{% for post in site.pages %}
{% if post.title and post.category3 %}{% if post.category2 contains "찾아가기" %}
<div class="col-12">
<h4>{{ post.title }}</h4>
{{ post.content }}
</div>
{% endif %}{% endif %}
{% endfor %}

</div>
