---
title: Archive
layout: default
---

<div class="object order">
<div class="year order">Date</div>
<div class="project order">Title</div>
<div class="type order">Type</div>
<div class="publication order">Publication</div>
</div>

<main class="preview" id="all-container">
{% for post in site.posts %}
        <a href="{{ site.baseurl }}{{ post.url }}">
        <div class="object">
            <div class="year">{{ post.pubdate }}</div>
            <div class="project">{{ post.title }}</div>
            <div class="type">{{ post.categories }}</div>
            <div class="publication">{{ post.publication }}</div>
        </div>
    </a>
    {% endfor %}

</main>

<section class="clear"></section>

