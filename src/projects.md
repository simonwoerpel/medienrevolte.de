---
title: Projects
menu_title: projects
---

**`>>>>` [check out my publications on
correctiv.org](https://correctiv.org/correctiv/redaktion/team/simon-woerpel/)
`<<<<`**

we @ correctiv.org love to share our data & code with others. [this are some
github-repos with data
visualizations](https://github.com/correctiv?utf8=%E2%9C%93&q=viz&type=&language=)

If you want to see how we wrangle data here are some [jupyter
notebooks](https://github.com/correctiv?utf8=%E2%9C%93&q=notebook&type=&language=).

{% if site.projects %}
{% assign projects = site.projects | sort: 'ordering' %}

## Here are a few in-depth descriptions about projects I worked on:

  <ul>
  {% for project in projects %}
    <li>
    <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
    <p>{{ project.teaser }}</p>
    <p>
    <a href="{{ project.url }}">> learn more</a>
      {% if project.external_url %} | visit: <a href="{{ project.external_url }}">{{ project.external_url }}</a>{% endif %}
    </p>
    </li>
  {% endfor %}
  </ul>
{% endif %}

### and here is some legacy stuff:

- [Simple Open Data Portal](https://essen.openruhr.de/) – the city of "Essen" publishes some open data sets but not in a proper way. we from the [OK Lab Ruhrgebiet](https://codefor.de/ruhrgebiet/) fixed that. --> [github](https://github.com/CodeforRuhrgebiet/offenes-datenportal)
- [conflicts of interests resolver](https://coi.medienrevolte.de/) – making possible conflicts of interests in open access papers searchable. this was done during a [gen hackathon](https://www.globaleditorsnetwork.org/programmes/editors-lab/sz-editors-lab/)
- [datenwende.org](http://datenwende.org/) – some attempts to map the german renewable energy market as part of a fellowship from the [Vocer Medialab](http://www.vocer.org/medialab/)
- [bruecken.medienrevolte.de](https://bruecken.medienrevolte.de) – see train bridges in germany from birds eye view
