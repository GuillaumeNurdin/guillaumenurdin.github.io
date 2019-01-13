---
layout: "single"
classes: wide
author_profile: "true"
feature_row:
  - image_path: "/assets/images/books.jpg"
    alt: "Mes recommandations de lecture"
    title: "Ma liste de lecture"
    excerpt: "Les livres inspirants"
    url: "/pages/books"
    btn_label: "Les livres"
    btn_class: "btn--inverse"
  - image_path: "/assets/images/Octocat.png"
    alt: "Mes repos favoris"
    title: "Mes repos favoris"
    excerpt: "Les repos à connaître"
    url: "/pages/repos"
    btn_label: "Les repos"
    btn_class: "btn--inverse"
  - image_path: "/assets/images/blog.jpg"
    alt: "Mes articles favoris"
    title: "Mes articles favoris"
    excerpt: "Les articles à lire"
    url: "/pages/articles"
    btn_label: "Les articles"
    btn_class: "btn--inverse"
    
---
Je partage ici les liens, repos, livres, etc. qui m'aident ou m'ont aidé à améliorer mes compétences de développeur.

<<<<<<< HEAD
***
{% for summary in site.summaries %}
### [{{summary.name}}]({{summary.goto}})
{% assign links_sum = site.links | where:"type", summary.type | where:"summary","true" %}
{% for link in links_sum %} 
* [{{link.name}}]({{link.link}})
{% endfor %}
[voir la suite]({{summary.goto}})

***
{% endfor %}
=======
---
{% include feature_row %}
>>>>>>> design and home page
