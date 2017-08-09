---
layout: page
title: Sobre
permalink: /about/
---

O Grupo de Estudos em Machine Learning do IME-USP é um grupo de pesquisadores dedicado a (Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in...)

<h3>Professores Coordenadores</h3>
{% for teacher in site.members %}
{% if teacher.kind == "teacher" %}

<p> {{teacher.name}} </p>
<p> {{teacher.occupation}} em {{teacher.place}} </p>

{% endif %}
{% endfor %}


<h3>Alunos</h3>
{% for student in site.members %}
{% if student.kind == "aluno" %}

<p> {{student.name}} </p>
<p> {{student.occupation}} em {{student.place}} </p>

{% endif %}
{% endfor %}


