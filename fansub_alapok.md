---
layout: page
title: "Fansub alapok kezdőknek"
permalink: /fansub_alapok
---
Szóval animéket szeretnél fordítani? Hát rendben.
Akkor a legjobb helyre jöttél: eme rövid cikksorozatban összefoglalom, hogyan is kezdj neki:
honnan töltsd le az animéket, hogyan fordítsd le őket, hogyan és hol publikáld, és végül néhány kezdeti jótanács.
Fogok beszélni a fansuboknál betöltött különböző feladatkörökről, és hogy mire van esetükben szükség.

<ul>
  {% for post in site.posts reversed %}
	{% if post.categories contains "fansub_alapok" %}
		<li>
		  <a href="{{ post.url }}">{{ post.title }}</a>
		</li>
	{% endif %}
  {% endfor %}
</ul>
