---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Contents
---

<div class="grid-container">

		{% for post in site.posts %}

		<div class="blog-roll">
				{% if post.image%}
				<img src="{{- post.image | relative_url -}}" alt="" class="blog-roll-img">
				{% endif %}
		</div>
		<div class="headline-grid">
			<h2> <a href="{{ post.url }}"> {{ post.title }} </a></h2>
			<h6 class="post_excerpt"> {{ post.headline }} </h6>
			
		</div>

		{% endfor %}

</div>
