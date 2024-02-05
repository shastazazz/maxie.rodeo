---
layout: default
---
# Publications
* * *
<ul class="list-1">
  {%- for post in site.posts -%}
    <li>
      {%- if post.image -%}
        <a href="{{ post.url | relative_url }}" class="imageborder">
          <img src="{{- post.image | relative_url -}}" alt="{{ post.imagealt }}">
        </a>
      {%- endif -%}
        <h2>{{ post.secrettitle }}</h2>
    </li>
  {%- endfor -%}
</ul>
* * *