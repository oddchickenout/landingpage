---
permalink: /
hidden: true
author_profile: false
title: "home"
layout: single

---

TikTok @oddchickout

Instagram @oddchickenout

Twitter @oddchickenout



{% if site.data.social-media %}
<div id="social-media">
    {% assign sm = site.data.social-media %}
    {% for entry in sm %}
        {% assign key = entry | first %}
        {% if sm[key].id %}
            <a href="{{ sm[key].href }}{{ sm[key].id }}" title="{{ sm[key].title }}"><i class="fa {{ sm[key].fa-icon }}"></i></a>
        {% endif %}
    {% endfor %}
</div>
{% endif %}


