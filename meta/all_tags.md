---
layout: page
title:  All Tags
---

{% capture alltags %}
  {% for p in site.pages %}
    {% for t in p.tags %}
      {{ t }}
    {% endfor %}
  {% endfor %}
{% endcapture %}

{% assign xtags = alltags | split:" " | uniq %}

{% for t in xtags %}
- {{ t }}
{% endfor %}

---

{% for t in xtags %}
## {{ t }}

{% for p in site.pages %}
{% if p.tags contains t %}

- [{{ p.title }}]({{ p.url }})

{% endif %}
{% endfor %}

{% endfor %}
