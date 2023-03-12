---
---

# Starter Pack - I Semestre

Texto sobre el semestre opcional

[//]: # (Falta agregar una tabla de contenidos)

## Herramientas

{% for curso in site.data.starter-pack-tools.por-cursos.I-semestre %}

### {{ curso.nombre }}

  {% for herramienta in curso.herramientas %}

    {%- if forloop.length > 0 -%}
      {{ herramienta.nombre }} <br>
      <a href="{{ herramienta.enlace }}">
        {{ herramienta.enlace }}
      </a>
    {%- endif -%}
    <br>

  {% endfor %}

{% endfor %}

