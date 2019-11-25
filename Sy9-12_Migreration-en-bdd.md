### Une foi l’Entity Créer et tous les champs créés préparer la migration avec la commande

```powershell
php bin/console make:migration
```

Cette commande va créer un fichier versionner de mes migrations

## CRÉER LA TABLE AVEC DOCTRINE

Une foi la migration préparer lancer la migration pour créer la table corespondante avec la commande
```powershell
php bin/console doctrine:migrations:migrate 
Q/ voulez vous éxécuter le script de migration
R/y ((yes))

```

Cette commande va créer ma table article dans la bdd avec les champs
