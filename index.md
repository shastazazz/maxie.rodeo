---
layout: default
---
<div class="flex-container">
  <button class="index-nav-butts" onclick="opentabs('Publications')">Publications</button>
  <button class="index-nav-butts" onclick="opentabs('Radio')">Radio Files</button>
  <button class="index-nav-butts" onclick="opentabs('About')">About Maxie</button>
</div>

<div id="Publications" class="tabs">
  <ul class="list-1">
  {%- for post in site.posts -%}
      {%- if post.categories contains 'Publications' -%}
        <li>
          {%- if post.imagehead -%}
            <a href="{{ post.url | relative_url }}">
              <img src="{{- post.imagehead | relative_url -}}" 
                   alt="{{ post.headalt }}" 
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
      {%- endif -%}
  {%- endfor -%}
  </ul>
</div>

<div id="Radio" style="display:none" class="tabs">
Check back later ;D !
  <ul class="list-1">
  {%- for post in site.posts -%}
      {%- if post.categories contains 'Radio' -%}
        <li>
          {%- if post.imagehead -%}
            <a href="{{ post.url | relative_url }}">
              <img src="{{- post.imagehead | relative_url -}}" 
                   alt="{{ post.headalt }}" 
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
      {%- endif -%}    
  {%- endfor -%}
  </ul> 
</div>

<div id="About" style="display:none" class="tabs">

Max was born in Gresham, but grew up in the foothills of Boise. They have tamed several packs of coyotes, and spent much time photosynthesizing with big sagebrush. They are currently raising a clutch of sage-grouse chicks in Portland, OR, as well as attending PSU (Portland State).


Maxwell is a poet, multimedia artist, gardener, and more.

## ABOUT MAXIE.RODEO

Beneath each publication scan, I have listed rejection notices and their corresponding publications.This is a way of reclaiming the anxiety around rejections, and the submission process as a whole. I'm _bragging_ about these rejections. They're proof I've put myself out there, and that publications aren't always a one-and-done process.


This page was forked and adapted from the <a href="https://github.com/pages-themes/minimal">minimal</a> Jekyll theme for GitHub pages, by <a href="https://github.com/orderedlist">orderedlist</a>. It is being updated and managed by Maxwell Kline.

</div>

<script>
function opentabs(tabsname) {
  var i;
  var x = document.getElementsByClassName("tabs");
  for (i = 0; i < x.length; i++) {
    x[i].style.display = "none";  
  }
  document.getElementById(tabsname).style.display = "block";  
}
</script>