---
title: Home
layout: default
---
Browse the cuisine below:

{% for indian_cuisine in site.indian_cuisine %}
    <h2>{{ indian_cuisine.title }}</h2>
    <p>{{ indian_cuisine.content }}</p>
    <a href="{{ indian_cuisine.source }}" target=" _blank">Source</a>
    {% endfor %}
