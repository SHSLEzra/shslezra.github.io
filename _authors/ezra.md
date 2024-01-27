---
layout: page
name: Ezra
---

{% assign ezra-about = site.pages | where: "path", "bemutatkozas.md" | first %}
{{ ezra-about.content }}