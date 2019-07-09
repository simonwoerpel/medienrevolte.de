---
title: Software
menu_title: software
---

i am experienced in building software for investigative journalists and other
data-related projects. here is a small list of interesting things:

{% if site.software %}
{% assign software = site.software | sort: 'ordering' %}

  <ul>
  {% for project in software %}
    <li>
    <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
    <p>{{ project.teaser }}</p>
    <p>developed for: <a href="{{ project.client.url }}">{{ project.client.name }}</a></p>
    <p>
    <a href="{{ project.url }}">> learn more</a>
    | repository: {% if project.repo %}<a href="{{ project.repo }}">{{ project.repo }}</a>{% else %}
      there is no public repo (yet) – maybe due to security or copyright concerns{% endif %}
    </p>
    </li>
  {% endfor %}
  </ul>
{% endif %}
