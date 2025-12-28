---
title: POTA Information
permalink: /pota/
toc: true
read_time: false
author_profile: false
#
# This page is designed to collect articles that are tagged as 'pota'
# If you create an article in the _articles folder and add front matter of
#   tags: pota
# it will appear in this page/list
#
---
## POTA Information

A collection of cheat sheets, technical guides and practical tips for POTA and activations.

**POTA Brochure:** [POTA Brochure - AU.pdf](/assets/pota/POTA Brochure - AU.pdf)
{: .notice--info}

**Amateur Radio in the Park - Handout:** [Amateur Radio in the Park - Handout.pdf](/assets/pota/Amateur Radio in the Park - Handout.pdf)
{: .notice--info}
**Parks on the Air Voice (SSB) Call & Response Cheat Sheet:** [Parks on the Air Voice (SSB) Call & Response Cheat Sheet.pdf](/assets/pota/Parks on the Air Voice (SSB) Call & Response Cheat Sheet.pdf)
{: .notice--info}
**POTA Explainer handout:** [POTA Explainer handout.pdf](/assets/pota/POTA Explainer handout.pdf)
{: .notice--info}
**POTA CW Cheat Sheet:** [POTA CW Cheat Sheet.pdf](/assets/pota/CW POTA Cheat Sheet.pdf)
{: .notice--info}

## POTA Articles

{%
assign entries = site.articles
        | where_exp: "item", "item.tags contains 'pota'"
        | sort: 'date'
        | reverse %}

{%- for post in entries -%}
  {%- unless post.hidden -%}
    {% include archive-single.html %}
  {%- endunless -%}
{%- endfor -%}