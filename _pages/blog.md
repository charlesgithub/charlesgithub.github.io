---
layout: page
title: Blog
description: Errol Tech Blog
permalink: /blog/
---

<div class="home">

  {% for post in site.posts %}
	<h2 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
	<p class="post-meta">{{ post.date | date_to_string }}</p>
	<div class="post-banner" style="background-image: url({{ post.img-url }});">
		<img src="{{ post.img-url }}" alt="Jekyll From Scratch - Core Architecture">
	</div>

	<p class="post-excerpt">{{ post.excerpt  | strip_html }}&hellip; [<a href="{{ post.url }}">read more</a>]</p>
{% endfor %}

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div>
