---
layout: page
title: Sobre
permalink: /about/
---

{{ site.description}}

<h3>Professores Coordenadores</h3>
{% for teacher in site.members %}
{% if teacher.kind == "teacher" %}

<p style="margin-bottom: 0"> {{teacher.name}} </p>
<p> {{teacher.occupation}} em {{teacher.place}} </p>

{% endif %}
{% endfor %}


<h3>Alunos</h3>
{% for student in site.members %}
{% if student.kind == "aluno" %}

<p style="margin-bottom: 0"> {{student.name}} </p>
<p> {{student.occupation}} em {{student.place}} </p>

{% endif %}
{% endfor %}


