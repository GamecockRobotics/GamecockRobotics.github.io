---
layout: home
---
<div id="team-page-content">
    {% for profile in site.data.members %}
        {% include adapter/profile.html member=profile %}
    {% endfor %}
</div>