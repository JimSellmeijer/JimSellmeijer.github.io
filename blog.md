---
title: "Blog: Effectively Software Development"
layout: landing
# image: assets/images/pic07.jpg
nav-menu: True
show-tile: false
---

<!-- Main -->
<div id="main">

<!-- Two -->
<section id="two" class="spotlights">
		{% for post in site.posts %}
		{% if post.title != 404 %}
		<section>
		<a href="generic.html" class="image">
			<img src="{{ site.url }}/{{ post.image }}" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>{{ post.title }}</h3>
				</header>
				<p>{{post.description}}
				</p>
				<ul class="actions">
					<li><a href="{{ site.url }}{{ post.url }}" class="button">Learn more</a></li>
				</ul>
			</div>
		</div>
	</section>
	{% endif %}
	{% endfor %}
</section>

</div>
