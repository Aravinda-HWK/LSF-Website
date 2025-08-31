---
layout: page
title: Board of Directors
permalink: /about/directors/
---
<table>
    {% for director in site.data.directors %}
        {% assign person = director[1] %}
        <tr>
            <td width="20%" style="vertical-align: top;">
                <img src="{{ site.baseurl }}/{{ person.image }} " width="100%">
            </td>
            <td>
                <p>
                    Name: <b> {{ person.name }} </b><br>
                    Start Date: <b>{{ person.start_date }}</b><br>
                    {{ person.shortbio | markdownify }}
                    More: 
                    <a href="{{ person.moreinfo }}"> {{ person.moreinfo}} </a>
                </p>                
            </td>
        </tr>
    {% endfor %}
</table>
