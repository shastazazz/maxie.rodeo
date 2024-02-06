---
layout: default
---
<!---<div class="inline">
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
</ul>--->

<div class="w3-container">
  <h2>Tabs</h2>
  <p>Tabs are perfect for single page web applications, or for web pages capable of displaying different subjects. Click on the links below.</p>
</div>

<div class="tabtitles">
  <button onclick="opentabs('Publications')"><span>Publications</span></button>
  <button onclick="opentabs('Radio')"><span>Radio Files</span></button>
  <button onclick="opentabs('About')"><span>About Maxie</span></button>
</div>

<div id="Publications" class="tabs,postborder">
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
</div>

<div id="Radio" style="display:none" class="tabs,postborder">
  <ul class="list-1">
  {%- for post in site.radio -%}
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
</div>

<div id="About" style="display:none" class="tabs,postborder">
  <p>Tokyo is the capital of Japan.</p>
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