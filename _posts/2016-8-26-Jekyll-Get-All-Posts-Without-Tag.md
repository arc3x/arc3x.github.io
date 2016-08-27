---
layout: post
title: Jekyll / Liquid Get All Posts Without A Tag
---

This took me some piecing together and wasn't readily available on a google search.

The `unless` conditional is basically an `if not`

```
{% raw %}
{% for post in site.posts %}
  {% unless post.tags contains "no_blog" %}

    ... content ...

  {% endunless %}
{% endfor %}
{% endraw %}
```
