## LES ROUTES UTILISE LE COMPOSANT ROUTE

Dans les controllers ajouter le use
```php
use Symfony\Component\Routing\Annotation\Route;
```

1.4.2 LES ROUTES SIMPLE
Dans le controller
Pour utiliser les routes dans un controller ajoure juste au dessu de la fonction 
   ```php
/**
    * @Route("/actu", name="article")
    */
```


les liens utilisent aussi le composant Route en remplaçant le liens habituel de votre href par 
```twig
{{ path(name_of_the_route)}}
```


