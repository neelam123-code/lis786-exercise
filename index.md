---
title: Home
layout: default
---
<p>Browse the cuisine below:</p>

<div class="card card-nav-tabs card-plain">
<div class="card-header card-header-primary">
<!-- colors: "header-primary", "header info", "header-success", "header-warning", "header-danger" -->
<div class="nav-tabs-navigation">
<div class="nav-tabs-wrapper">
<ul class="nav nav-tabs" data-tabs="tabs">
<li class="nav-item">
<a class="nav-link active show" href="#alpha" data-toggle="tab">Sort alphabetically<div class="ripple-container"></div></a>
    </li>
    <li class="nav-item">
 <a class="nav-link" href="#weight" data-toggle="tab">Sort by weight<div class="ripple-container"></div></a>
 </li>
    </ul>
    </div>
    </div>
    </div>
    <div class="card-body ">
        <div class="tab-content">
        <div class="tab-pane active show" id="alpha">
{% for indian_cuisine in site.indian_cuisine %}
<div class="cuisine-teaser clearfix">
<div class="img-left teaser-image">
<a href="{{ indian_cuisine.url}}" alt="go to the detail page"><img src="{{indian_cuisine.image }}" alt="photo>
</div>
<div class="teaser-content">
<h2><a href="{{ indain_cuisine.url }}" alt=" go to the detail page">{{ indian_cuisine.title }}</a></h2>
    <p>{{ indian_cuisine.content | truncatewords:44, '...' }}</p>
<p><small>weight category: <em>{{ indian_cuisine.category }}</em></small></p>
<p><a href="{{ indian_cuisine.source }}" target=" _blank">Source</a></p>
</div>
<div class="tab-pane" id="weight">
<p>Coming soon.</p>
</div>
</div>
<div>
</div>