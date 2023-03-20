---
---

# Starter Pack - VII Semestre

[//]: # (Texto sobre el semestre opcional)

## Herramientas

{% for curso in site.data.starter-pack-tools.por-cursos.VII-semestre %}
### {{ curso.nombre }}

  {% for herramienta in curso.herramientas %}
    {%- if forloop.length > 0 -%}
        **{{ herramienta.nombre }}** <br>

        {%- if herramienta.enlace -%}
            <a href="{{ herramienta.enlace }}" target="_blank">
                {{ herramienta.enlace }}
            </a>
            <br>
        {%- endif -%}

        {%- if herramienta.descripcion -%}
            {{ herramienta.descripcion }} <br>
        {%- endif -%}

    {%- endif -%}
  {% endfor %}

{% endfor %}