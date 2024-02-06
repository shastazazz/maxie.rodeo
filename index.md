---
layout: default
---
<div class="tabtitles">
  <button class="hoverbold" onclick="opentabs('Publications')"><span>Publications</span></button>
  <button class="hoverbold" onclick="opentabs('Radio')"><span>Radio Files</span></button>
  <button class="hoverbold" onclick="opentabs('About')"><span>About Maxie</span></button>
</div>

<div id="Publications" class="tabs">
  <ul class="list-1">
  {%- for post in site.posts -%}
      {%- if post.categories contains 'Publications' -%}
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
      {%- endif -%}
  {%- endfor -%}
  </ul>
</div>

<div id="Radio" style="display:none" class="tabs">
  <ul class="list-1">
  {%- for post in site.posts -%}
      {%- if post.categories contains 'Radio' -%}
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
      {%- endif -%}    
  {%- endfor -%}
  </ul> 
</div>

<div id="About" style="display:none" class="tabs">
Maxwell was born in Gresham, (OR,) raised in Boise, (ID,) and now lives in Portland, Oregon.
    
They are a poet, multimedia artist, gardener, and so much more.
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