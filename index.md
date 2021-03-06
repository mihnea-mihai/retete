# Rețete

{% for category in site.categories %}
** {{ category[0] }} **
  ** {{ category[0] }}
{% endfor %}

{{ site.categories | array_to_sentence_string }}

{% for category in site.categories %}
  {{ category[0] }}

  {% for post in category[1] %}
  * [{{ post.title }}]({{ post.url | absolute_url }})
  {% endfor %}
{% endfor %}

