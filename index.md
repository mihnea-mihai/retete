# Rețete 

{% for category in site.categories %}
  {{ category[0] }}

  {% for post in category[1] %}
  * [{{ post.title }}]({{ site.url }}/retete{{ post.url }})
  {% endfor %}
{% endfor %}

