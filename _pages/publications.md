---
layout: page
permalink: /publications/
title: 配布物 
description: 三鷹ハードウェアエンジニアカフェは、以下のオリジナルのドキュメント／ソースコード等を配布しています。
years: [1956, 1950, 1935, 1905]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
