---
layout: page
title: "Fansubber útmutató"
permalink: /fansub_guide
---

2022 óta folyamatosan készülő útmutató a modern fansubolásról. További információért olvasd el a bevezető cikket.  
Kezdőknek és másoknak kapcsolatépítéshez: [Magyar Fansub Közösség](https://discord.gg/gam4ZVWKvn)  

**Szerzők:** Ezra, [Nihil]({%link _authors/nihil.md %})

**Legutolsó frissítés: 2024.01.28. - az oldal feltöltés alatt áll**


## Cikkek / tartalomjegyzék
{% assign sorted_posts = site.posts | sort: 'chapter' %}
<ol>
  {% for post in sorted_posts %}
	{% if post.tags contains "technikai" %}
		<li>
		  <a href="{{ post.url }}">{{ post.title }}</a>
		</li>
	{% endif %}
  {% endfor %}
</ol>


## Formázási útmutató
{% assign sorted_posts = site.posts | sort: 'chapter' %}
<ol>
  {% for post in sorted_posts %}
	{% if post.categories contains "formazas" %}
		<li>
		  <a href="{{ post.url }}">{{ post.title }}</a>
		</li>
	{% endif %}
  {% endfor %}
</ol>


## Időzítési és karaoke készítési útmutató

Jelenleg nem található cikk ebben a kategóriában.

{% assign sorted_posts = site.posts | sort: 'chapter' %}
<ol>
  {% for post in sorted_posts %}
	{% if post.categories contains "idozites" %}
		<li>
		  <a href="{{ post.url }}">{{ post.title }}</a>
		</li>
	{% endif %}
  {% endfor %}
</ol>
	
{% assign sorted_posts = site.posts | sort: 'chapter' %}
<ol>
  {% for post in sorted_posts %}
	{% if post.categories contains "karaoke" %}
		<li>
		  <a href="{{ post.url }}">{{ post.title }}</a>
		</li>
	{% endif %}
  {% endfor %}
</ol>