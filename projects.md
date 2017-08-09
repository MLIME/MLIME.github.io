---
layout: page
title: Projetos
permalink: /projects/
---

<p>Lista de projetos realizados pelo grupo:</p>

{% for project in site.projects %}
<h3> {{project.title}}  </h3>
<p>  {{project.content}} </p>
Veja <a href=" {{project.link}}">mais</a>

{% endfor %}




