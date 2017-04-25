`block / extends`

``` php

<!DOCTYPE html>
<html>
    <head>
        {% block head %}
            <link rel="stylesheet" href="style.css" />
            <title>{% block title %}{% endblock %} - My Webpage</title>
        {% endblock %}
    </head>
    <body>
        <div id="content">{% block content %}{% endblock %}</div>
        <div id="footer">
        {% block footer %}
        &copy; Copyright 2011 by <a href="http://domain.invalid/">you</a>.
        {% endblock %}
        </div>
    </body>
</html>

```

 Child template

``` php

{% extends "base.html" %}
    {% block title %}Index{% endblock %}
    {% block head %}
    {{ parent() }}
        <style type="text/css">
        .important { color: #336699; }
        </style>
    {% endblock %}
    {% block content %}
        <h1>Index</h1>
        <p class="important">
        Welcome on my awesome homepage.
        </p>
    {% endblock %}

```
