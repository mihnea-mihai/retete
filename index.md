# Categorii

{% for category in site.categories %}
  {{ category[0] }}

  {% for post in category[1] %}
  * [{{ post.title }}]({{ post.url | absolute_url }})
  {% endfor %}
{% endfor %}

{% for tag in site.tags %}
  {{ tag[0] }}

  {% for post in tag[1] %}
  * [{{ post.title }}]({{ post.url | absolute_url }})
  {% endfor %}
{% endfor %}

