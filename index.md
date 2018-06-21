<h1>Liquid</h1>

{% for page in site.html_pages %}
  {% if page.url != '/' %}
  - [{{ page.title }}]({{ page.url | relative_url }})
    - {{page.description}} 
  {% endif %}
{% endfor %}
