---
layout: default
---
<div class="inline">
  <h1 class="postborder">
      Publications
  </h1>
  <h1 class="postborder">
      Radio Files
  </h1>
  <h1 class="postborder">
      About
  </h1>
</div>
<ul class="list-1">
  {%- for post in site.posts -%}
    <li>
      {%- if post.image -%}
        <a href="{{ post.url | relative_url }}">
          <img src="{{- post.image | relative_url -}}" 
               alt="{{ post.imagealt }}" 
               width="790"
          >
        </a>
      {%- endif -%}
        <a href="{{ post.url | relative_url }}">
            <h2 class="postborder hoverbold">
                {{ post.secrettitle }}
            </h2>
        </a>
    </li>
  {%- endfor -%}
</ul>