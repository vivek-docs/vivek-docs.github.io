---
layout: default
permalink: /travelogue/
title: travelogue
nav: true
nav_order: 4
pagination:
  enabled: true
  collection: posts
  permalink: /page/:num/
  per_page: 5
  sort_field: date
  sort_reverse: true
  trail:
    before: 1 # The number of links before the current page
    after: 3 # The number of links after the current page
---

I ride bicycles into places that have no business being cycled in. Then I write about it and photograph everything along the way.

These are not travel guides. They are honest accounts of what it feels like to be small on a big road — the exhaustion, the altitude, the silence, and the occasional moment where everything is exactly right.

<div style="display: flex; gap: 1rem; margin: 2rem 0; flex-wrap: wrap;">
  <a href="https://medium.com/@vivek.author" target="_blank"
     style="display: inline-flex; align-items: center; gap: 0.5rem; padding: 0.75rem 1.5rem;
            background: var(--global-theme-color); color: white; border-radius: 8px;
            text-decoration: none; font-weight: 500;">
    ✍️ Read on Medium
  </a>
  <a href="https://www.youtube.com/@InnerWheelJourneys" target="_blank"
     style="display: inline-flex; align-items: center; gap: 0.5rem; padding: 0.75rem 1.5rem;
            background: #ff0000; color: white; border-radius: 8px;
            text-decoration: none; font-weight: 500;">
    ▶ Watch on YouTube
  </a>
</div>

---

## Latest Rides from Medium

<!-- RSS feed is pulled via _config.yml external_sources -->
<!-- Add your Medium RSS below once you confirm your handle -->

{% if site.external_sources %}
  {% for source in site.external_sources %}
    {% if source.name == "medium.com" %}
      {% for post in site.data.external_posts[source.name] %}
<div style="padding: 1rem 0; border-bottom: 1px solid var(--global-divider-color);">
  <a href="{{ post.url }}" target="_blank" style="font-size: 1.1rem; font-weight: 500;">
    {{ post.title }}
  </a>
  <p style="font-size: 0.85rem; opacity: 0.6; margin: 0.25rem 0 0;">
    {{ post.date | date: "%B %d, %Y" }}
  </p>
</div>
      {% endfor %}
    {% endif %}
  {% endfor %}
{% endif %}

---

## Photography

Every image you see in my articles was taken by me — on the road, in the moment, with whatever light was available. No stock photography, no filters beyond what the mountain already provides.

All photos © Vivek M. Deshmukh