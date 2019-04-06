{% assign links_filtered = site.links | where:"topic", page.topic %}
{% assign groupby = "type" %}
{% include links_collection_groupby.md %}
