{% for link in links %}
     {% if link.picture %}
![{{link.name}}]({{link.picture}}){: .align-left} {% endif %}
<i class="{{site.data.types[link.type].fa}}" aria-hidden="true"></i>
[**{{link.name}}**]({{link.link}}) *{{link.author}}*
<br/> 
{{link.content | remove: '<p>' | remove: '</p>' }}{: .notice--primary}
{% for top in link.topic%}<a href="/topics/{{ top | slugify }}" class="btn btn btn--small"><i class="fas fa-tags"></i> {{top}}</a>
{% endfor %}
---
{% endfor %}