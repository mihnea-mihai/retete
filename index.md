# Rețete 
{% for post in site.posts %}  
  [{{ post.title }}]({{ site.url }}/retete{{ post.url }})  
{% endfor %}


{% for category in site.categories %}
  {{ category[0] }}

  {% for post in category[1] %}
    * [{{ post.title }}]({{ site.url }}/retete{{ post.url }})
  {% endfor %}
{% endfor %}


{% for tag in site.tags %}
  {{ tag[0] }}
  {% for post in tag[1] %}
    * [{{ post.title }}]({{ site.url }}/retete{{ post.url }})
  {% endfor %}
{% endfor %}