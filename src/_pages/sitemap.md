---
layout: page
permalink: /sitemap/
title: "Sitemap"
excerpt: "An index of all the pages found on mademistakes.com"
---

A hierarchical breakdown of all the sections and pages found on the site. For you robots out there, here is an [XML version]({{ site.url }}/sitemap.xml) available for your crawling pleasure.

<h2>Pages</h2>
<ul>
  <li><a href="{{ site.url }}/about/">About</a></li>
  <li><a href="{{ site.url }}/contact/">Contact</a></li>
  <li><a href="{{ site.url }}/faqs/">Frequently Asked Questions</a></li>
  <li><a href="{{ site.url }}/support/">Support</a></li>
  <li><a href="{{ site.url }}/tag/">Tag Archive</a></li>
  <li><a href="{{ site.url }}/terms/">Terms and Policies</a></li>
</ul>

<h2><a href="{{ site.url }}/articles/">Blog Articles</a></h2>
<ul>
  {% for post in site.categories.articles %}
    {% include post-list.html %}
  {% endfor %}
</ul>

<h2><a href="{{ site.url }}/til/">Today I Learned</a></h2>
<ul>
  {% for post in site.categories.til %}
    {% include post-list.html %}
  {% endfor %}
</ul>

<h2><a href="{{ site.url }}/mastering-paper/">Mastering Paper by FiftyThree</a></h2>
<ul>
  {% for post in site.categories.mastering-paper %}
    {% include post-list.html %}
  {% endfor %}
</ul>

<h2><a href="{{ site.url }}/work/">Portfolio Work</a></h2>
<ul>
  {% for post in site.work %}
    {% include post-list.html %}
  {% endfor %}
</ul>
