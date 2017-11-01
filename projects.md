---
layout: page
title: Projetos
permalink: /projects/
---
<div>
    <img src="/assets/code_angular.gif" alt="angular gif">
</div>
<br>
{% for post in site.projects %}
<div class="li-project">
    <h2>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
    </h2>
    <p>
    {{ post.description }}
    </p>
    <div align="right">
    {% if post.link %}
        <a href="{{ post.link }}" target="_blank" >
            <i class="fa fa-link" aria-hidden="true"></i>
        </a>
        &emsp;
    {% endif %}
        <a href="{{ post.github }}" target="_blank" >
            <i class="fa fa-github" aria-hidden="true"></i>
        </a>
    </div>
</div>
{% endfor %}