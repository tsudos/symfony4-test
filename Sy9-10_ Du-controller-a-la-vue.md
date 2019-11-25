Pour retourner les différents variable à la vue et donc à twig il faut utiliser l’action rendre
	   
```php
return $this->render('artcle/index.html.twig', [
         'controller_name' => 'ArtcleController',
         'NomUtilisableDansLaVue' => $variableAenvoyerALaVue,
     ]);
```

exemple pour envoyer la variable $article dans la vue 


```php
return $this->render('artcle/index.html.twig', [
         'controller_name' => 'ArtcleController',
         'article' => $article,
     ]);
```



Dans la vue 

  ```html
{% for articles in article %}
       <div class="col-sm-4">
           <div class="card">
               <!--{{ articles.category.title}} renvoie le titre des ctégories relier à l'article-->
           <span class="badge blog text-white">{{ articles.category.title}} </span>
               <img src="{{ articles.image}}" class="card-img-top" alt="...">
               <div class="card-body">
                   <!--{{ articles.title}}  renvoie le titre de l'article-->
                   <h5 class="card-title">{{ articles.title}} </h5>
                  <!--{{ articles.CreatedAt | date('d/m/Y')}} renvoie la date en argument il faut luis passer le formatage de la date ici date('d/m/Y') idem pour l'heure {{ articles.CreatedAt | date('H:i')}}-->
                       <div class="cardTime">Poster le {{ articles.CreatedAt | date('d/m/Y')}} à {{ articles.CreatedAt | date('H:i')}}</div>     
                      <!--{{ articles.content | croptext}} renvoie le contenue de l'article avec en parametre un filtre twig [croptext](helper_Symfony%2FSy-Helper.md)-->
                   <p class="card-text">{{ articles.content | croptext}} </p>
                   <!--path avec argument {{ path('blog_show', {id: articles.id})}} ici l'id de l'article-->
                   <p class='text-right'><a href="{{ path('blog_show', {id: articles.id})}} " class="btn btn-info justify-content-between">lire la suite</a></p>
               </div>
           </div>
       </div>
   {% endfor %}
```
