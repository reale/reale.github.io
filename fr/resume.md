---
layout: page
title: CV
lang: fr
ref: resume
permalink: /fr/resume
---

<section>
	<header class="major">
		<h2>CV</h2>
	</header>
	<div class="posts">
	{% for post in site.categories.resume %}
		<article>
			<a href="{{ site.baseurl }}{{ post.url }}" class="image"><img src="{{ post.image }}" alt="" /></a>
			<h3><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
			<p>{{ post.excerpt }}</p>
			<ul class="actions">
				<li><a href="{{ post.url }}" class="button">{{ site.data.labels.read-more[page.lang] }}</a></li>
			</ul>
		</article>
	{% endfor %}
	</div>
</section>