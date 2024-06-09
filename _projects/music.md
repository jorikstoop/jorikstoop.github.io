---
layout: page
title: Music
permalink: /projects/music
published: true
cover_img: /assets/img/music_cover.jpg
---

#### Current Song Recommendations

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


#### My Music
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

<!-- CSS for layout styling -->
<style>
  .song-rec-list {
    margin-bottom: 30px;
  }
  .song-list {
    margin-bottom: 15px;
  }
</style>