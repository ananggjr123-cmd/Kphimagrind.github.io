---
layout: default
title: Beranda
---
<div class="document-list">
    {% for post in site.posts %}
    <div class="document-item">
        <a href="{{ site.baseurl }}{{ post.url }}" class="document-link">{{ post.title }}</a>
        <div class="document-meta">
            {{ post.date | date: "%d %B %Y" }} &bull; {{ post.categories }}
        </div>
    </div>
    {% endfor %}
</div>
