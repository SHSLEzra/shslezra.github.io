---
layout: page
title: "Fansub alapok kezdőknek"
permalink: /fansub_alapok
---
Szóval animéket szeretnél fordítani? Hát rendben.
Akkor a legjobb helyre jöttél: eme rövid cikksorozatban összefoglalom, hogyan is kezdj neki:
honnan töltsd le az animéket, hogyan fordítsd le őket, hogyan és hol publikáld, és végül néhány kezdeti jótanács.
Fogok beszélni a fansuboknál betöltött különböző feladatkörökről, és hogy mire van esetükben szükség.


## Az út kezdete
{% assign sorted_posts = site.posts | sort: 'chapter' %}
<ol>
  {% for post in sorted_posts %}
	{% if post.categories contains "fansub_alapok" and post.tags contains "kezdetek" %}
		<li>
		  <a href="{{ post.url }}">{{ post.title }}</a>
		</li>
	{% endif %}
  {% endfor %}
</ol>


## Fansubolás csapatban
<ol>
  {% for post in sorted_posts %}
	{% if post.categories contains "fansub_alapok" and post.tags contains "csapat" %}
		<li>
		  <a href="{{ post.url }}">{{ post.title }}</a>
		</li>
	{% endif %}
  {% endfor %}
</ol>