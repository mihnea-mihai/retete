# Rețete 
{% for post in site.posts %}  
  [{{ post.title }}]({{ site.url }}/retete{{ post.url }})  
{% endfor %}  

{% for category in site.categories %}  
    {{ category }}  
    {{ category.name }} 
    {{ category.text }}  

    {% for post in site.posts %}  
      {% if post.category == category %}
        [{{ post.title }}]({{ site.url }}/retete{{ post.url }})
      {% endif %}  
    {% endfor %}  
{% endfor %}  

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

{% for tag in site.tags %}
  {{ tag[0] }}
  
    {% for post in tag[1] %}
      {{ post.url }}{{ post.title }}
    {% endfor %}
  
{% endfor %}