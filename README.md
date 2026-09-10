# Data Dictionary of a Blog


# Article:

| name              | meaning                      | type    | nullable | countable | exemple                |
| ----------------- | ---------------------------- | ------- | -------- | --------- | ---------------------- |
| article_id        | unique id                    | int     | no       | no        | 101                    |
| article_name      | name of the article          | varchar | no       | no        | My first article       |
| description       | description of the article  | text    | no       | no        | Introduction to HTML   |
| content           | content of the article      | text    | no       | no        | HTML is a markup...    |
| image             | cover image of the article  | varchar | yes      | no        | url                    |
| category_id       | category of the article     | int     | no       | no        | 2                      |
| author_id         | author of the article       | int     | no       | no        | 10                     |
| date_publication  | publication date of article | date    | no       | no        | 10-09-2026             |
| status            | draft / published           | enum    | no       | no        | published              |


# Authors:

| name         | meaning                    | type    | nullable | countable | exemple          |
| ------------ | -------------------------- | ------- | -------- | --------- | ---------------- |
| author_id    | unique id                  | int     | no       | no        | 10               |
| name         | full name of the author    | varchar | no       | no        | Oussama          |
| email        | email address of the author| varchar | no       | no        | user@gmail.com   |
| password     | password of the author     | varchar | no       | no        | ********         |
| image_auteur | profile picture of author  | varchar | yes      | no        | url              |


# Categories:

| name         | meaning                    | type    | nullable | countable | exemple          |
| ------------ | -------------------------- | ------- | -------- | --------- | ---------------- |
| category_id  | unique id                  | int     | no       | no        | 2                |
| category_name| name of the category       | varchar | no       | no        | Development      |
| color        | color of the category      | varchar | no       | no        | #3498DB          |
| icon         | icon of the category       | varchar | no       | no        | code             |