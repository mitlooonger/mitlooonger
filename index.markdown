---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: collection
---

<!-- {% if site.tags!="" %}
   {%include collecttags.html%}
{%endif%} -->


<body>
{% for row in site.data.data %}

{% if row.Media == "Image" %}
 <div class="grid__item_team">
      <a target="_blank" href="_images/archive/{{row.RelativePath}}">
        <img class ="img_tg" src="_images/archive/{{row.RelativePath}}" alt="_images/" width=300px>
      </a>
  <div class="desc">{{row.Title}}</div>
    <div class="pile">{{row.Pile}}</div>

</div>

{% elsif row.Media == "Link" %}
  <div class="gallery_link">
      <a target="_blank" href="_images/icons/link.png">
        <img class ="img_tg" src="_images/icons/link.png" alt="_images/" width=300px>
      </a>
  <div class="desc">{{row.Title}}</div>
  <div class="pile">{{row.Pile}}</div>

</div>
{% endif %} 
{% endfor %} 

<div class="section_end"> WE ARE DONE.</div>

<!--TEST linking images -- didnt work:( <body>
{% for row in site.data.data %}
  <div class="gallery">
  <a target="_blank" href="_images/archive/foldername/filename.ext">
    <img src="_images/archive/" 
    alt="_images/" width="600" height="400">
  </a>
  <div class="desc">"{{row.Title}}"</div>
    
  </div>
{% endfor %}


<div class="gallery">
  <a target="_blank" href="img_5terre.jpg">
    <img src="img_5terre.jpg" alt="Cinque Terre" width="600" height="400">
  </a>
  <div class="desc">Add a description of the image here</div>
</div>

<div class="gallery">
  <a target="_blank" href="img_forest.jpg">
    <img src="img_forest.jpg" alt="Forest" width="600" height="400">
  </a>
  <div class="desc">Add a description of the image here</div>
</div>

<div class="gallery">
  <a target="_blank" href="img_lights.jpg">
    <img src="img_lights.jpg" alt="Northern Lights" width="600" height="400">
  </a>
  <div class="desc">Add a description of the image here</div>
</div>

<div class="gallery">
  <a target="_blank" href="img_mountains.jpg">
    <img src="img_mountains.jpg" alt="Mountains" width="600" height="400">
  </a>
  <div class="desc">Add a description of the image here</div>
</div> -->

</body>
