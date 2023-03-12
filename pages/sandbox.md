---
title: Sandbox
sitemap: true
---

{% for item in site.data.starter-pack-tools.uso-general %}

{{ item.nombre }} <br>
<a href="{{ item.enlace }}">
  {{ item.enlace }}
</a>


{% endfor %}


<h2>Ejemplo de 1 semestre</h2>

# Starter Pack - I Semestre
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

