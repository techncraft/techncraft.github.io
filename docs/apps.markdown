---
layout: default
title:  "Apps"
---

{% for collection in site.collections %}
  {% if collection.label == "apps_data" %}
  <h2>Privacy Policy of the Android Apps</h2>
  <p>View the Privacy Policy of the apps published on the Google Play.</p>
  <ul>
    {% for item in site[collection.label] %}
      <li><a href="{{ item.url }}">{{ item.title }}</a></li>
    {% endfor %}
  </ul>
  {% endif %}
{% endfor %}