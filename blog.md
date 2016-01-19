---
layout: page
title: Sean's Blog
permalink: /blog/
---
<div class="row">
	<div class="col-xs-4 col-sm-4 col-md-4">
		<h1 class="page-heading">Posts</h1>
		<ul class="post-list">
			{% for post in site.posts %}
			<li>
				<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
				<h2>
					<a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
				</h2>
			</li>
			{% endfor %}
		</ul>
		<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
	</div>
	<div class="col-xs-2 col-sm-2 col-md-2e"></div>
	<img src="/images/golf_pic.jpg" class="img-responsive" id="about-me-pic">
</div>
