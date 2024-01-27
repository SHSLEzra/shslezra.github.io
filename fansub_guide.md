---
layout: page
title: "Fansubber útmutató"
permalink: /fansub_guide
---

2022 óta készülő útmutató a modern fansubolásról. További információkhoz olvasd el a bevezető cikket.  
Kezdőknek és másoknak kapcsolatépítéshez: [Magyar Fansub Közösség](https://discord.gg/gam4ZVWKvn)  
Ha pedig személyesen engem akarsz zaklatni: [shsl.ezra@gmail.com](mailto:shsl.ezra@gmail.com)

**Legutolsó frissítés: 2024.01.20. - az oldal feltöltés alatt áll**


## Cikkek / tartalomjegyzék
<ul>
  {% for post in site.posts | sort: "chapter" %}
	{% if post.categories contains "fansub" %}
		<li>
		  <a href="{{ post.url }}">{{ chapter }}. fejezet: {{ post.title }}</a>
		</li>
	{% endif %}
  {% endfor %}
</ul>


## Formázási útmutató

Jelenleg nem található cikk ebben a kategóriában.
<ul>
  {% for post in site.posts reversed %}
	{% if post.categories contains "formazas" %}
		<li>
		  <a href="{{ post.url }}">{{ post.title }}</a>
		</li>
	{% endif %}
  {% endfor %}
</ul>


## Időzítési és karaoke készítési útmutató

Jelenleg nem található cikk ebben a kategóriában.
<ul>
  {% for post in site.posts reversed %}
	{% if post.categories contains "idozites" %}
		<li>
		  <a href="{{ post.url }}">{{ post.title }}</a>
		</li>
	{% endif %}
  {% endfor %}
	
  {% for post in site.posts reversed %}
	{% if post.categories contains "karaoke" %}
		<li>
		  <a href="{{ post.url }}">{{ post.title }}</a>
		</li>
	{% endif %}
  {% endfor %}
</ul>