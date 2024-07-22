---
layout              : page
show_meta			: false
title               : "Contact"
header:
   image_fullwidth  : "header_unsplash_2-970x.jpg"
permalink           : "/contact/"
---
<div>
	<p> You can get in touch with me using one of the following ways: </p>
	<ul class="contact-icons">
		{% for social_item in site.data.socialmedia %}
			<li>
				<a href="{{ social_item.url }}"> {{social_item.name}} </a> 
				<a href="{{ social_item.url }}" target="_blank" class="{{ social_item.class }}" title="{{ social_item.title }}"></a>
			</li>
		{% endfor %}
	</ul>
</div>
