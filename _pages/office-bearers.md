---
title: Office Bearers
permalink: /docs/office-bearers/

# We will define the list of roles and office bearers in
# the _data/office-bearers.yml file so that we can build
# a nice layout below.
#
# it will be available in site.data.officebearers

---

## Office Bearers {{ site.data.officebearers.year }}

<table>
    <thead>
        <tr class="header">
            <th>Office</th>
            <th>Bearer</th>
        </tr>
    </thead>
    <tbody>
        {%- for o in site.data.officebearers.offices -%}
        <tr>
            <td><strong>{{ o.office }}</strong></td>
            <td>
                {%- if o.bearer -%}
                    {{ o.bearer }} {%- if o.callsign -%}&nbsp;<small>{{ o.callsign }}</small>{%- endif -%}
                {%- else -%}
                    <small>Vacant</small>
                {%- endif -%}
            </td>
        </tr>
        {%- endfor -%}
    </tbody>
</table>

## Notes
Committee positions are elected at the Annual General Meeting which is held in May of each year.

