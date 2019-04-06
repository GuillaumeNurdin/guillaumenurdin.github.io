{% assign links_filtered = site.links | where:"type", page.type %}
{% include links_collection_simple.md %}