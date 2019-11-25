Pour utiliser les styles des templates boostrap par exemple mais aussi tout autre template c’est très simple 
Pour cela dans le fichier 
*Config/package/twig.yaml*
		Ajouter après la dernière ligne
```yaml
form_themes: ['bootstrap_4_layout.html.twig']
```

Puis dans la vue ajouter la ligne
```twig
{% form_theme form 'bootstrap_4_layout.html.twig' %}
```


