
{% assign links_grouped = site.links | where:"type", page.type | group_by: 'category' %}
{% for group in links_grouped %}
## {{group.name}}
    {% for link in group.items %}
        {% if link.picture %}
![{{link.name}}]({{link.picture}}){: .align-left} {% endif %}
{% for top in link.topic%}
<span><i class="fas fa-tags"></i>{{top}}</span>{% endfor %}<br/>[**{{link.name}}**]({{link.link}}) *{{link.author}}*
<br/> 
{{link.content | remove: '<p>' | remove: '</p>' }}{: .notice--primary}
    {% endfor %}
{% endfor %}