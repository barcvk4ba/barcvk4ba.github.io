---
title: DMR Information
permalink: /articles/dmr/
toc: false
read_time: false
author_profile: false
#
# This page is designed to collect articles that are tagged as 'dmr'
# If you create an article in the _articles folder and add front matter of
#   tags: dmr
# it will appear in this page/list
#
---

Our Club entry into DMR started with a member presentation on all Digital Radio modes
and after some discussion we settled on DMR and in particular Retevis RT3S handheld
radios to make our way into this Network.

Our information on this page will be based on these radios specifically but most of
the information will still apply to other types of radios.

For club members to all be on the same level of operation we have provided a code
plug/config file to get started with and you will need your own radio id to make it go



## Retevis RT3s Club Plug


**Curent File:** [BARC_ver1.1.0.rdt](/assets/dmr/BARC_ver1.1.0.rdt)
<br/>
Please ensure you set your _**Radio ID**_, _**Radio Name**_, and customise your
_Intro Screen Lines_.
<br/>
<br/>
(We suggest you use your call sign in the intro lines so everyone can identify
who owns any random radio left floating around the club!)
{: .notice--info}



The BARC plug is based on seven local Sth East Qld repeaters with the usual talk
groups attached with some analogue 70cm/2m repeaters etc.

A long push of buttons above or below the PTT will change the repeater zone
and then twist of the top knob to tune into popular talk groups make it an easy
way to operate efficiently.

If updated we will change the version number so you know if you have the latest
version into the future.

Also should we in future publish other config versions they will be based on
other repeaters that we may wish to use inside Australia or Worldwide.

You are encouraged to modify and add to this file as your preferences lead you,
but then you own it and this one will remain should you ever need it again.

Enjoy your radio.

Les Neilson VK4LEZ, BARC President.

## A collection of articles related to DMR

{%
assign entries = site.articles
        | where_exp: "item", "item.tags contains 'dmr'"
        | sort: 'date'
        | reverse %}

{%- for post in entries -%}
  {%- unless post.hidden -%}
    {% include archive-single.html %}
  {%- endunless -%}
{%- endfor -%}
