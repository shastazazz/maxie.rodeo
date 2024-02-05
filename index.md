---
layout: default
---
# Publications
<!--- Text can be **bold**, _italic_, or ~~strikethrough~~.--->
* * *
![Headline of "HOW TO CHANNEL CAR ANXIETY INTO FORWARD MOMENTUM" as seen in Lurch Zine.](../assets/img/forward_momentum_headline.png)

<ul style="list-style-type:none;padding:0">
  {% for post in site.posts %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

* * *
<!---
### Small image
![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)
### Large image
![Branching](https://guides.github.com/activities/hello-world/branching.png)
--->