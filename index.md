---
layout: default
---
# Publications
<!--- Text can be **bold**, _italic_, or ~~strikethrough~~.--->
* * *
![Headline of "HOW TO CHANNEL CAR ANXIETY INTO FORWARD MOMENTUM" as seen in Lurch Zine.](../assets/img/forward_momentum_headline.png)

<ul>
  {% for post in site.posts %}
      <a href="{{ post.url }}">{{ post.title }}</a>
  {% endfor %}
</ul>

* * *
<!---
### Small image
![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)
### Large image
![Branching](https://guides.github.com/activities/hello-world/branching.png)
--->