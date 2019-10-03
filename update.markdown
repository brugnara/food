---
layout: default
category: update
---

{% assign posts = site.posts | where_exp: "item", "item.categories[0] == page.category" %}
{% include post_list.html posts=posts %}
