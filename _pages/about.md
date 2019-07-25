---
permalink: /
title: "Jaron Lee"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
I'm a PhD student in the [Department of Computer Science](https://www.cs.jhu.edu) at the Johns Hopkins University working with [Ilya Shpitser](https://www.cs.jhu.edu/~ilyas/). I'm interested in applying causal inference to solving problems in healthcare.


## Latest Blog Post
{% assign post = site.posts.first %}
{% capture written_year %}'None'{% endcapture %}
{% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
{% if year != written_year %}
<h2 id="{{ year | slugify }}" class="archive__subtitle">{{ year }}</h2>
{% capture written_year %}{{ year }}{% endcapture %}
{% endif %}
{% include archive-single.html %}

