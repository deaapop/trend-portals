---
layout: default
title: Tren Terkini Indonesia
description: Ringkasan orisinal hasil lokalisasi AI tentang topik yang sedang ramai di Indonesia. Sumber selalu dicantumkan.
lang: id
permalink: /articles/id/
---

<div class="hero">
  <h1>Tren Terkini Indonesia</h1>
  <p>Ringkasan orisinal hasil lokalisasi AI tentang topik yang sedang ramai dibicarakan, selalu disertai tautan ke sumber aslinya.</p>
</div>

## Artikel terbaru

{% assign portal_posts = site.posts | where: "lang", "id" %}
{% if portal_posts.size > 0 %}
<ul class="post-list">
{% for post in portal_posts %}
  <li>
    <span class="post-meta">{{ post.date | date: "%d/%m/%Y" }}</span>
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p>{{ post.description }}</p>
  </li>
{% endfor %}
</ul>
{% else %}
<div class="empty-state">
  <p>Belum ada artikel yang diterbitkan. Silakan kembali lagi nanti!</p>
</div>
{% endif %}

<div class="how-it-works">
  <h2>Cara kerjanya</h2>
  <p>Kami memantau sinyal tren publik (hanya judul topik, tidak pernah menyalin teks sumber). AI menulis ringkasan orisinal dalam Bahasa Indonesia, dan seseorang meninjau setiap artikel sebelum diterbitkan. Sumber asli selalu dicantumkan di akhir tulisan.</p>
  <p><em>Beberapa artikel mungkin memuat tautan afiliasi, yang selalu diberi keterangan pengungkapan.</em></p>
</div>

<p><a href="{{ '/' | relative_url }}">← Trend Portals</a> · <a href="{{ '/articles/pt-br/' | relative_url }}" hreflang="pt-BR" lang="pt-BR">Português (Brasil)</a></p>
