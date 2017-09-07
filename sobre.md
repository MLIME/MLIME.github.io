---
layout: page
title: Sobre
permalink: /about/
---
<style>
    .memberlist{
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: space-evenly
    }

    .member{
        text-align: center;
        width: 30%;
        margin-left: 2.5%;
        margin-right: 2.5%;
    }

    .memberimage{
        width: 140px;
        height: 140px;
        margin-bottom: 5%;
        border-radius: 50%;
    }

</style>

{{ site.description}}

<h3>Teachers</h3>
<div class="memberlist">
{% for teacher in site.members %}
{% if teacher.kind == "teacher" %}

<div class="member">
{% if teacher.image %}
    <img class="memberimage" src="{{site.baseurl}}images/{{teacher.image}}">
{% else %}
    <img class="memberimage" src="{{site.baseurl}}images/noimage.png">
{% endif %}
<p style="margin-bottom: 0"> {{teacher.name}} </p>
<p> {{teacher.interests}} </p> 
</div>
{% endif %}
{% endfor %}
</div>


<h3>Students</h3>
<div class="memberlist">
{% for student in site.members %}
{% if student.kind == "aluno" %}
<div class="member">
{% if student.image %}
    <img class="memberimage" src="{{site.baseurl}}images/{{student.image}}">
{% else %}
    <img class="memberimage" src="{{site.baseurl}}images/noimage.png">
{% endif %}
<p style="margin-bottom: 0"> {{student.name}} </p>
<p> {{student.interests}} </p>
</div>

{% endif %}
{% endfor %}
</div>


