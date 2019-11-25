Dans le fichier
        `src/maVueForm.html.twig`

```html
{% block title %}crér un article{% endblock %}
{% block body %}
    <h1>Création d'un article</h1>
    <!--Création du formulaire formArticle -->
    {{ form_start(formArticle) }}
    <!--Form_rom détermine la ligne du formulaire
        formArticle.title dit que dans le formulaire que nous avons creer dans le form builder nous recuperon le champs titre
        Puis les attributs habituel d'un champs input-->
        {{ form_row(formArticle.title,{'attr' :{ 'placeholder': "Titre de l'article" }}) }}
        {{ form_row(formArticle.category) }}
        <!--il détermine luis m^me le type de champs du formulaire comme ici dans le content il met un textarea-->
        {{ form_row(formArticle.content,{'attr' :{ 'placeholder': "Contenue de l'article" }} )}}
        {{ form_row(formArticle.image,{'attr' :{ 'placeholder': "Image de l'article" }} )}}
        <!--le button peut se mettre en dur-->
        <button type="submit" class="btn btn-success">
            <!--si editMode est a true sinon -->
        {% if editMode %}
            Modifier l'article
        {% else %}
            Enregistrer l'article 
        {% endif %}
        </button>
        <!--fermer le formulaire-->
    {{ form(formArticle) }}
{% endblock %}
```


Et voila notre formulaire est créer reste à le sécuriser 
