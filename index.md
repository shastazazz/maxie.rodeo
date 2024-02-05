---
layout: default
---
<div>
  <h1 class="postborder">
  Publications
  </h1>
</div>
<ul class="list-1">
  {%- for post in site.posts -%}
    <li>
      {%- if post.image -%}
        <!---<a href="{{ post.url | relative_url }}">--->
          <img src="{{- post.image | relative_url -}}" 
               alt="{{ post.imagealt }}" 
               width="790"
          >
        <!---</a>--->
      {%- endif -%}
        <h2 href="{{ post.url | relative_url }}" 
            class="postborder">
            {{ post.secrettitle }}
        </h2>
    </li>
  {%- endfor -%}
</ul>