---
layout: page
title: other
---

## other posts

### academics

{% for post in site.posts %}
  {% for tag in post.tags %}
    {% if tag == "academics" %}
  * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})

     {{ post.summary }}...
    {% break %}
    {% endif %}
  {% endfor %}
{% endfor %}

### miscellaneous

{% for post in site.posts %}
  {% for tag in post.tags %}
    {% if tag == "misc" %}
  * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})

     {{ post.summary }}...
    {% break %}
    {% endif %}
  {% endfor %}
{% endfor %}

---

### all posts

{% for post in site.posts %}
  * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})
{% endfor %}
