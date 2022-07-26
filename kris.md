---
layout: default
---

<section>
  <h1>Kris</h1>
  <br/>
kris is my personal project
</section>

<section>


  {% for work in site.categories.kris %}
  <div class="media t-hackcss-media">
    
    <div class="media-left">
      {% if work.spotify-url %}
      <iframe src="https://open.spotify.com/embed/{{ work.spotify-url }}" width="250" height="80" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
      {% endif %}
      {% if work.youtube-url %}
      <iframe width="250" height="120" src="https://www.youtube-nocookie.com/embed/{{ work.youtube-url }}" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      {% endif %}

    </div>
    
    <div class="media-body">
      <div class="media-content">
        <h2 style="margin-top:0px;margin-bottom:0.2rem;">{{work.artist}} - {{work.title}}</h2>
        <i style="margin-top:0px;margin-bottom:0.2rem;">( {{ work.type }} &raquo; {{work.year}} )</i>
        <p style="margin-top:0px;margin-bottom:0.2rem;">{{work.roles}}</p>
      </div>
    </div>
    
    {% if forloop.last == false %}
      <hr/>
    {% endif %}
  </div>
  {% endfor %}
</section>
