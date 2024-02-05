---
layout: default
---
# Publications
* * *
<ul class="list-1">
  {%- for post in site.posts -%}
    <li>
      {%- if post.image -%}
        <a href="{{ post.url | relative_url }}">
          <img src="{{- post.image | relative_url -}}" alt="{{ post.imagealt }}">
        </a>
      {%- endif -%}
        <h2>{{ post.secrettitle }}</h2>
    </li>
  {%- endfor -%}
</ul>
* * *



    
    
<!---
{%- for post in site.posts -%}
<div>
  {% assign image_path = '/assets/img/' | append: post.image %}
  <img src="{{ image_path | relative_url }}" />
  <h2>{{ post.title }}</h2>
  <a href="{{ post.url }}">{{ post.secrettitle }}</a>
</div>
{% endfor %}
--->
