# Rețete 

{% for category in site.categories %}
  {{ category[0] }}

  {% for post in category[1] %}
  * [{{ post.title }}]({{ site.url }}/retete{{ post.url }})
  * [{{ post.title }}](_posts/2021-02-28-gris-cu-lapte.md)
  * [{{ post.title }}]({{ post.url | absolute_url }})
  {% endfor %}
{% endfor %}

