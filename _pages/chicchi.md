---
layout: page
permalink: /chicchi/
title: "Chicchi di caffè, maginati in modo sicuro"
image:
  feature: java.jpg
  credit: Lilian Wong
  creditlink: https://flic.kr/p/7Ubonh
---

Il buongiorno di ogni buon pirata, parte con una dose di codice sicuro.
Pillole, trucchi, _snippet_ di codice, serviti caldi e tostati a punto giusto.
Prendeteli, adattateli, commentateli e fateli vostri.

{% assign chicchi = site.chicchi | sort: "order" %}

<ul>
{% for chicco in chicchi %}
  <li>Tazzina #{{chicco.order}}: <a href="{{chicco.url}}">{{chicco.title}}</a></li>
{% endfor %}
</ul>
