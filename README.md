# Data Dictionary of a Blog

This documentation is based on `dictionnaire_donnees.csv`.

`Obligatoire` indicates whether a field is required. `Calculé` indicates whether its value is derived automatically.

## User

| Name | Meaning | Type | Required | Calculated |
| --- | --- | --- | --- | --- |
| `nom` | Nom d'auteur | `VARCHAR` | Oui | Non |
| `prenom` | Prénom d'auteur | `VARCHAR` | Oui | Non |
| `nom complete` | Nom et prénom d'auteur | `VARCHAR` | X | Oui |
| `email` | Adresse email de l'auteur | `VARCHAR` | Oui | Non |
| `mot_de_passe` | Mot de passe de l'auteur | `VARCHAR` | Oui | Non |
| `photo_profil` | Photo de profil de l'auteur | `VARCHAR` | Non | Non |

## Champs calculés liés à l'utilisateur

| Name | Meaning | Type | Required | Calculated |
| --- | --- | --- | --- | --- |
| `date d'inscreption` | Date d'inscription d'auteur | `DATETIME` | Oui | Non |

## Article

| Name | Meaning | Type | Required | Calculated |
| --- | --- | --- | --- | --- |
| `id_article` | ID article | `INT` | Oui | Non |
| `titre` | Titre de l'article | `VARCHAR` | Oui | Non |
| `contenu` | Contenu complet de l'article | `TEXT` | Oui | Non |
| `id_article_precedent` | ID article précédent | `INT` | X | Oui |
| `id_article_suivant` | ID article suivant | `INT` | X | Oui |
| `nombre de vue` | Nombre de vues | `INT` | Oui | Non |
| `image_article` | Image principale de l'article | `VARCHAR` | Non | Non |
| `statut_article` | État de l'article (Brouillon ou Publié) | `ENUM` | Oui | Non |
| `date_creation` | Date de création de l'article | `DATETIME` | Oui | Non |
| `date_publication` | Date de publication de l'article | `DATETIME` | Non | Non |
| `temps_lecture_estime` | Durée estimée nécessaire pour lire l'article | `INT` | X | Oui |

## Champs calculés liés aux articles

| Name | Meaning | Type | Required | Calculated |
| --- | --- | --- | --- | --- |
| `nombre de vue totale` | Nombre de vues totale | `INT` | X | Oui |

## Category

| Name | Meaning | Type | Required | Calculated |
| --- | --- | --- | --- | --- |
| `nom_categorie` | Nom de la catégorie | `VARCHAR` | Oui | Non |
| `couleur` | Couleur associée à la catégorie | `VARCHAR` | Oui | Non |
| `icone` | Icône associée à la catégorie | `VARCHAR` | Oui | Non |
