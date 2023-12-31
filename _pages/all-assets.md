---
layout: archive
title: "Assets"
permalink: /assets/all/
author_profile: true
header:
  overlay_image: /assets/images/home/oddworld_header.jpg
  caption: "Photo credit: [**Oddworld inhabitants**](http://www.oddworld.com/)"
---
[Materials](/assets/materials){: .btn .btn--primary .btn--small} [All assets](##){: .btn .btn--success .btn--small}
---
{: style="text-align: center;"}
---

{% for collection in site.collections %}
  {% for post in collection.docs %}
    {% unless collection.output == false or collection.label == "posts" %}
      {% include archive-single.html type=page.entries_layout %}
    {% endunless %}
  {% endfor %}
{% endfor %}