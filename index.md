---
layout: default
---
# Publications
<!--- Text can be **bold**, _italic_, or ~~strikethrough~~.--->
* * *

{%- for post in site.posts -%}

<div>
  {% assign image_path = '/assets/img/' | append: post.image %}
  <img src="{{ image_path | relative_url }}" />
  <h2>{{ post.title }}</h2>
  <a href="{{ post.url }}">{{ post.secrettitle }}</a>
</div>

{% endfor %}

* * *
<!---The above section is an example of how posts should look on the front page!--->