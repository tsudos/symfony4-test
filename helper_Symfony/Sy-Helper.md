```php
<?php
namespace App\Twig;

use Twig\Extension\AbstractExtension;
use Twig\TwigFilter;

class TwigTexteExtention extends AbstractExtension {
// indiquer les infos du filtre
    public function getFilters()
    {
    // retourner le nom du filtre à utiliser dans la vue puis dans [$this représente ]
     //   return [NomDuFiltreFilter], puis [is_safe dit retourne du [html]]
            
            new TwigFilter('croptext', [$this, 'croptextFilter'],['is_safe' => ['html']] )
        ];
    }
//la creation m^me du filtre prend le contenu et aucune option : retourne une chaine de caractères
    public function croptextFilter($content, array $options = []): string
    {
       //definir les option par défault ici le nombre limite de mot par défault
        $defaultOptions = [
            'limit' =>'60'
        ];
        enssuite je fais un array_merge des options par défault et des options
        $options = array_merge($defaultOptions, $options
        );
        // je défini la varible a défault limite en claire dans ma vue si je veux mettre plus ou moins de mot je le rajoute en option sinon j'utilise les options définis par la variable defaultOption
        $limit = $options['limit'];
        // si la taille du content est inférieur ou égale a la limite ont retourne simplement le content
        if (mb_strlen($content) <= $limit) {
            return $content;
        }
        // sinon je retourne le crop de mon content
        
        // $lastpast recherche l'espace en fin de la limite
        $lastspace = mb_strpos($content, ' ',$limit);
        // je retire l'espace en fin de la limite
        $content = mb_substr($content, 0, $lastspace);
        // je retourne le content entre une balise de paragraphe
        return '<p>'.$content.' ...</p>';
    }

}
```
