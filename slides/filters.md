### Filters

`|raw`

``` php
{% autoescape %}
    {% set hello = '<strong>Hello</strong>' %}
    {% set hola = '<strong>Hola</strong>' %}
    {{ false ? '<strong>Hola</strong>' : hello|raw }}
        does not render the same as
    {{ false ? hola : hello|raw }}
        but renders the same as
    {{ (false ? hola : hello)|raw }}
{% endautoescape %}
```

``` php
{% filter upper %}
    This text becomes uppercase
{% endfilter %}
```
