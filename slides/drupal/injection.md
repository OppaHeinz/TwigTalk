# Variable Injection

## Preprocessing Hooks

mytheme.theme

``` php
/**
 * Implements hook_preprocess_HOOK() for node.html.twig.
 */
function mytheme_preprocess_node(&$variables) {
  $variables['foo'] = 'bar';
}
```

node.html.twig

``` php
<h1 {{ foo }} </h1>
```