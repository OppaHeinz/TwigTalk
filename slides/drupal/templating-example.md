# Templating

page-title.html.twig

``` php
{{ title_prefix }}
{% if title %}
  <h1{{ title_attributes }}>{{ title }}</h1>
{% endif %}
{{ title_suffix }}
```