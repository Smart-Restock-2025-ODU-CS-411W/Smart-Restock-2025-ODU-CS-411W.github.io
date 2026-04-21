---
layout: page
title: Documents
permalink: /documents/
---

<ul class="doc-list">
  {% for doc in site.data.documents %}
    <li>
        <a href="{{ doc.link | relative_url }}" target="_blank">
          {% if doc.type == "external" %}🔗{% else %}📄{% endif %}
          {{ doc.title }}
        </a>
    </li>
  {% endfor %}
</ul>