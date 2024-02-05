---
layout: default
---
# Publications
<!--- Text can be **bold**, _italic_, or ~~strikethrough~~.--->
* * *

{%- for post in site.posts -%}

<div>
  {% assign photo_path = '/img/large/' | append: post.photo %}
  <img src="{{ photo_path | relative_url }}" />
  <h2>{{ post.title }}</h2>
  <a href="{{ post.url }}">{{ post.secrettitle }}</a>
</div>

{% endfor %}

* * *
<!---The above section is an example of how posts should look on the front page!--->
<!---
### Small image
![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)
### Large image
![Branching](https://guides.github.com/activities/hello-world/branching.png)
--->