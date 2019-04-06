{% assign links_grouped = links_filtered | sort : date | group_by: 'category'   %}
{% for group in links_grouped %}
    {% assign links = group.items%}
### {{group.name}}
    {% include links_loop.md %}
{% endfor %}