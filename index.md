---
layout: default
---
# Publications
<!--- Text can be **bold**, _italic_, or ~~strikethrough~~.--->
* * *
<ul style="list-style-type:none;padding:0">
  {% for post in site.posts %}
      <li><a href="{{ post.url }}">{{ post.secrettitle }}</a></li>
                {% if post.secrettitle %}
                    <ul style="list-style-type:none;padding:0">
                        <li></li>
                        <li><a href="{{ post.url }}">{{ post.secrettitle }}</a></li>
                    </ul>   
                {% endif %}    
  {% endfor %}
</ul>

{%- for post in site.posts -%}
<div>
  <h2>{{ post.title }}</h2>
  {% assign photo_path = '/img/large/' | append: post.photo %}
  <img src="{{ photo_path | relative_url }}" />
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