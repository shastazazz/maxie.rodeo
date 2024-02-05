---
layout: default
---
# Publications
<!--- Text can be **bold**, _italic_, or ~~strikethrough~~.--->
* * *
<div class="list-1">
    <ul class="list-1">
    {%- for post in site.posts -%}
      <li>
        {%- if post.image -%}
          <img src="{{- post.image | relative_url -}}" alt=""
          >
        <!---{%- else -%}
          {%- assign postImage = "/assets/images/image-default.jpg" -%}
          <img src="{{- postImage | relative_url -}}" alt="" class="blog-roll-image">--->
        {%- endif -%}
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h3>
      </li>
      {%- endfor -%}
    </ul>
</div>
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