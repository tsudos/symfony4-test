la sécurité des formulaire se passe dans le fichier entity correspondant au controller du formulaire
    `Src/Entity/Name.php`
    
`Source: https://symfony.com/doc/current/validation.html`
Les validations de champs se font dans les commentaires avec le mot clè `@Assert`

```php
/**
* @Assert\NotBlank
*/
```


Grâce à la librairie `symfony/validator doctrine/annotations` 
si besoin installer le composant validator de doctrine pour activer  les annotations
```powershell
composer require symfony/validator doctrine/annotations
```

et pour l’utiliser dans le fichier
`Src/Entity/Name.php
use Symfony\Component\Validator\Constraints as Assert;`
