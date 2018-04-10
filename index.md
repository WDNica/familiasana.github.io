---
layout: home
permalink: /
image:
  feature: wood-texture-1600x800.jpg
tags: [family, children, parents, children, children, girls, adolescents, child, care, education, education, health, child care, learning, maternal care, matenality, school, homework, money, finances, home, manage, house, baby, baby, life, home care, learning, fashion, personal care, exercise, homework, school, illness, diseases]
author: admin
---
<!-- {% assign category_name = "life" %}
  {% include latest-posts-list-by-category.html %}

{% assign category_name = "business" %}
  {% include latest-posts-list-by-category.html %}
{% include latest-posts-list.html %}
 -->

 <style>
.supcategory {
font-size: 70%;
position: relative;
bottom: 0.3em;
}
</style>
 <h3>Latest</h3>
<ul>
{% for post in site.posts limit:30 %}
<li>
{% if post.date %}
<span>{{ post.date | date: "%B %d, %Y" }}</span> &raquo;
{% endif %}
<a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
<span class="supcategory">{{ post.categories | first }}</span>
</li>
{% endfor %}
</ul>
