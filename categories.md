---
layout: page
title: All Post
description: This page displays all posts.
header: All Post
---

## All Post : 

<div class="wrapper" markdown="0">

	<div id="linkdiv1" class="kate1">


		<ul>
		{% for post in site.posts %}
			<!-- ORI  -->
				<li>{{ post.date | date: "%B %d, %Y" }}: <a href="{{site.url}}/TAJ{{post.url}}.html">{{ post.title }}</a></li>
			
			<!-- <li><a href="{{site.url}}{{post.url}}.html">{{ post.title }}</a></li> -->
		{% endfor %}
		</ul>

	
</div>

<!-- <hr> -->
<!-- 
{% for post in site.posts %}	
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p><small><strong>{{ post.date | date: "%B %e, %Y" }}</strong> . {{ post.category }} . <a href="http://erjjones.github.com{{ post.url }}#disqus_thread"></a></small></p>			
{% endfor %} -->