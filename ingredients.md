# Ingrediente

{% assign sorted_ingredients = site.ingredients | sort %}

{% for ingredient in sorted_ingredients %}
  * [{{ ingredient.name }}]({{ ingredient.url }})  
{% endfor %}