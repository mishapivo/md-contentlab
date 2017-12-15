# Способы установки MySQL на локальный компьютер под Windows

[Главная](https://www.wordpress-abc.ru/) » [Хостинг](https://www.wordpress-abc.ru/hosting) » [Локальный сервер](https://www.wordpress-abc.ru/hosting/lokalnyiy-server) » Способы установки MySQL на локальный компьютер под Windows

![img](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/mysql-5-7-1-1.jpg)

Содержание

- [Вступление](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/sposoby-ustanovki-mysql-na-lokalnyj-kompyuter-pod-windows.html#i)
- [Схема присвоения версий MySQL](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/sposoby-ustanovki-mysql-na-lokalnyj-kompyuter-pod-windows.html#__MySQL)
- [GA и RA релизы MySQL](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/sposoby-ustanovki-mysql-na-lokalnyj-kompyuter-pod-windows.html#GA_RA_MySQL)
- [Способы установки MySQL на локальный компьютер -инсталлятор и автономная версия](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/sposoby-ustanovki-mysql-na-lokalnyj-kompyuter-pod-windows.html#_MySQL)
- Набор MySQL
  - [Выводы](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/sposoby-ustanovki-mysql-na-lokalnyj-kompyuter-pod-windows.html#i-2)

## Вступление

Здравствуйте! Для самостоятельно сборки локального сервера (хостинга) на своем компьютере необходимы, как минимум, три основные составляющие программы: MySQL, PHP и веб-сервер, к примеру, Apache. В статьях этой серии (локальный сервер), я покажу, все этапы сборки локального сервера, но без понимания общего процесса не обойтись без дополнительных информационных статей. Здесь, я познакомлю вас с системой управления базой данных MySQL, которая теперь принадлежит Aracle. Разберемся с версиями MySQL, существующими дистрибутивами и посмотрим способы установки MySQL на локальный компьютер под Windows.

Для начала стоит отметить, что установка MySQL на локальную машину, нужна не только для сборки сервера, но и для других программных работ.

[![mysql-5-7](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/mysql-5-7.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/mysql-5-7.jpg)

[![img](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/mysql-5-7-command-line.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/mysql-5-7-command-line.jpg)

## Схема присвоения версий MySQL

Как и любой серьезный программный продукт, версии MySQL имеют специальную маркировку. Посмотрим на неё.

**Последняя версия, MySQL 5.7.11. Что это значит?**

- Первая цифра [5] обозначает номер основной версии. Также, одинаковая версия разных дистрибутивов, означает единый формат файла.
- Вторая цифра [7] обозначает уровень очередного выпуска. Первая и вторая цифры вместе это серийный номер релиза.
- Третья цифра [11] это номер версии в пределах выпуска. Чем больше последняя цифра, тем новее версия MySQL.

## GA и RA релизы MySQL

Все выпускаемые версии MySQL делят на два типа релизов. «Сырой» релиз, который еще дорабатывается и обкатывается программистами, называют RA релизы. Их использовать не нужно. Нам более интересны, релизы общей доступности, RA релизы.

## Способы установки MySQL на локальный компьютер -инсталлятор и автономная версия

Инсталлятор, или бинарная версия это небольшая программа, которая после установки, сама качает нужные программы MySQL. Важно понимать, инсталлятор работает, только на компьютерах, подключенных к Интернет. Формат инсталлятора: msi. Есть два варианта инсталлятора: bin-32 и bin-64.

[Читайте так же:  7 способов защитить сайт WordPress от копирования](https://www.wordpress-abc.ru/plaginy/5-sposobov-zashhitit-sayt-wordpress-ot-kopirovaniya.html)

[![MySQL Installer фото](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/MySQL-Installer-photo.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/MySQL-Installer-photo.jpg)

Автономная версия MySQL, в теории должна устанавливаться с переносных устройств и для такой установки не нужно подключение компьютера к сети. Формат автономной версии: ZIP архив.

**На автономной версии стоит остановиться подробнее.**

Общей автономной версии MySQL (дистрибутива исходного кода) в бесплатном варианте, не существует, Однако, возможность скачать отдельные части MySQL в ZIP архивах. Вот адрес, [http://dev.mysql.com/downloads/windows/](http://dev.mysql.com/downloads/windows/)

## Набор MySQL

MySQL предоставляет вам набор инструментов для разработки и управления важных бизнес-приложений на Windows. В полный бесплатный комплект, который называют (Developer Default) входят следующие программы.

- **Connectors:** набор для подключения драйвера, чтобы  использовать MySQL с приложениями и инструментами.
- **Workbench:** Визуальный инструмент для администрирования баз данных и разработчики различных  интегрированных инструментов в среде проектирования баз данных, администрирования, разработки SQL и миграции базы данных.
- **для Excel:** Позволяет пользователям импортировать, экспортировать и редактировать данные MySQL с помощью Microsoft Excel.
- **Notifier:** Позволяет разработчикам и администраторам контролировать, запускать и останавливать работу системы MySQL.
- **для Visual Studio:** Интегрирует MySQL со студией Visual Studio Windows.

Все упомянутые части системы доступны с инсталлятора MySQL Installer. Релиз инсталлятора правильно обозначается так: Инсталлятор (MySQL Installer) mysql-installer-web-community-5.7.11.0.msi

### Выводы

> Не будем изобретать велосипед, для удобства и начального знакомства вполне достаточно использовать инсталлятор MySQL Installer.

[![MySQL Installer](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/MySQL-Installer.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/MySQL-Installer.jpg)

В завершении замечу, наиболее полный набор MySQL это коммерческая версия MySQL Enterprise Edition.

Это все способы установки MySQL на локальный компьютер.

©www.wordpress-abc.ru

### Еще статьи по теме

- [Как установить WordPress на XAMPP](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/kak-ustanovit-wordpress-na-xampp.html)
- [Установка Apache MSI: пошаговая установка Apache](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-apache-msi.html)
- [Установка сервера MySQL 5.7.11 на Windows 7](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html)
- [Способы установки MySQL на локальный компьютер под Windows](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/sposoby-ustanovki-mysql-na-lokalnyj-kompyuter-pod-windows.html)
- [Установка Apache 2.4 binaries VC14 без инсталлятора](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-apache-2-4-bez-installyatora.html)