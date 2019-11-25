```powershell
php bin/console server:run 0.0.0.0:8000
```
## :warning:
si vous avez wampserver ou tout autre SGBD d'ouvert lancer la commande

```powershell
php bin/console server:run 
```
Après avoir lancé le server interne ouvrir votre navigateur et aller sur l’adresse donnée en référence.
Si tous fonctionne bien la page d’intro de symfony 4 s’affiche

## :warning:
Pour stoper le serveur 

```diff
Ctrl + c
```
## la barre de debug

si a la place de la barre de debug en bas de votre page html dans votre navigateur vous avez 

rien


entrer cette commande dans votre shell

```powershell
composer require --dev symfony/apache-pack
```
 et repond "y" à la question

cela va creer un fichier .Htaccess à la base de votre dossier *public* 