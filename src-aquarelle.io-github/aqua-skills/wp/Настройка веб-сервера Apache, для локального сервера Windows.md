# Настройка веб-сервера Apache, для локального сервера Windows

[Главная](https://www.wordpress-abc.ru/) » [Хостинг](https://www.wordpress-abc.ru/hosting) » [Локальный сервер](https://www.wordpress-abc.ru/hosting/lokalnyiy-server) » Настройка веб-сервера Apache, для локального сервера Windows

![Настройка веб-сервера Apache, для локального сервера Windows](https://www.wordpress-abc.ru/wp-content/uploads/2017/01/nastroyka-veb-servera-Apache.jpg)

Содержание

- [Вступительная часть](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/nastrojka-veb-servera-apache-windows.html#i)
- [Подготовка к настройке веб-сервера Apache](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/nastrojka-veb-servera-apache-windows.html#__-_Apache)
- [Настройка веб-сервера Apache по шагам](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/nastrojka-veb-servera-apache-windows.html#_-_Apache)
- [Проверка работы файла httpd.php](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/nastrojka-veb-servera-apache-windows.html#__httpdphp)
- Вывод
  - [Еще статьи](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/nastrojka-veb-servera-apache-windows.html#i-3)

## Вступительная часть

Продолжаем собирать локальный сервер на своем компьютере, с осью Windows. После установки трех компонентов локального сервера AMP (Apache+MySQL+PHP) на свой компьютер, работающий под Windows, переходим к их настройке. В этой статье настроим веб-сервер, Apache.

## Подготовка к настройке веб-сервера Apache

Если вы делаете установку локального сервера без временных пауз, вам достаточно легко, будет вспомнить, куда вы установили компоненты сервера Apache; MySQL; PHP.

*Общая задача настроек Apache; MySQL; PHP это связать их воедино, указав в каждом из них, расположение других серверов. А также, нужно выставить наиболее приемлемые настройки параметров этих компонентов.*

Задача этой статьи, понять, где у сервера Apache, лежит «золотой ключик» настроек. Настройки можно менять в зависимости от встающих задач, ведь глобальная задача, не установить локальный сервер на локальный компьютер, а пользоваться им.

## Настройка веб-сервера Apache по шагам

Идем в директорию установки Apache. В прошлых статьях я ставил Apache в папки c:/www ([установка Apache MSI](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-apache-msi.html)) и c:/Apache24 (~~установка Apache без инсталлятора~~);

В папке c:/www/conf нам нужен файл конфигурации веб-сервера, httpd.php;

*Настройка веб-сервера Apache (редактирование файла) делаем в удобном редакторе Notepad++.*

**Примечание:** Термин раскомментировать (**uncomment**), означает открыть доступ к функционально строке файла для системы. По факту. Раскомментировать в файлах Apache, значит убрать в начале строке знак решетка (#).

1.

(включаем загрузку для модуля  mod_rewrite)

[![Настройка веб-сервера Apache включаем загрузку для модуля mod_rewrite](https://www.wordpress-abc.ru/wp-content/uploads/2017/01/1-448x171.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/01/1.jpg)включаем загрузку для модуля mod_rewrite

2.

```
LoadModule php5_module "C:/php/php5apache2_2.dll"

AddType application/x-httpd-php .php

PHPIniDir "c:/php/"

```

3.

[Читайте так же:  Установка Apache 2.4 binaries VC14 без инсталлятора](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-apache-2-4-bez-installyatora.html)

[![Порт 80 Apache](https://www.wordpress-abc.ru/wp-content/uploads/2017/01/2-448x155.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/01/2.jpg)

4.

[![DoccumentRoot](https://www.wordpress-abc.ru/wp-content/uploads/2017/01/3-448x159.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/01/3.jpg)

5

```
<Directory />

Options FollowSymLinks

AllowOverride None

</Directory>
```

Меняем [None] на команду [All]

[![поменять none на all](https://www.wordpress-abc.ru/wp-content/uploads/2017/01/41-448x110.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/01/41.jpg)

6.

[![Строка 322](https://www.wordpress-abc.ru/wp-content/uploads/2017/01/5-448x153.jpg)](https://local-site.ru/wp-content/uploads/2017/01/5.jpg)

7.

```
(816)#AddType text/html .shtml

(817)#AddOutputFilter INCLUDES .shtml
```

[![img](https://www.wordpress-abc.ru/wp-content/uploads/2017/01/6-448x102.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/01/6.jpg)

Дополняем их двумя строками:

```
AddType application/x-httpd-php-source .phps

AddType application/x-httpd-php .php
```

(тем самым, включаем SSL на Apache)

[![поддержка SSL](https://www.wordpress-abc.ru/wp-content/uploads/2017/01/6a-448x118.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/01/6a.jpg)

8.

9.

10.

## Проверка работы файла httpd.php

Для проверки правильности настройки идем через меню «Пуск» во все программы, далее Apache HTTP  файл «TestConfiguration». Если есть ошибки они отразятся на экране.

## Вывод

Настройка веб-сервера Apache завершена. В завершении замечу, что в файле httpd.php сервера Apache, все директории и блоки директорий снабжены подробными комментариями на английском языке. Для глубоко понимания настроек их нужно почитать.

Скачать файл httpd.php сервера Apache можно [тут](https://www.wordpress-abc.ru/wp-content/uploads/2017/07/configs.zip) (на сайте). Обратите внимание, что в нем другое место расположения Apache.

©www.wordpress-abc.ru

### Еще статьи

- [Как установить WordPress на XAMPP](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/kak-ustanovit-wordpress-na-xampp.html)
- [Веб-сервер Apache — что такое http Apache, для чего нужен, где скачать](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/veb-server-apache-2.html)
- [Установка PHP на локальный компьютер](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-php-na-lokalyj-kompyuter.html)
- [Как полностью удалить MySQL с локального компьютера с Windows](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/kak-udalit-mysql-s-lokalnogo-kompyutera.html)
- [Способы установки MySQL на локальный компьютер под Windows](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/sposoby-ustanovki-mysql-na-lokalnyj-kompyuter-pod-windows.html)