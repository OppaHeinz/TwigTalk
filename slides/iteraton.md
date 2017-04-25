### Iteration

`for`

``` php
    <ul>
        {% for key, item in items %}
            <!-- start output -->
                <li>{{ key }}. {{ item.caption }}</li>
            <!-- end output -->
        {% else %}
            <!-- start output -->
                <li>No Items to output</li>
            <!-- end output -->
        {% endfor %}
    </ul>

```
