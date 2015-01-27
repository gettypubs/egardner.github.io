---
title: Publications
layout: default
permalink: /survey/
---
<table class="survey" style="width:100%">
  <tr>
    <th class="row-title" colspan="3">Title</th>
    <th colspan="2">Institution</th> 
    <th>Type</th>
    <th>Format</th>
    <th>Price</th>
  </tr>
  {% assign sorted_data = site.data.survey | sort:"institution" %}
  {% for item in sorted_data %}
  <tr>
    <td class="row-title" colspan="3"><a href="{{item.purchase_url}}">{{item.title}}</a></td>
    <td colspan="2"><a href="{{item.publisher_url}}">{{item.institution}}</a></td> 
    <td>{{item.type}}</td>
    <td>{{item.format}}</td>
    <td>{{item.price}}</td>
  </tr>
  {% endfor %}
</table>