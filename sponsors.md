---
layout: sponsors
---
<div id="sponsors-content">
    <!--{% assign sponsor-rows = 1 | plus: site.data.sponsors.silver.size | plus: site.data.sponsors.bronze.size | plus: site.data.sponsors.copper.size | divided_by: 3 | floor | plus: 1 | plus: site.data.sponsors.gold.size | divided_by: 3 | floor | plus: site.data.sponsors.diamond.size | times:  3 %}
    {% assign row = 1 %}
    {% assign col = 1 %}
    -->
    <style>
        .content {
            margin: 2px;
        }
        .sponsors {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            grid-template-rows: repeat({{sponsor-rows}}, 1fr);
            grid-column-gap: 10px;
            grid-row-gap: 10px;
        }
        h1 {
            text-align: center;
        }
    </style>
    <div class="content">
        <h1><u>Sponsors</u></h1>
        <div class="sponsors">
            {% include uofsc/sponsor.html %}
        </div>
        <h1><u>Grants</u></h1>
        <br>
        <br>
        {% for grant in site.data.sponsors.grants %}
            {% include uofsc/grant.html grant=grant %}
        {% endfor %}
    </div>
</div>