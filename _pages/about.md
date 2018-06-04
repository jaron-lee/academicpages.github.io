---
permalink: /
title: "Jaron Lee"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
I'm a Sydney-based data scientist, born in Hong Kong, raised in Perth. I'm interested in statistics, machine learning, data science, and programming. I completed a degree in statistics, and currently work for a data science startup called [Hivery](https://www.hivery.com). In my spare time I enjoy learning German, and sing as part of a choral group called [Vox Canvas](https://www.facebook.com/voxcanvas/).

## Latest Blog Post
{% assign post = site.posts.first %}
{% capture written_year %}'None'{% endcapture %}
{% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
{% if year != written_year %}
<h2 id="{{ year | slugify }}" class="archive__subtitle">{{ year }}</h2>
{% capture written_year %}{{ year }}{% endcapture %}
{% endif %}
{% include archive-single.html %}

