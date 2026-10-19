---
layout: default
title: Tendências do Brasil
description: Resumos originais, localizados com apoio de IA, sobre os assuntos em alta no Brasil. Sempre com as fontes citadas.
lang: pt-BR
permalink: /articles/pt-br/
---

<div class="hero">
  <h1>Tendências do Brasil</h1>
  <p>Resumos originais, localizados com apoio de IA, sobre os assuntos que estão em alta. Sempre com links para as fontes originais.</p>
</div>

## Últimos artigos

{% assign portal_posts = site.posts | where: "lang", "pt-BR" %}
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
  <p>Ainda não há artigos publicados. Volte em breve!</p>
</div>
{% endif %}

<div class="how-it-works">
  <h2>Como funciona</h2>
  <p>Monitoramos sinais públicos de tendências (somente os títulos dos assuntos, nunca o texto das fontes). Uma IA escreve um resumo original em português do Brasil e uma pessoa revisa cada artigo antes da publicação. As fontes originais aparecem sempre no fim de cada texto.</p>
  <p><em>Alguns artigos podem conter links de afiliados, sempre identificados com um aviso de divulgação.</em></p>
</div>

<p><a href="{{ '/' | relative_url }}">← Trend Portals</a> · <a href="{{ '/articles/id/' | relative_url }}" hreflang="id" lang="id">Bahasa Indonesia</a></p>
