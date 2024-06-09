---
layout: page
title: My Photography
permalink: /projects/photography
published: true
cover_img: /assets/img/foto_cover.png
---


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
      <div class="photography-row">
      <div class="img-aqua">
        <img src="/assets/img/5.jpg" alt="Georgia Aquarium">
      </div>
      <div class="img-lake">
        <img src="/assets/img/6.jpg" alt="Lake Lanier">
      </div>
    </div> 
  </section>



<!-- CSS for Style -->
<style>
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