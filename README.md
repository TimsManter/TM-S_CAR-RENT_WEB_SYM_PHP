Symfony 3 Car-Rent Sample Demo PL
=================================

Info
----

Framework: Symfony 3.0.*
Language: Polish
Project type: Sample
Licence: MIT

Live Demo
-----------

URL: [nat.darkville.o12.pl](http://nat.darkville.o12.pl/)

Accounts:

Login|Password|Role
---|---|---
Kasia|kasia|USER
Ania|ania|USER
Stefan|stefan|USER
Mod|mod|MOD

Installation
------------
1. Install pure [Symfony 3](https://symfony.com/download)
2. Clone this repository
3. Configure your database in `app\config\parameters.yml`
4. Create schema by command `php bin/console doctrine:schema:update --force`
5. Fill database. Example:

#### cars
id|name|category_id|image|description|parameters|price
:---:|:---:|:---:|:---:|:---:|:---:|:---:
...|...|...|...|...|...|...
2|Honda Accord|2|2.jpg|(description text)|Gasoline;5;No|500.00
...|...|...|...|...|...|...

#### categories
id|name
:---:|:---:
1|SUV
2|Sedan
...|...

#### users
id|username|mail|password|roles
:---:|:---:|:---:|:---:|:---:
1|Jack|jack(at)example.com|jack123|ROLE_USER
2|Megan|megan(at)example.com|megan456|ROLE_MOD
...|...|...|...|...

**Tip:** You can create users by registration form and then give them right roles.

Roles
--------

Activity|ANON|USER|MOD
---|:---:|:---:|:---:
register            |+|-|-
login               |-|+|+
show cars           |+|+|+
show cars sorted    |+|+|+
show categories     |+|+|+
show car status     |+|+|+
show car details    |+|+|+
show opinions       |+|+|+
show orders         |-|+|+
order cars          |-|+|+
add opinions        |-|+|+
accept opinions     |-|-|+
remove opinions     |-|-|+

Credits
-------

Sample created by [TimsManter](http://timsmanter.net/) under MIT licence.