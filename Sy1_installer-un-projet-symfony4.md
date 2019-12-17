Pour de microservices
```powershell
composer create-project symfony/skeleton my-project
```

Pour des applications web simple comme des blogs
```powershell
Composer create-project symfony/website-skeleton my-projet
```

Maintenant que nous avons installé le projet symfony, il faut installer le server interne de symfony4



(stephane Dufour) =>
Depuis la mise à jour Symfony 5, si on veut installer une version anterieur de Symfony on utilise ":^4.4" pour spécifier la version souhaité du projet (là il s'agit de Symfony 4.4) :


composer create-project symfony/website-skeleton:^4.4 my-projet
