---
layout: page
title: Projects
permalink: /projects/
---

#### My Music

Current Song Recommendations:

<ul class="song-rec-list">
    {% for song in site.data.song_recs %}
    <li>
    <div class="song-list">
        {{ song.name}}
        <span>{{ song.by }}</span>
    </div>
    </li>
    {% endfor %}
</ul>

I play the alto saxophone. Here are some song covers I made:

<ul class="cover-list">
    {% for cover in site.data.covers %}
    <li>
    <div class="song-list">
        {{ cover.name}}
        <span>{{ cover.artist }}</span>
        <span>
            {% if cover.link %}
            <a href= "{{ cover.link | relative_url }}" target="_blank" rel="noopener noreferrer">
              {{ cover.date }}
            </a>
            {% else %}
            <span>{{ cover.date }}</span>
            <audio controls>
              <source src="{{ cover.source | relative_url }}" type="audio/mpeg">
              Your browser does not support the audio element.
            </audio>
            {% endif %}
        </span>
    </div>
    </li>
    {% endfor %}
</ul>

#### My Photography

<!-- Create Rows of Fotos -->
  <section class="photography">
    <div class="photography-row">
      <div class="img-museum">
        <img src="/assets/img/1.jpg" alt="Civil Rights Museum ATL">
      </div>
      <div class="img-nyc">
        <img src="/assets/img/4.jpg" alt="NYC">
      </div>
    </div>    
    <div class="photography-row">
      <div class="img-boat">
        <img src="/assets/img/3.jpg" alt="Sailboat Lisbon">
      </div>
      <div class="img-trees">
        <img src="/assets/img/2.jpg" alt="ATL Botanical Garden">
      </div>
    </div>
  </section>


<!-- CSS for layout styling -->
<style>
  .song-list {
    margin-bottom: 15px;
  }

  .photography-row {
    display: flex;
    align-items: center;
    margin-bottom: 20px;
  }

  .img-boat {
    max-width: 64%;
  }
  .img-trees{
    max-width: 36%;
  }
</style>