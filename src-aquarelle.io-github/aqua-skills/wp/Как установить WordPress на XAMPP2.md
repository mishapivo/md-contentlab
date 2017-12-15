# Как установить WordPress на XAMPP

[Главная](https://www.wordpress-abc.ru/) » [Хостинг](https://www.wordpress-abc.ru/hosting) » [Локальный сервер](https://www.wordpress-abc.ru/hosting/lokalnyiy-server) » Как установить WordPress на XAMPP

![установить WordPress на XAMPP](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/ustanovka-Wordpres-na-XAMPP.jpg)

Содержание

- [Вводная часть](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/kak-ustanovit-wordpress-na-xampp.html#i)
- [Что такое локальный сервер](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/kak-ustanovit-wordpress-na-xampp.html#i-2)
- [Готовые сборки локальных серверов](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/kak-ustanovit-wordpress-na-xampp.html#i-3)
- [Сервер XAMPP установка](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/kak-ustanovit-wordpress-na-xampp.html#_XAMPP)
- [Как запустить XAMPP](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/kak-ustanovit-wordpress-na-xampp.html#_XAMPP-2)
- [Как проверить запуск XAMPP](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/kak-ustanovit-wordpress-na-xampp.html#__XAMPP)
- Как установить WordPress на XAMPP по шагам
  - [Как создать базу данных на XAMPP](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/kak-ustanovit-wordpress-na-xampp.html#___XAMPP)
- Ставим WordPress на XAMPP
  - [Итог](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/kak-ustanovit-wordpress-na-xampp.html#i-4)
  - [Еще статьи](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/kak-ustanovit-wordpress-na-xampp.html#i-5)

## Вводная часть

Создание сайта дело не одного дня, и часто, для этих целей используют локальный сервер, установленный на домашний компьютер. Не будем останавливаться на преимуществах и минусах этого способа работы, дело вкуса и привычки. Есть факт, что можно создать сайт WordPress на локальном сервере размещенном на своём компьютере.

## Что такое локальный сервер

У меня есть возможность показывать скриншоты только операционной системы Windows, поэтому говорить буду только о локальном сервере на Win7.

Локальный сервер это сборка и взаимосвязанная настройка трех программных продуктов, нужных для веб-сайта:

- Сервер HTTPS. Обычно это Apache, реже Nignx.
- Сервер базы данных. Обычно используют MySQL, реже MiraBD.
- Интерпретатор PHP.

> Перечислен  минимальный набор программ, которые нужны для создания сайта на локальном сервере.

## Готовые сборки локальных серверов

Если вы используете заглавные буквы указанных программных продуктов и возглавите этот акроним Windows, то получите общепринятое название локального сервера для Windows: WAMP.

Логично, что сборку WAMP можно собрать самостоятельно, установив и настроив каждый продукт в отдельности. Вопрос,— зачем? Зачем мучиться со слабой сборкой WAMP сервера, если есть готовые локальные сервера с многофункциональными возможностями.

Готовых, популярных WAMP+ сборок около десятка. На русском языке единицы. Я работал с пол дюжиной, в том числе:

- **Denwer (Денвер)**. Русская сборка, авторы которой застряли в прошлом. Отсутствие развитие этого продукта, откровенное неудобство и проблемы переноса готового сайта, опускают этот сервер вниз списка. [Установка WordPress на Denwer](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-wordpress-na-denver.html#1).
- **Open Server**. Отличная русская сборка локального сервера с простым и понятным интерфейсом.
- **XAMPP.** Герой этого поста. Англоязычная очень удобная сборка, имеющая дополнительный облачный сервер.
- **AppServ**. Англоязычная, развитая сборка удобная в работе.
- **WAMPServer.** Авторы особо не заморачивались с названием, и взяли для своего названия акроним WAMP. Достойная англоговорящая сборка.

[Читайте так же:  Установка сервера MySQL 5.7.11 на Windows 7](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-servera-mysql-5-7-11-na-windows-7.html)

## Сервер XAMPP установка

Герой этого поста, сервер XAMPP. Не знаю, по каким причинам, но XAMPP удивительным образом заточен по WordPress. У него даже все внутренние инструкции написаны для WordPress.

Качаем XAMPP на родном сайте (https://www.apachefriends.org/ru/index.html). Берем версию с установщиком под ваш win (например, xampp-win32-5.6.30-0-VC11-installer).

Установка осуществляется от имени администратора через 7 окон установщика и не требует пояснений. Более интересен запуск XAMPP.

[![img](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/XAMPP-ustanovka-1-448x374.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/XAMPP-ustanovka-1.jpg)[![img](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/XAMPP-ustanovka-2-448x374.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/XAMPP-ustanovka-2.jpg)[![img](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/XAMPP-ustanovka-3-448x374.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/XAMPP-ustanovka-3.jpg)[![img](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/XAMPP-ustanovka-4-448x374.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/XAMPP-ustanovka-4.jpg)[![img](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/XAMPP-ustanovka-5-448x374.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/XAMPP-ustanovka-5.jpg)[![img](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/XAMPP-ustanovka-6-448x374.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/XAMPP-ustanovka-6.jpg)[![img](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/XAMPP-ustanovka-7-448x374.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/XAMPP-ustanovka-7.jpg)

## Как запустить XAMPP

Чтобы полностью запустить XAMPP, запускаем три программы:

- Apache. Для этого нужен свободный порт 80.
- MySQL. Порт 3036.
- FTP. Необязательно, запускается на порту 21.
- Почтовик Mercury запускать необязательно.

> Коробочная версия XAMPP настроена на запуск Apache на порту 80.

Запускаем XAMPP из Пуск–Меню;

Попробуем запустить Apache кнопкой Start. Если порт 80 занят, видим сообщение в красном цвете;

[![img](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/zapusk-XAMPP-2.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/zapusk-XAMPP-2.jpg)Запускаем XAMPP

Про освобождение порта 80, рекомендую почитать на форуме XAMPP, тут: https://community.apachefriends.org/f/viewtopic.php?f=22&t=69784&p=239058#p239059

> Разработчики XAMPP, не рекомендуют перестраивать XAMPP на запуск на другом порту, например 8080. Последний раз, я освободил 80 порт, отключением службы IIS.

[Читайте так же:  Веб-сервер Apache — что такое http Apache, для чего нужен, где скачать](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/veb-server-apache-2.html)

## Как проверить запуск XAMPP

Проверить правильный запуск XAMPP достаточно просто. В адрес браузера пишем [localhost], и браузер откроет панель локального сервера. Меню управления сервера вверху.

[![панель XAMPP](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/panel-XAMPP.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/panel-XAMPP.jpg)панель локального сервера XAMPP

## Как установить WordPress на XAMPP по шагам

Установка WordPress на XAMPP не от стандартной установки WordPress на платный хостинг. Для этого:

- Создаем базу данных для сайта;
- Заливам WordPress в catalog сайта;
- Шагаем по окнам установщика.

### Как создать базу данных на XAMPP

- Запустите XAMPP. Достаточно Apache и MySQL;
- Пишем localhost  в браузере и открываем панель XAMPP;
- Из меню открываем [phpmyadmin].

[![создать базу данных на XAMPP](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/phpmyadmin-XAMPP-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/phpmyadmin-XAMPP-1.jpg)

[![базf данных на XAMPP создана](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/phpmyadmin-XAMPP-2.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/phpmyadmin-XAMPP-2.jpg)

Интерфейс phpmyadmin стандартный, просто создаем базу данных:

- Кнопка «База данных»;
- Следующее окно. Графа «Создать базу данных» пишем её название, любое. Сравнение пропускаем. Кнопка «Создать».
- Этого достаточно, чтобы создать БД локального сайта.

Данные БД фиксируем.

- Название:  своё название;
- Имя пользователя: root;
- Пароль: пустой;
- Сервер БД: localhost.

## Ставим WordPress на XAMPP

Берем последнюю версию WordPress, https://ru.wordpress.org/. Архив распаковываем.

Содержимое каталога [wordpress] из архива полностью копируем в папку [xampp\htpdocs].

Меняем название каталога [wordpress]  на название созданной ранее базы данных.

В каталоге уже локального сайта ищем **файл wp-config-sample.php** и открываем его в Notepad++.

Пишем в этот файл данные созданной ранее базы данных. Файл сохраняем с новым названием **wp-config.php**.

Проверяем запуск XAMPP. В адресе браузера пишем **localhost/имя_catalogа_сайта**. Жмём [Enter].

Видим окна установки WordPress, которые проходим заполняя необходимые поля и формы.

[![установка wordpress на локальный сервер XAMPP шаг 1 ](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/ustanovka-wordpress-xampp-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/ustanovka-wordpress-xampp-1.jpg)установить WordPress на XAMPP шаг 1

[![сайт wordpress на локальном сервере XAMPP](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/fasad-ustanovlennogo-wordpress.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/fasad-ustanovlennogo-wordpress.jpg)Удалось установить WordPress на XAMPP

[![установка wordpress на локальный сервер XAMPP шаг 2 ](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/ustanovka-wordpress-xampp-2.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/ustanovka-wordpress-xampp-2.jpg)[![установка wordpress на локальный сервер XAMPP шаг 3 ](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/ustanovka-wordpress-xampp-3.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/ustanovka-wordpress-xampp-3.jpg)[![установка wordpress на локальный сервер XAMPP шаг 4 ](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/ustanovka-wordpress-xampp-4.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/ustanovka-wordpress-xampp-4.jpg)[![установка wordpress на локальный сервер XAMPP авторизация](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/ustanovka-wordpress-xampp-5.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2017/04/ustanovka-wordpress-xampp-5.jpg)

### Итог

Нам удалось установить WordPress на XAMPP. Теперь имеем, доступ в панель управления сайтом и доступ к самому сайту на своём компьютере. Это значить, что можно спокойно работать с сайтом локально и не зависеть от платных хостингах.

©www.wordpress-abc.ru

### Еще статьи

- Записи не найдены