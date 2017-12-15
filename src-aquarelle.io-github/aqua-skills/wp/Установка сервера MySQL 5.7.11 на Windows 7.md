# Установка сервера MySQL 5.7.11 на Windows 7

[Главная](https://www.wordpress-abc.ru/) » [Хостинг](https://www.wordpress-abc.ru/hosting) » [Локальный сервер](https://www.wordpress-abc.ru/hosting/lokalnyiy-server) » Установка сервера MySQL 5.7.11 на Windows 7

![установка сервера MySQL 5.7.11 на Windows 7](https://www.wordpress-abc.ru/wp-content/uploads/2017/06/ustanovka-servera-MySQL-5.7.11-na-OS-Windows-7.jpg)

Содержание

- [Вступление](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html#i)
- [Зачем нужна отдельная установка сервера MySQL](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html#___MySQL)
- [Что такое MySQL](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html#_MySQL)
- Установка сервера MySQL 5.7.11 на Windows 7 поэтапная инструкция
  - [Скачать MySQL 5.7.11 для Windows](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html#_MySQL_5711_Windows)
  - [Запуск инсталлятора](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html#i-2)
  - [Побочная установка программных продуктов](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html#i-3)
  - [License Agreement](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html#License_Agreement)
  - [Choosing a Setap Type](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html#Choosing_a_Setap_Type)
  - [Installation](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html#Installation)
  - [Product Configuration](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html#Product_Configuration)
  - [Type and Networking](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html#Type_and_Networking)
  - [Account and Roles](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html#Account_and_Roles)
  - [Windows Server](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html#Windows_Server)
  - [Установка завершена](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html#i-4)
- [Запуск сервера MySQL](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html#_MySQL-2)

## Вступление

Обращу внимание, в этой статье я ставлю, только MySQL Server (сервер базы данных) без визуальных «плюшек», MySQL Workbench, Connectors и т.д.

## Зачем нужна отдельная установка сервера MySQL

Зачем нужна отдельная установка сервера? Например, для обучения работе с базами данных через «черный экран» командной строки. Или чтобы изучить команды SQL языка и «в прямом эфире» увидеть свои ошибки и поупражняться. Или для самостоятельной сборки локального сервера. Не важно, зачем это нужно, важно, что это можно сделать.

## Что такое MySQL

Прежде чем заняться [установкой сервера MySQL](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/sposoby-ustanovki-mysql-na-lokalnyj-kompyuter-pod-windows.html) 5.7.11 на Windows 7 вспомним, что такое MySQL, зачем это нужно. Если вы в курсе, смело пропускайте первую, вступительную, часть.

Данный сайт посвящен созданию и разработке локальных сайтов, на всевозможных локальных серверах. В самом простом исполнении, вернее в самой простой сборке, локальный сервер это сборка трех компонентов: веб-сервер, система управления базами данных и интерпретированный динамический язык программирования. Данная сборка ставится под определенную операционную систему, которая стоит на вашем компьютере.

В этой серии статей, мы не ищем легких путей и не используем готовые сборки локальных серверов, можно называть, локальных хостингов. В этой серии, мы настойчиво собираем локальный хостинг, самостоятельно из отдельных программных продуктов.

Одной из частей, локального сервера является СУБД (система управления базами данных). Для разработки и создания сайтов, вполне достаточно установить бесплатную СУБД MySQL компании Aracle. На март 2016 года актуальна версия MySQL 5.7.11.

[Читайте так же:  Установка Wordpress через ISPmanager](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-cherez-ispmanager.html)

## Установка сервера MySQL 5.7.11 на Windows 7 поэтапная инструкция

1.

### Скачать MySQL 5.7.11 для Windows

Идем на официальный сайт продукта (**http://www.mysql.com/downloads/**) и страницу скачивания бесплатных компонентов (**http://dev.mysql.com/downloads/**).

 

[![скачать-server-mysql-5_7_11-photo-6](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/skachat-server-mysql-5_7_11-photo-6.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/skachat-server-mysql-5_7_11-photo-6.jpg)Идем на вкладку MySQL Community Edition

[![скачать-server-mysql-5_7_11-photo-5](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/skachat-server-mysql-5_7_11-photo-5.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/skachat-server-mysql-5_7_11-photo-5.jpg)Выбираем downloads community server

При скачивании внимательно выбираем инсталлятор не путая тип системы компьютера bit-32 и bit-64 Windows 7. Хотя 32 битная программа будет работать на 64-битном процессоре.

[![скачать-server-mysql-5_7_11-photo-1](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/skachat-server-mysql-5_7_11-photo-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/skachat-server-mysql-5_7_11-photo-1.jpg)Для скачивания выбираем MySQL Installer MSI

Для удобства из способов установки MySQL берем не ZIP архив, а MSI Installer. Это автоматический установщик, который через сеть закачает выбранные программные продукты. Недостаток файла – работает только на машинах подключенных к Интернет, компенсируется простотой установки.

[![скачать-server-mysql-5_7_11-photo-2](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/skachat-server-mysql-5_7_11-photo-2.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/skachat-server-mysql-5_7_11-photo-2.jpg)

[![Для скачивания MySQL можно нерегистрироваться](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/skachat-server-mysql-5_7_11-photo-3.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/skachat-server-mysql-5_7_11-photo-3.jpg)Для скачивания MySQL можно нерегистрироваться

Напомню, посмотреть тип системы своей машины можно в меню Пуск→Компьютер→Свойства→Тип системы.

[![скачать-server-mysql-5_7_11-photo-7](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/skachat-server-mysql-5_7_11-photo-7.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/skachat-server-mysql-5_7_11-photo-7.jpg)Проверка типа процессора на компьютере

2.

### Запуск инсталлятора

Скачанный exe файл проверяем на вирусы, своей антивирусной программой. Если файл брали на официальном сайте он гарантированно безопасен.

[![установить-server-mysql-5_7_11-photo-1](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-1.jpg)Запускаем инсталлятор MySQL

3.

### Побочная установка программных продуктов

Для установки сервера MySQL на компьютере должны быть установлены две обязательные программы:

- .NET Framework 4
- Visual Studio C++

По умолчанию Windows 7 уже укомплектован этими программами, правда версии могут быть поменьше.

При запуске инсталлятора MySQL он сообщит о необходимости установить нужные программные продукты. На сколько я помню, инсталлятор подкачает нужные программы. Если нет установите их самостоятельно. В этом нет ничего сложного, но можно почитать у меня:

- Установить .NET Framework 4
- Установить Visual Studio C++

4.

### License Agreement

Продолжаем установку MySQL. Окно License Agreement. Это стандартное подписание лицензии.

[![установить-server-mysql-5_7_11-photo-2](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-2.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-2.jpg)установка сервера MySQL 5.7.11 на Windows 7 соглашение с лицензией

5.

### Choosing a Setap Type

Именно на этом этапе, выбираем тип установки, вернее, устанавливаемый комплект MySQL.

[![установить-server-mysql-5_7_11-photo-3](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-3.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-3.jpg)

- Developer Default (MySQL Server, MySQL Workbench, Connectors в комплекте)
- **Server Only** – выбираем и ставим его, только сервер.
- Client Only
- Full (MySQL Server, MySQL Workbench, Connectors на выбор)
- Custom

> Если вы четко понимаете, что делаете, можно выбрать, Custom и в наборе программных продуктов, выбрать нужную комплектацию.

*По умолчанию СУБД будет установлена в папку: C:\Program Files\MySQL\MySQL5.7*

Еще раз поясню, почему вам может пригодиться, установка Server Only. Например, вы на своем компьютере не используете Visual Studio или, изучаете язык SQL и хотите изнутри понять, как работать с базами данных из командной строки, а не «играть» в визуальные картинки.

[Читайте так же:  Хостинг и сайт WordPress: выбор хостинга для сайта](https://www.wordpress-abc.ru/hosting/hosting-i-sayt-wordpress.html)

6.

### Installation

[![установить-server-mysql-5_7_11-photo-4](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-4.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-4.jpg)Installation server mysql 5.7.11

[![установить-server-mysql-5_7_11-photo-5](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-5.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-5.jpg)[![установить-server-mysql-5_7_11-photo-6](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-6.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-6.jpg)

7.

### Product Configuration

[![установить-server-mysql-5_7_11-photo-7](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-7.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-7.jpg)Устанавливаем конфигурацию MySQL

8.

### Type and Networking

[![установить-server-mysql-5_7_11-photo-8](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-8.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-8.jpg)Type and Networking MySQL 5.7.11

На локальной машине MySQL поддерживает порт TCP/IP- ставим галочку;

Обратите внимание: Если поставить галочку в строке: *Open freewall port for network access* (открытый порт брандмауэра для доступа к сети), то не нужно будет делать дополнительный разрешительных настроек в брандмауэре Windows 7.

9.

### Account and Roles

[![установить-server-mysql-5_7_11-photo-9](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-9.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-9.jpg)Задаем пароль MySQL

Здесь нам нужно задать пароль для работы в MySQL. Не будем нарушать традиций и ставим пароль: **root**. Кстати, без установки пароля на следующую страницу не попасть.

[![установить-server-mysql-5_7_11-photo-10](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-10.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-10.jpg)Задаем root пароль MySQL

10.

### Windows Server

Это окно простых настроек запуска MySQL. Если нужно, чтобы сервер запускался с запуском машины, то выделяете чекбокс, как на фото. Если хотите запускать его по необходимости, чекбокс не выделяете (лучше галочку поставить).

[![установить-server-mysql-5_7_11-photo-11](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-11.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-11.jpg)Конфигурация MySQL для Windows server

Здесь тормозим: Смотрим на чекбокс: Show advanced options (показать дополнительные функции).

11.

На следующей странице сервис наполнится конфигурацией, о чем сообщит зелеными галочками.

[![установить-server-mysql-5_7_11-photo-12](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-12.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-12.jpg)

[![установить-server-mysql-5_7_11-photo-13](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-13.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-13.jpg)

12.

### Установка завершена

Всё! Установка сервера MySQL 5.7.11 на ОС Windows 7, завершена. Можно сделать копию входа в буфер обмена и положить на рабочий стол.

[![установить-server-mysql-5_7_11-photo-15](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-15.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/ustanovit-server-mysql-5_7_11-photo-15.jpg)установка сервера MySQL 5.7.11 на Windows 7 завершена

## Запуск сервера MySQL

Установка сервера MySQL 5.7.11 на Windows 7 завершена. Проверяем правильность установки и запускаем сервер MySQL.

- Идем в меню Пуск;

[![img](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/zapustit-server-mysql-5_7_11-photo-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/zapustit-server-mysql-5_7_11-photo-1.jpg)

- Жмем на иконку запуска сервера: MySQL Command Line Client – Unicode. Он  там появится, если вы поставили галочку в пункте (10 Windows Server), в чекбоксе: Start the MySQL Server at System Startup.
- Откроется «черное окно» приложения: MySQL5.7 Command Line Client.
- Вводим пароль: **root** и работаем с СУБД из окон MySQL5.7 Command Line Client.

[![запустить-server-mysql-5_7_11-photo-7](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/zapustit-server-mysql-5_7_11-photo-7.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/zapustit-server-mysql-5_7_11-photo-7.jpg)

Пробуем первую команду: знак вопроса [?] или [help]. Сервер покажет элементарные служебные команды.

[![запустить-server-mysql-5_7_11-photo-8](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/zapustit-server-mysql-5_7_11-photo-8.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/zapustit-server-mysql-5_7_11-photo-8.jpg)

На самом деле, экран будет «черный».

[![запустить-server-mysql-5_7_11](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/zapustit-server-mysql-5_7_11.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/zapustit-server-mysql-5_7_11.jpg)

©www.wordpress-abc.ru

### Другие статьи раздела: Локальный сервер 

- [Установка Apache MSI: пошаговая установка Apache](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-apache-msi.html)
- [Настройка веб-сервера Apache, для локального сервера Windows](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/nastrojka-veb-servera-apache-windows.html)
- [7+ WAMP платформ для разработки локального сайта на Windows](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/7-wamp-platform-dlya-razrabotki.html)
- [Как полностью удалить MySQL с локального компьютера с Windows](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/kak-udalit-mysql-s-lokalnogo-kompyutera.html)
- [Установка сервера MySQL 5.7.11 на Windows 7](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html)