## La partie Entity sert pour la gestion des tables (relation-champs-validation)
créer un Entity

```powershell
$ Php bin/console make:entity
```


### Une foi la commande envoyée répondre au question suivantes 

nom de la class  de type Entity qui va être crée 
```powershell
Class name of the entity to create or update (e.g. OrangeGnome):
> Article
```

nom du champ dans la table défini par l’Entity 
 ```powershell
New property name (press <return> to stop adding fields):
 > title
```

type de champ ou type de relation que vous souhaitez Il propose string je suis ok j'appuie sur entrer  
([Voir tous les types possibles](Sy1.13_Les-differents-types-de-champs.md))
```powershell
Field type (enter ? to see all types) [string]:
>
```

longeur du champ je suis ok donc entrer
```powershell
Field length [255]:
>
```

le champ peut il être null 
il propose automatiquement no je suis ok donc entrer 
```powershell
Can this field be null in the database (nullable) (yes/no) [no]:
>
```


