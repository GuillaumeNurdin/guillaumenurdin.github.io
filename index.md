---
layout: home
---
Je partage ici les liens, repos, livres, etc. qui m'aident ou m'ont aidé à améliorer mes compétences de développeur.

***
{% for summary in site.summaries %}
### [{{summary.name}}]({{summary.goto}})
{% assign links_sum = site.links | where:"type", summary.type | where:"summary","true" %}
{% for link in links_sum %} 
* [{{link.name}}]({{link.url}})
{% endfor %}
[voir la suite]({{summary.goto}})

***
{% endfor %}
