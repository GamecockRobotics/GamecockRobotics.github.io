---
layout: home
---
<div id="sponsors-content">
    {% assign sponsor-rows = 1 | plus: site.data.sponsors.silver.size | plus: site.data.sponsors.bronze.size | plus: site.data.sponsors.copper.size | divided_by: 3 | floor | plus: 1 | plus: site.data.sponsors.gold.size | divided_by: 3 | floor | plus: site.data.sponsors.diamond.size | times:  3 %}
    {% assign row = 1 %}
    {% assign col = 1 %}
    <style>
        .content {
            margin: 10px;
        }
        .sponsors {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            grid-template-rows: repeat({{sponsor-rows}}, 1fr);
            grid-column-gap: 10px;
            grid-row-gap: 10px;
        }
    </style>
    <div class="content">
        <h1>Sponsors</h1>
        <div class="sponsors">
            {% for sponsor in site.data.sponsors.diamond %}
                {% include uofsc/sponsor.html sponsor=sponsor tier="diamond" %}
                {% assign row = row | plus: 3 %}
            {% endfor %}
            {% for sponsor in site.data.sponsors.gold %}
                {% include uofsc/sponsor.html sponsor=sponsor tier="gold" %}
                {% assign col = col | plus: 1 %}
                {% if col == 4 %}
                    {% assign col = 1 %}
                    {% assign row = row | plus: 3 %}
                {% endif %}
            {% endfor %}
            {% for sponsor in site.data.sponsors.silver %}
                {% include uofsc/sponsor.html sponsor=sponsor tier="silver" %}
            {% endfor %}
            {% for sponsor in site.data.sponsors.bronze %}
                {% include uofsc/sponsor.html sponsor=sponsor tier="bronze" %}
            {% endfor %}
            {% for sponsor in site.data.sponsors.copper %}
                {% include uofsc/sponsor.html sponsor=sponsor tier="copper" %}
            {% endfor %}
        </div>
        <h1>Grants</h1>
        {% for grant in site.data.sponsors.grants %}
            {% include uofsc/grant.html grant=grant %}
        {% endfor %}
    </div>
</div>