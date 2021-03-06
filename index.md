# Rețete 
{% for post in site.posts %}  
  [{{ post.title }}]({{ site.url }}/retete{{ post.url }})  
  {{ post.url }}  
  {{ page.url }}  
  {{ site.url }}  
  {{ site.url }}/retete{{ post.url }}  
{% endfor %}  
