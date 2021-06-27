# Rețete

{% for recipe in site.recipes %}
  * [{{ recipe.title }}]({{ recipe.url }})
{% endfor %}