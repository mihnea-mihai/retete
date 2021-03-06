# Rețete 
{% for post in site.posts %}  
  [{{ post.title }}]({{ site.url }}/retete{{ post.url }})  
{% endfor %}  

{% for category in site.categories %}  
    {% for post in site.posts %}  
    category  
      {% if post.category == category %}
        [{{ post.title }}]({{ site.url }}/retete{{ post.url }})
      {% endif %}  
    {% endfor %}  
{% endfor %}  
