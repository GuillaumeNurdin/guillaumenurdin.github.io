{% assign links_grouped = links_filtered | sort : date | group_by: groupby   %}
{% for group in links_grouped %}
    {% assign links = group.items%}
    {% if site.data.types[group.name].label == nil %}
### {{group.name}}
 {% else %}
### {{site.data.types[group.name].label}}
{% endif%}
    {% include links_loop.md %}
{% endfor %}