---
layout: default
title: Beranda
---
<div class="document-list">
    {% for post in site.posts %}
    <div class="document-item">
        <a href="{{ post.pdf_link }}" class="document-link">{{ post.title }}</a>
        <div class="document-meta">
            {{ post.date | date: "%d %B %Y" }} &bull; {{ post.categories }}
        </div>
    </div>
    {% endfor %}
</div>
