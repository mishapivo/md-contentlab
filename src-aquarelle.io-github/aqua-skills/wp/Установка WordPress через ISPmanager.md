# Установка WordPress через ISPmanager

[Главная](https://www.wordpress-abc.ru/) » [Установка WordPress](https://www.wordpress-abc.ru/ustanovka-wordpress) » Установка WordPress через ISPmanager

![Установка Wordpress через ISPmanager](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/ustanovka-wordpress-ISP.jpg)

Содержание

- [Подготовка к установке WordPress](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-cherez-ispmanager.html#__WordPress)
- [Установка WordPress через ISPmanager](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-cherez-ispmanager.html#_WordPress_ISPmanager)
- [Создание базы данных](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-cherez-ispmanager.html#i)
- [Редакция файла wp-config.php](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-cherez-ispmanager.html#_wp-configphp)
- Инсталляция WordPress
  - [Итоги](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-cherez-ispmanager.html#i-2)
  - [Другие стати раздела: Установка WordPress](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-cherez-ispmanager.html#__WordPress-2)

## Подготовка к установке WordPress

Прежде всего, скачайте с официального сайта русского WordPress последнюю стабильную версию WordPress. На скриншотах статьи ставим [WordPress 3.8](https://www.wordpress-abc.ru/administrirovanie/novaya-versiya-wordpress-3-8.html).

Распакуйте скачанный архив. Откройте папку WordPress и заново запакуйте все папки и файлы дистрибутива WordPress в ZIP архив. Начинается установка  WordPress через ISPmanager с закачки этого архива на ваш сервер или хостинг, арендованный у хостинг-провайдера.

Под сервером понимаем виртуальный выделенный [сервер (VDS/VPS)](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-na-vds-vps-server.html) с отдельным IPи правами root  супер администратора. Под хостингом понимаем часть выделенного сервера под общим IP с другими хостингами и правами на управление только корневой папки вашего домена.

Несмотря на принципиальные отличия сервера и хостинга, установка  WordPress через ISPmanager абсолютно идентична для обоих из них. Перед установкой вам нужно прикрепить ваш домен на хостинг. В ISPmanager прикрепление домена, называется «Создать домен». Будем считать, что домен создан, а с созданием домена автоматом была создана папка с именем домена (www/VASH_DOMEN). В эту папку и будет происходить, всем известная 5 минутная  установка  WordPress через ISPmanager.

Обращу внимание, после создания домена вам необходимо привязать домен к DNS серверам. Сделать это можно до или после установки WordPress. Если этого не сделать, то в браузере вы увидите следующее сообщение.

[![Установка WordPress через ISPmanager](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-5-400x256.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-5.png)

Кстати, проверить записи DNS можно on-line, одним из серверов:

До привязки:

[![Установка_wordpress_через_ISP-6](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-6-400x153.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-6.png)

После привязки:

[![Установка_wordpress_через_ISP-8](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-8-400x195.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-8.png)

## Установка WordPress через ISPmanager

- Авторизуйтесь в панели ISP;
- Открой вкладку «Файловый менеджер»;
- Нажмите кнопку «Загрузить»;
- Выберите на локальном компьютере zip архив WordPress, упакованный ранее;
- Нажмите кнопку «Извлечь». Система предложит извлечь файлы и папки архива WordPress в текущую папку;

[Читайте так же:  7 способов защитить сайт WordPress от копирования](https://www.wordpress-abc.ru/plaginy/5-sposobov-zashhitit-sayt-wordpress-ot-kopirovaniya.html)

[![Установка WordPress через ISPmanager ](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-1-400x168.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-1.png)

[![Установка_wordpress_через_ISP-2](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-2-400x158.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-2.png) [![Установка_wordpress_через_ISP-3](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-3-400x212.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-3.png)

Архив моментально распаковывается. Скорость установки  это существенное улучшение, чем установка WordPress через ISPmanager отличается от аналогичной установки по FTP. После извлечения, удалите ZIP архив WordPress.

[![Установка_wordpress_через_ISP-4](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-4-400x237.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-4.png)

## Создание базы данных

Для будущего сайта нужно создать базу данных. Желательно, поддерживать простую формулу: Один сайт — одна база данных. Правда, меняя префиксы баз данных, можно установить два сайта на одну базу данных.

[![Создать базу данных](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Sozdat-bazu-dannyih-400x280.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Sozdat-bazu-dannyih.png)

База данных должна иметь имя, имя пользователя, и пароль доступа. В ISP база данных создается на вкладке «Базы данных». В ее создании нет ничего сложного, достаточно заполнить форму во всплывшем модальном окне после нажатия кнопки «Создать» во вкладке «Базы данных».

## Редакция файла wp-config.php

Чтобы создать файл wp-config.php, переименуйте wp-config-sample.php. Получите файл  wp-config.php — основной файл необходимый для работы системы. Перед инсталляцией (последним шагом установки Worpress) нужно отредактировать  файл  wp-config.php, прописав в нем параметры созданной базы данных. Для этого выделите файл wp-config.php в файловом менеджере ISP, и откройте его,  нажав кнопку «Изменить». Параметры базы данных (имя, имя пользователя и пароль) введите в соответствующие строки файла.

[![Установка_wordpress_через_ISP-7](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-7-400x170.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-7.png)

В строке

введите имя сервера MySQL. Обычно это localhost, но могут быть варианты. Например, ряд цифр или что-то подобное (Аккаунт.mysql.Хостинг.ru). Сомневаетесь, обратитесь к провайдеру.

После редактирования не забывайте «Сохранить» файл  wp-config.php.

Примечание: Последние версии WordPress могут сами формировать файл wp-config.php, но не все хостинг- провайдеры это поддерживают.

[![Установка_wordpress_через_ISP](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP-400x149.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Ustanovka_wordpress_cherez_ISP.png)

## Инсталляция WordPress

Завершается **установка WordPress через ISPmanager**, тремя простыми шагами инсталляции. Для этого открываем страницу: http://VASH_DOMEN/wp-admin/install.php и проходим два окна инсталляции

![Инсталяция wordpress](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Instalyatsiya-wordpress-318x400.png)

[![Инсталяция wordpress-1](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Instalyatsiya-wordpress-1-400x264.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Instalyatsiya-wordpress-1.png)

В ISPmanager в корневой паке сайта создается файл index.html. Это, так называемая «Заглушка». Некоторые хостинги настроены на его удаление, после установки WordPress. Если его не удалить, то вместо сайта вы увидите картинку с надписью, что каталог не содержит информации.

[Читайте так же:  Перенос комментариев между постами без плагина](https://www.wordpress-abc.ru/plaginy/wordpress-bez-plugins/perenos-kommentariev-mezhdu-postami-bez-plagina.html)

### Итоги

- **Установка WordPress через ISPmanager** не вызывает сложных проблем;
- По скорости установки значительно превосходит аналогичную установку по FTP;
- Правда сама панель требует некоторого привыкания, но  это уже дело вкуса. Тем более что всегда есть возможность [установить WordPress по FTP](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-na-xosting.html), независимо от панели хостинга (сервера).

Игорь Серов, специально для сайта «[Как создать сайт WordPress](https://www.wordpress-abc.ru/)»

### Другие стати раздела: Установка WordPress

- Записи не найдены