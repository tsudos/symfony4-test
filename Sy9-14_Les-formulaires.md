Source:https://symfony.com/doc/current/forms.html

Pour créer un formulaire avec la console 
```powershell
$ php bin/console make:form 
**```
déterminer le nom du formulaire qui dois se terminer par “Type”
```powershell
ArticleType
```
puis dire sur quel entité se base le formulaire ici l'entity article
```powershell
Sur quel entity se base le form
Article
```

 
Cette commande et les réponses données vont créer un dossier form dans le dossier *src* et place le fichier

```makefile
ArticleType.php
```
Dans le dossier *Src/Type/*
