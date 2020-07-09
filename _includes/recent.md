{% assign latest_items = site.posts | concat: site.articles | concat: site.projects %}
{% assign latest_items = latest_items | sort: "date" | reverse %}

{% for p in latest_items limit:5 %}
* [{{ p.title }}]({{p.url}})
   {{p.excerpt}}
{% endfor %}

