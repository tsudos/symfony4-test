MAIN TYPES

  * string
  * text
  * boolean
  * integer (or smallint, bigint)
  * float

RELATIONSHIPS / ASSOCIATIONS
  
  * relation (a wizard will help you build the relation)

les différents types de relations entre les entity

  * ManyToOne

Chaque catégorie concerne (a) un article.   
            Chaque article peut concerner plusieurs objets de la catégorie
  * OneToMany

Chaque catégorie peut avoir une relation avec de nombreux objets Article.
              		     Chaque article concerne (a) une catégorie
  
  * ManyToMany

Chaque catégorie peut avoir une relation avec de nombreux objets Article.
Chaque article peut également concerner de nombreux objets de catégorie

  * OneToOne

OneToOne Chaque catégorie concerne (a) exactement un article.
Chaque article concerne également (a) exactement une catégorie


ARRAY/OBJECT TYPES

  * array (or simple_array)
  * json
  * object
  * binary
  * blob

DATE/TIME TYPES
  * datetime (or datetime_immutable)
  * datetimetz (or datetimetz_immutable)
  * date (or date_immutable)
  * time (or time_immutable)
  * dateinterval

OTHER TYPES
  * json_array
 * decimal
  * guid

