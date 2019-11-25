## FILE
`Source: https://symfony.com/doc/current/reference/constraints/File.html`
Cette méthode vérifie plusieurs containtes sur le fichier téléchargé
```php
/**
   * @Assert\File(
   *     maxSize = "1024k",
   *     mimeTypes = {"application/pdf", "application/x-pdf"},
   *     mimeTypesMessage = "Please upload a valid PDF"
   * )
   */
```
### `File` peut prendre plusieurs paramettre

## maxSize

<table>
<thead>
	<tr>
		<th>Suffixe</th>
		<th>Nom de l'unité</th>
		<th>Valeur</th>
		<th>Exemple</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td>(aucun)</td>
		<td>Octet</td>
		<td>1 octet</td>
		<td>4096</td>
	</tr>
    <tr>
		<td>(aucun)</td>
		<td>Octet</td>
		<td>1 octet</td>
		<td>4096</td>
	</tr>
    <tr>
		<td>k</td>
		<td>Kilooctet</td>
		<td>1000 octets</td>
		<td>200k</td>
	</tr>
    <tr>
		<td>M</td>
		<td>Mégaoctet</td>
		<td>1 000 000 octets</td>
		<td>2M</td>
	</tr>
    <tr>
		<td>Ki</td>
		<td>Kibibyte</td>
		<td>1 024 octets</td>
		<td>32Ki</td>
	</tr>
    <tr>
		<td>Mi</td>
		<td>Mebibyte</td>
		<td>1 048 576 octets</td>
		<td>8Mi</td>
	</tr>	
</tbody>
</table>


#### . La taille du fichier peut être donnée dans l’un des formats suivants:
			
	

## maxSizeMessage 

### les paramètres suivants dans le message lier au maxSizeMessage message:
<table>
    <thead>
        <tr>
            <th>Paramètre</th>
            <th>La description   </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>{{ file }}</td>
            <td>Chemin de fichier absolu  </td>
        </tr>
        <tr>
            <td>{{ limit }}</td>
            <td>Taille de fichier maximale autorisée  </td>
        </tr>
        <tr>
            <td>{{ name }}</td>
            <td>Nom du fichier de base     </td>
        </tr>
        <tr>
            <td>{{ size }}</td>
            <td>Taille du fichier donné  </td>
        </tr>
        <tr>
            <td>{{ suffix }}</td>
            <td>Suffixe pour l'unité de taille de fichier utilisée (voir ci-dessus) </td>
        </tr>
    </tbody>
</table>

### uploadErrorMessage 
Le message qui s'affiche si le fichier téléchargé n'a pas pu être chargé pour une raison inconnue.

### uploadExtensionErrorMessage
Le message qui s'affiche si une extension PHP entraîne l'échec du téléchargement du fichier.

### uploadFormSizeErrorMessage
Le message qui s'affiche si le fichier téléchargé est plus volumineux qu'autorisé par le champ de saisie du fichier HTML.

### uploadIniSizeErrorMessage
Le message qui s'affiche si le fichier téléchargé est plus volumineux que le upload_max_filesize php.iniparamètre.
Vous pouvez utiliser les paramètres suivants dans ce message:
<table>
    <thead>
        <tr>
            <th>Paramètre</th>
            <th>La description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>{{ limit }}</td>
            <td>Taille de fichier maximale autorisée</td>
            
        </tr>
        <tr>
            <td>{{ suffix }}</td>
            <td>Suffixe pour l'unité de taille de fichier utilisée (voir ci-dessus)</td>
        </tr>
    </tbody>
</table>


### uploadNoFileErrorMessage
Le message qui s'affiche si aucun fichier n'a été téléchargé.

### uploadNoTmpDirErrorMessage
Le message qui s'affiche si le paramètre `php.ini` `upload_tmp_direst` manquant.

### uploadPartialErrorMessage
Le message qui s'affiche si le fichier téléchargé n'est que partiellement téléchargé.


## IMAGE
`Source: https://symfony.com/doc/current/reference/constraints/Image.html`

Cette méthode vérifie plusieurs contrainte sur un fichier photo
```php
/**
     * @Assert\Image(
     *     minWidth = 200,
     *     maxWidth = 400,
     *     minHeight = 200,
     *     maxHeight = 400
     * )
     */
```


#### :warning: Image contient plusieurs paramettre
### MAXHEIGHT
Si défini, la hauteur du fichier image doit être inférieure ou égale à cette valeur en pixels.

### MAXHEIGHTMESSAGE
:The image height is too big `({{ height }}px)`. Allowed maximum height is `{{ max_height }}`px.
Vous pouvez utiliser les paramètres suivants dans ce message:
<table>
    <thead>
        <tr>
            <th>parametre</th>
            <th>description</th>
        </tr>
    </thead>
    <tbody>
    <tr>
        <td>{{ height }}</td>
        <td>	La hauteur actuelle (invalide)</td>
    </tr>
    <tr>
        <td>{{ max_height }}</td>
        <td>La hauteur maximale autorisée</td>
    </tr>
    </tbody>
</table>

	
### MAXPIXELS
Si défini, la quantité de pixels du fichier image doit être inférieure ou égale à cette valeur.

### maxPixelsMessage
The image has to many pixels `({{ pixels }} pixels)`. Maximum amount expected is `{{ max_pixels }}` pixels.
Vous pouvez utiliser les paramètres suivants dans ce message:

<table>
<thead>
	<tr>
		<th>valeur</th>
		<th>La description</th>
	</tr>
</thead>
<tbody>
    <tr>
        <td>{{ height }}</td>
        <td>	La hauteur actuelle de l'image</td>
    </tr>
    <tr>
        <td>{{ max_pixels }}</td>
        <td>La quantité maximale autorisée de pixels</td>
    </tr>
    <tr>
        <td>{{ pixels }}</td>
        <td>La quantité actuelle de pixels</td>
    </tr>
    <tr>
        <td>{{ width }}</td>
        <td>La largeur de l'image actuelle</td>
    </tr>
</tbody>
</table>

## GERER LE RETPUR DES ERREURS 
Vous pouvez également transférer la collection d'erreurs dans un modèle☹controller)
```php
if (count($errors) > 0) {
    return $this->render('author/validation.html.twig', [
        'errors' => $errors,
    ]);
}
```


Dans le modèle, vous pouvez générer la liste des erreurs exactement comme vous le souhaitez:

```html
{# templates/author/validation.html.twig #}
<h3>The author has the following errors</h3>
<ul>
{% for error in errors %}
    <li>{{ error.message }}</li>
{% endfor %}
</ul>
```



