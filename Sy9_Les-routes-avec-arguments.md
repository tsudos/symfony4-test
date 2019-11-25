### Dans le controller

   ```php
   /**
   * @Route("/actu/{id}", name="artcle")
   */
    ```
en ajoutant {id} nous demandons à Symfony de passer l'id dans l'URL
		
 
L’ argument href du <a> Dans la vue
```twig
{{ path(name_of_the_route,{id : article.id})}}
```



