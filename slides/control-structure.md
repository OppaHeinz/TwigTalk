### Control Structure

`if`

``` php
{% if users %}
    <ul>
        {% for user in users %}
        <li>{{ user.username|e }}</li>
        {% endfor %}
    </ul>
{% endif %}

```

``` php
{% if temperature > 18 and temperature < 27 %}
    <p>It is a nice day for a walk in the park.</p>
{% endif %}

```
