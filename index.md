# Rețete 
{% for post in site.posts %}  
  [{{ post.title }}]({{ site.url }}/retete{{ post.url }})  
{% endfor %}  
