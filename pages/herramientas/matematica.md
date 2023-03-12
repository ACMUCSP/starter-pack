---
title: De uso general
sitemap: true
---

# Starter Pack - Área de matemáticas
## Herramientas
{% for curso in site.data.starter-pack-tools.matematicas %}

### {{ curso.nombre }}

  {% for herramienta in curso.herramientas %}

    {%- if forloop.length > 0 -%}
        **{{ herramienta.nombre }}** <br>
        <a href="{{ herramienta.enlace }}">{{ herramienta.enlace }}</a><br>
        {%- if herramienta.extra -%}
        {{ herramienta.extra }} <br>
        {%- endif -%}

    {%- endif -%}

  {% endfor %}

{% endfor %}