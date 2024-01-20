---
layout: page
title: "Fansubber útmutató (2022)"
permalink: /fansub_guide
categories: [fansub, formazas, idozites, karaoke]
---

2022 óta készülő útmutató a modern fansubolásról. További információkhoz olvasd el a bevezető cikket.

Kezdőknek és másoknak kapcsolatépítéshez:

Ha pedig személyesen engem akarsz zaklatni:


**Legutolsó frissítés: 2024.01.20. - az oldal feltöltés alatt áll**


# Cikkek / tartalomjegyzék

<ul>
  {% for post in site.posts %}
	{% if post.cathegories contains "fansub" %}
		<li>
		  <a href="{{ post.url }}">{{ post.title }}</a>
		</li>
	{% endif %}
  {% endfor %}
</ul>


## Formázási útmutató

<ul>
  {% for post in site.posts %}
	{% if post.cathegories contains "formazas" %}
		<li>
		  <a href="{{ post.url }}">{{ post.title }}</a>
		</li>
	{% endif %}
  {% endfor %}
</ul>
