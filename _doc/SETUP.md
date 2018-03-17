Having composer installed :

```
> composer selfupdate
> composer create-project --prefer-dist --stability=dev yiisoft/yii2-app-basic basic
> cd basic
> vendor\bin\codecept run
```

- create a DB
```
CREATE SCHEMA `db-001` DEFAULT CHARACTER SET utf8 ;
```

- update webapp db configuration in `config/db.php`
- create table **USER**

```
CREATE TABLE `db-001`.`user` (
  `id` VARCHAR(32) NOT NULL,
  `name` VARCHAR(45) NOT NULL,
  `email` VARCHAR(45) NOT NULL,
  PRIMARY KEY (`id`),
  UNIQUE INDEX `id_UNIQUE` (`id` ASC),
  UNIQUE INDEX `name_UNIQUE` (`name` ASC),
  UNIQUE INDEX `email_UNIQUE` (`email` ASC));
```

- create *User* model with Gii (first rename existing *User* model created by yii2-app-basic template)
- create *UserController* 
