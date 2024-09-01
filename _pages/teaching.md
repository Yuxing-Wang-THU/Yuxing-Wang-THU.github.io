---
layout: page
permalink: /photos/
title: Gallery
description: I am not expert in photography, but I like keep a record of happy times. 
nav: true
nav_order: 6
---

{% for gallery in page.galleries %}
<div style="width: 35em; text-align: center; padding: 1em 0 4em 0;">
    <a href="{{ gallery['gallery'] }}">
        <img style="max-height: 20em; max-width: 20em;" src="{{ gallery['gallery'] }}/thumbs/{{ gallery['best_image'] }}">
    </a>
    <h3><a href="{{ gallery['gallery'] }}">{{ gallery["name"] }}</a></h3>
    {{ gallery["images"] | size }} images
</div>
{% endfor %}

<style TYPE="text/css">
.gallery-image-wrapper {
  height: 300px;
  width: 300px;
  display: inline-block;
  margin: 1em;
  position: relative;
  text-align: center;
}
.gallery-image {
  margin: auto;
  position: absolute;
  top: 0px;
  bottom: 0px;
  max-height: 100%;
  max-width: 100%;
}
</style>
<h1><a href="/{{ site.gallery_dir }}">{{ page.title }}</a></h1>
<hr />
{% for image in page.images %}
    <div class="gallery-image-wrapper">
			<a href="{{ image }}"><img class="gallery-image" src="thumbs/{{ image }}" /></a>
			<div>
				<p>
					height:{{ page.photos[image].height }} width:{{ page.photos[image].width }}
				</p>
				<p>model:{{ page.photos[image].model }} data_time:{{ page.photos[image].data_time }} </p>
				<p>exposure_time: {{ page.photos[image].exposure_time }} f_number:{{ page.photos[image].f_number }}</p>
			</div>
    </div>
{% endfor %}

