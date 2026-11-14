---
layout: default
title: Beiträge
---
# Politik in Deutschland, fachlich eingeordnet

Wöchentliche Analysen zu aktuellen politischen Entwicklungen in Deutschland. Jeder Beitrag stützt sich auf Primärquellen und Forschung und benennt Gegenpositionen und Unsicherheiten.

<ul class="post-list">
{% for post in site.posts %}
  <li>
    <span class="meta">{{ post.date | date: "%d.%m.%Y" }}</span>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {% if post.summary %}<p>{{ post.summary }}</p>{% endif %}
  </li>
{% endfor %}
</ul>
