## Macros

``` php
{% macro input(name, value, type, size) %}
<input type="{{ type|default('text') }}" name="{{ name }}" value="{{ value|e }}" size="{{ size|default(20)
}}" />
{% endmacro %}
```

``` php
{% import "forms.html" as forms %}
<p>{{ forms.input('username') }}</p>
```
