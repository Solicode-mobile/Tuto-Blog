# Data Dictionary of a School Management System


# Course:

| name        | meaning                         | type    | nullable | countable | exemple                  |
| ----------- | ------------------------------- | ------- | -------- | --------- | ------------------------ |
| id          | unique id                       | int     | no       | no        | 101                      |
| name        | course name                     | varchar | no       | no        | Web Development          |
| content     | course content                  | text    | no       | no        | Introduction to HTML...  |
| description | course description              | text    | no       | no        | Basic web development    |
| img         | course image                    | varchar | yes      | no        | url                      |
| status      | published / draft               | enum    | no       | no        | published                |
| category_id | category of the course          | int     | no       | no        | 2                        |
| user_id     | teacher or user of the course   | int     | no       | no        | 10                       |


# User:

| name  | meaning                | type    | nullable | countable | exemple            |
| ----- | ---------------------- | ------- | -------- | --------- | ------------------ |
| id    | unique id              | int     | no       | no        | 10                 |
| name  | user name              | varchar | no       | no        | Oussama            |
| email | user email address     | varchar | no       | no        | user@gmail.com     |


# Category:

| name        | meaning                 | type    | nullable | countable | exemple              |
| ----------- | ----------------------- | ------- | -------- | --------- | -------------------- |
| id          | unique id               | int     | no       | no        | 2                    |
| name        | category name           | varchar | no       | no        | Web Development      |
| description | category description    | text    | yes      | no        | Programming courses  |