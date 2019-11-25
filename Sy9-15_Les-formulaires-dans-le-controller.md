### Dans le controller 

Instancier le formulaire


```php
$form = $this->createForm(NameType::class, $function);
        $form->handleRequest($request);
```



et bien-sur retourner le formulaire à la vue 

```php
return $this->render('blog/create.html.twig', [
            'formArticle' => $form->createView(),
        ]);
```

