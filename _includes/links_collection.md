
{% assign links_grouped = site.links | where:"type", page.type | group_by: 'category' %}
{% for group in links_grouped %}
    {% assign links = group.items%}
## {{group.name}}
    {% include links_loop.md %}
{% endfor %}