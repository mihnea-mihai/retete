# Rețete 
{% for post in site.posts %}
  [{{ post.title }}]({{ post.url }})  
  {{ post.url }}  
  {{ page.url }}  
  {{ page.path }}
  {{ site.url }}
  {{ site.url }}{{ post.url }}
{% endfor %}
