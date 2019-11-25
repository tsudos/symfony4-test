## EMAIL
`Source: https://symfony.com/doc/current/reference/constraints/Email.html`
```php
/**
 * @Assert\Email(
 *     message = "The email '{{ value }}' is not a valid email.",
 * )
 */
```


## LENGTH
`Source: https://symfony.com/doc/current/reference/constraints/Length.html`
### Cette méthode de validation détermine la longueur du champs
```php
/**
     * @Assert\Length(
     *      min = 2,
     *      max = 50,
     *      minMessage = "Your first name must be at least {{ limit }} characters long",
     *      maxMessage = "Your first name cannot be longer than {{ limit }} characters"
     * )
     */
```


Les message possèdent deux variables

`{{ limit }}` //définit la limite données
`{{ value  }}` // définit la valeur du champs

## L’URL
`Source: https://symfony.com/doc/current/reference/constraints/Url.html`
### Pour une validation simple
```php
/**
   * @Assert\Url(
   *    message = "The url '{{ value }}' is not a valid url",
   * )
   */
```

 
### Pour vérifier le protocole de l’url
```php
/**
     * @Assert\Url(
     *    protocols = {"http", "https", "ftp"}
     * )
     */
```


## EQUALTO
`Source: https://symfony.com/doc/current/reference/constraints/EqualTo.html`

### Cette méthode vérifie une égalité entre la valeur du champs et une réponse données en paramettre de la contrainte
```php
/**
     * @Assert\EqualTo("Mary")(
     *    message = "The url '{{ value }}' is not a valid url",
     * )
     */
```

La partie message peut renvoyer plusieurs variables

`{{ compared_value }}` // The expected value
`{{ compared_value_type }}` // The expected value type
`{{ value }}` // la valeur du champ 

## NOTEQUALTO
`Source: https://symfony.com/doc/current/reference/constraints/NotEqualTo.html`
### Vérifie si la valeurs du champ n’est pas égale à la valeur passés en paramèttre
```php
/**
     * @Assert\NotEqualTo(
     *     value = 15,
     *     message= « This value should not be equal to {{ compared_value }} »
     * )
     */
```


La partie message peut renvoyer plusieurs variables

`{{ compared_value }}` // The expected value
`{{ compared_value_type }}` // The expected value type
`{{ value }}` // la valeur du champ 

## DATE
`Source: https://symfony.com/doc/current/reference/constraints/Date.html`
### Cette méthode vérifie si la date est bien une date au bon format
```php
/**
     * @Assert\Date(message= »{{ value}} n’est pas une date valide »)
     * @var string A "Y-m-d" formatted value,
     * 
     */
```


## DATETIME
`Source: https://symfony.com/doc/current/reference/constraints/DateTime.html`
### Cette méthode vérifie si la contrainte format de la date  est bien respecté
```php
/**
     * @Assert\DateTime(message= »{{ value}} n’est pas une date valide »)
     * @var string A "Y-m-d H:i:s" formatted value
     */
```


#### Il y a possibilité de créer d’autre format via
```php
$date = DateTime::createFromFormat('j-M-Y', '15-Feb-2009');
Return $date;
```


## TIME
`Source:https://symfony.com/doc/current/reference/constraints/Time.html`
### Cette métode vérifie si le champ est bien un horaire
```php
/**
     * @Assert\Time(message= »{{ value}} n’est pas une heure valide »)
     * @var string A "H:i:s" formatted value
**/
```
