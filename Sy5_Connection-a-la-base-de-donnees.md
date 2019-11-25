##### La connection à la base de données se fait dans le fichier *.env* à la ligne
chercher la ligne 

```yaml
DATABASE_URL=mysql://db_user::db_password@127.0.0.1:3306/db_name
```

#### MODIFIER LE CHAMPS

db_user: => votre nom d’user ou vide si pas de nom d user
db_password =>votre assword ou vide si pas de password
db_name => le nom de la base de données 


## :warning:
Attention ne créer pas votre base de données dans votre SGBD
