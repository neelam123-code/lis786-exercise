---
title: Home
layout: default
---
<p>Browse the cuisine below:</p>

{% for indian_cuisine in site.indian_cuisine %}
<div class="cuisine-teaser clearfix">
<div class="img-left teaser-image">
<a href="{{ indian_cuisine.url}}" alt="go to the detail page"><img src="{{indian_cuisine.image }}" alt="photo>
</div>
<div class="teaser-content">
<h2><a href="{{ indain_cuisine.url }}" alt=" go to the detail page">{{ indian_cuisine.title }}</a></h2>
    <p>{{ indian_cuisine.content | truncatewords:20, '...' }}</p>
<p><small>weight category: <em>{{ indian_cuisine.category }}</em></small></p>
<p><a href="{{ indian_cuisine.source }}" target=" _blank">Source</a></p>
    </div>
    </div>
    {% endfor %}
