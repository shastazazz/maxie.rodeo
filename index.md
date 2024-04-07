---
layout: default
---
<div class="flex-container">
  <button class="index-nav-butts" onclick="opentabs('Publications')">Publications</button>
  <button class="index-nav-butts" onclick="opentabs('Stream')">Downstream</button>
  <button class="index-nav-butts" onclick="opentabs('About')">About</button>
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

<div id="Stream" style="display:none" class="tabs">
  <ul class="list-1">
  {%- for post in site.posts -%}
      {%- if post.categories contains 'Stream' -%}
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
                <p>&emsp;</p>
    <div>
<h1>
    About Maxwell Kline
</h1>
<div class="gifflex">
    <div>
        <video autoplay loop class="gifitem">
            <source src="/assets/video/super8unedited.gif" type="video/gif">
            <source src="/assets/video/super8unedited.mp4" type="video/mp4">
            Your browser does not support the video element.
        </video>
    </div>
    <div>
        <p>
            <i>(Above Super 8 video of Maxwell is courteous of multimedia artist <a href="http://instagram.com/_u/deb.is.sick/">Deb Seitz</a> [aka Deb Sicko]. All rights belong to Deb!)</i>
        </p>
    </div>
</div>
<p>
    Max was born in Gresham, but grew up in the foothills of Boise. They have tamed several packs of coyotes, and spent much time photosynthesizing with big sagebrush. They are currently raising a clutch of sage-grouse chicks in Portland, OR, as well as attending PSU (Portland State).
</p>
<p>
    Maxwell is a poet, multimedia artist, gardener, bad coder (re: this site), and more! Please forward all inquiries to my email, at the left of this page (or bottom, if you're on mobile).
</p>
<p>
    They have a piece forthcoming in <i><a href ="https://www.buckmanjournal.com/">Buckman Journal</a></i>, entitled "HAIL COLUMBIA!" Expect this piece sometime in July!
</p>
    </div>
                <p>&emsp;</p>
    <div>
<h1>
    About "maxie.rodeo"
</h1>
    <div>
<h3>MY OWN PRIVATE IDAHO</h3>
<p>
    The site's headline/return button reads: "MY OWN PRIVATE IDAHO". Yes, this is a reference to the Gus Van Sant film of the same name. (Shot entirely outside of Idaho, I might add.) I (Maxwell) no longer live in Idaho, and so this page is my little slice of old-home. It's a website on the internet, so it's both not really anywhere, and also everywhere. To me, the site is hosted in the mycorrhizae beneath the Arco desert. Or it's torrented from the Owyhees. Maybe it's frolicking naked in the Sawtooths. Regardless, I like to think of this site as my own private Idaho. 
</p>
    </div>
    <div>
<h3>Publications</h3>
<p>
    This tab is dedicated to a selection of publications I am particularly proud of and want to make available. It will update as new pieces are accepted and released into the wider world.
</p>
<p>
    Beneath each publication scan, I have listed rejection notices and their corresponding publications. This is a way of reclaiming the anxiety around rejections, and the submission process as a whole. Rejections are proof I've put myself out there, and that publications aren't always a one-and-done process.
</p>
    </div>
    <div>
<h3>Downstream</h3>
<p>
    I imagine this tab as an outflowing of rants, ravings, thoughts, and ideas. Some downstreams will be in-progress, and some will be complete. I plan on posting future collaborations, projects, and whatever else the future might hold. (But never NFTs, this site is anti-NFT!)
</p>
    </div>
    <div>
<h3>About</h3>
<p>
    This page was forked and adapted from the <a href="https://github.com/pages-themes/minimal">minimal</a> Jekyll theme for GitHub pages, by <a href="https://github.com/orderedlist">orderedlist</a>. The fonts used are <a href="https://fonts.google.com/specimen/Goblin+One?query=goblin+one">Goblin One</a>, by Riccardo De Franceschi, and <a href="https://fonts.google.com/specimen/Poltawski+Nowy">Półtawski Nowy</a>, by Adam Półtawski, Mateusz Machalski, Borys Kosmynka, and Ania Wieluńska. "maxie.rodeo" is being updated and managed by Maxwell Kline.
</p>
<p>
    All copyright belongs to Maxwell, unless I (Maxwell) state otherwise (or in a siuation where that statement is just outright untrue ;D ). Through the lens of derivatives, I am heavily considering the ethics of copyright. Expect changes on that front.
</p>
    </div>
    </div>
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