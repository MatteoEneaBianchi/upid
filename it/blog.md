---
layout: page
title: Blog
lang: it
ref: 
permalink: /blog/
order: 2
img: https://www.dopara.it/cdn/shop/articles/come-conservare-libri-usati-consigli.jpg?v=1636232915
---



<div class="row">
  {% for post in site.posts %}
    <div class="col-12 col-lg-8">
      <!--start card-->
      <div class="card-wrapper card-space">
        <div class="card card-bg card-big">
          <div class="card-body">
            <div class="top-icon">
              <svg class="icon"><use href="/assets/bootstrap-italia/dist/svg/sprite.svg#it-card"></use></svg>
            </div>
            <h3 class="card-title h5">
              <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
            </h3>
            <p class="card-text font-serif">
              {{ post.excerpt | strip_html | truncatewords: 20 }}
            </p>
            <a class="read-more" href="{{ post.url | relative_url }}">
              <span class="text">Leggi di più</span>
              <span class="visually-hidden">su {{ post.title }}</span>
              <svg class="icon"><use href="/bootstrap-italia/dist/svg/sprites.svg#it-arrow-right"></use></svg>
            </a>
          </div>
        </div>
      </div>
      <!--end card-->
    </div>
  {% endfor %}
</div>
