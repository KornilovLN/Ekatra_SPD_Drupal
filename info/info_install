# Подготовка Drupal платформы для создания сайта

#### Некоторые источники
```
https://texterra.ru/blog/kak-sdelat-sayt-na-drupal-samostoyatelno.html
``` 

## Системные требования для Drupal 10

1. PHP

   <br>Минимальная версия: PHP 8.1
   <br>Рекомендуемая версия: PHP 8.2 или выше

2. База данных

   Drupal 10 поддерживает несколько СУБД:

>  MySQL/MariaDB:
   <br>MySQL: Версия 5.7 или выше
   <br>MariaDB: Версия 10.3 или выше
>  PostgreSQL:
   <br>Версия 10 или выше
>  SQLite:
   <br>Версия 3.26 или выше

3. Веб-сервер

   Drupal 10 может работать на разл. веб-серверах:

>  Apache: Версия 2.4.7 или выше
>  Nginx: Поддерживаются все текущие стабильные версии

4. Дополнительные компоненты и библиотеки

> Composer: Для управления зависимостями
> <br>Drush: утилита для управления Drupal
  <br>(рекомендуется, но не обязательна)

5. Расширения PHP

   Для работы Drupal 10 необходимы следующие расширения PHP:
```
    ctype
    curl
    dom
    fileinfo
    filter
    gd
    hash
    intl
    json
    mbstring
    openssl
    pdo
    session
    SimpleXML
    sodium
    tokenizer
    xml
    xmlwriter
    yaml
    zip
```

6. Рекомендуемая конфигурация

   Для оптимальной производительности и безопасности рекомендуется
   <br>использовать следующие версии и конфигурации:
```
    PHP: 8.2
    MySQL: 8.0 (или MariaDB 10.5)
    Apache: 2.4.x (с поддержкой mod_rewrite)
    Nginx: Последняя стабильная версия
    Composer: Последняя версия
    Drush: Последняя стабильная версия
```

7. Пример настройки окружения

   Если вы используете Apache и MySQL,
   <br>вот пример конфигурации:

   _**Apache**_           Включите модуль mod_rewrite:

```
bash

sudo a2enmod rewrite
sudo systemctl restart apache2 
```

  _**PHP**_               Установите необходимые расширения:
```
sudo apt-get install php8.2 php8.2-cli php8.2-fpm php8.2-mysql \
  php8.2-gd php8.2-xml php8.2-mbstring php8.2-curl php8.2-zip \
  php8.2-intl php8.2-soap
```

  _**MySQL**_             Установите MySQL и создайте базу данных:

```
sudo apt-get install mysql-server
sudo mysql_secure_installation
mysql -u root -p
CREATE DATABASE drupal;
CREATE USER 'drupaluser'@'localhost' IDENTIFIED BY 'password';
GRANT ALL PRIVILEGES ON drupal.* TO 'drupaluser'@'localhost';
FLUSH PRIVILEGES;
EXIT;
```

  _**Composer**_          Установите Composer глобально:

```
curl -sS https://getcomposer.org/installer | php
sudo mv composer.phar /usr/local/bin/composer
```



