# LE FORMULAIRE ::  TYPE
Dans le fichier
		`Src/form/NameType.php`
Les class `NameType` gèrent la création des champs de l’article et leurs types

```php
{
public function buildForm(FormBuilderInterface $builder, array $options)
    $builder
        ->add('title')
        ->add('category', EntityType::class, [
            'class' => Category::class,
            'choice_label' => 'title'
        ])
        ->add('content')
        ->add('image')
        
    ;
}
```


`:warning: Ne pas oublier d’inclure les entity correspondant à la demande dans notre cas` 


```php
use App\Entity\Article;
use App\Entity\Category;
```



:warning: Quand on donne un type précis à un champs ne pas oublier d’ inclure sa class distante avec un Use
dans le vue
