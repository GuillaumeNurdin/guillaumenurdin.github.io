{% assign links_filtered = site.links | where:"topic", page.topic %}
{% assign groupby = "type" %}
{% include links_collection_groupby.md %}


{% assign psize = site.tags[page.topic] | size %}
{% if psize != 0 %} 
# Mes articles sur ce sujet
  {%- for post in site.tags[page.topic] -%}
  {% include archive-single.html %}
{%- endfor -%}
{% endif %}

