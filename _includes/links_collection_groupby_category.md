{% assign links_filtered = site.links | where:"type", page.type %}
{% assign groupby = "category" %}
{% include links_collection_groupby.md %}