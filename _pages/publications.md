---
layout: archive
title: "Recent Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can find the full list of my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

<div class="{{ include.type | default: "list" }}__item">
  <article class="archive__item" itemscope itemtype="http://schema.org/CreativeWork">
    <ol class="bibliography">
      {% for post in site.publications reversed %}
        {% include archive-single.html %}
      {% endfor %}
    </ol>
  </article>
</div>
