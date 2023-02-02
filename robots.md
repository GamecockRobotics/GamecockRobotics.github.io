---
layout: home
title: "Retired Bots"
---
<div class="retired-robots">
    {% include structure/gallery-script.html %}
    {% include structure/ytapi.html %}
    {% for robot in site.data.robots reversed %}
        {% include uofsc/robot-display.html robot=robot %}
        {% unless forloop.last %}
        <div style="height: 1px;background-color:{{site.data.theme.neutral1}};margin-top:20px;"></div>
        {% endunless %}
    {% endfor %}
</div>