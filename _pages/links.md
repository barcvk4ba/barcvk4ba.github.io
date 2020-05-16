---
title: Links
permalink: /docs/links/
toc: true
#
# The list of links is sourced from the _data/links.yml file.
#
---

{% for section in site.data.links %}
### {{ section.name }}

{{ section.description }}

  {% for link in section.links %}
* [{{ link.title }}]({{ link.url }}){:target="_blank"} {{ link.detail }}
  {% endfor %}
{% endfor %}
