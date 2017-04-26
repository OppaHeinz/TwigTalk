# Filters

## Translation

``` php
<a href="{{ url('<front>') }}" title="{{ 'Home'|t }}" rel="home" class="site-logo"></a>
```

``` php
{% trans %}Submitted on {{ date|placeholder }}{% endtrans %}
```

## Aditional

clean_class, clean_id, format_date, raw, render, safe_join, without