# Создание базы данных для WordPress

[Главная](https://www.wordpress-abc.ru/) » [Уроки WordPress](https://www.wordpress-abc.ru/uroki-wordpress) » Создание базы данных для WordPress

![Создание базы данных для WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2015/02/sozdanie-bazyi-dannyih-wordpress.jpg)

Здравствуйте Уважаемые читатели раздела «Уроки создания WordPress» блога WordPress-abc.ru. Тема урока: Создание базы данных для WordPress. Сегодня я расскажу, как  создать базу данных для блога WordPress в различных административных панелях управления на сервере хостинга.

Для начала, совсем немного теории о базе данных.

Содержание

- [Что такое база данных сайта](https://www.wordpress-abc.ru/uroki-wordpress/sozdanie-bazyi-dannyih-dlya-wordpress.html#i)
- [Адрес сервера базы данных](https://www.wordpress-abc.ru/uroki-wordpress/sozdanie-bazyi-dannyih-dlya-wordpress.html#i-2)
- [Создание базы данных для WordPress в панели ISPmanager](https://www.wordpress-abc.ru/uroki-wordpress/sozdanie-bazyi-dannyih-dlya-wordpress.html#__WordPress__ISPmanager)
- [Создание базы данных в панели DirectAdmin](https://www.wordpress-abc.ru/uroki-wordpress/sozdanie-bazyi-dannyih-dlya-wordpress.html#___DirectAdmin)
- [Создание базы данных в панели в CPanel](https://www.wordpress-abc.ru/uroki-wordpress/sozdanie-bazyi-dannyih-dlya-wordpress.html#___CPanel)
- Создание базы данных в панели в других панелях
  - [Итоги урока Создание базы данных для WordPress](https://www.wordpress-abc.ru/uroki-wordpress/sozdanie-bazyi-dannyih-dlya-wordpress.html#___WordPress)
- Полезные ссылки
  - [Другие Уроки WordPress](https://www.wordpress-abc.ru/uroki-wordpress/sozdanie-bazyi-dannyih-dlya-wordpress.html#_WordPress)

## Что такое база данных сайта

База данных это вся информация, которая есть на сайте, собранная в одном месте, объединенная в таблицы базы данных. То есть, все статьи, страницы, данные плагинов, данные виджетов хранятся в базе данных в виде отдельных таблиц. Сервер, где хранится база данных и на котором установлено  программное обеспечение для управления базой данных называется MySQL. Есть и другие сервера для БД, но обычно хостинги устанавливают именно это программное обеспечение для управления базами данных.

## Адрес сервера базы данных

Хостинг провайдер может установить сервер для базы данных у себя на сервере, в этом случае адрес сервера MySQL будет localhost. Но могут быть варианты. Например, хостинг MaкХост располагает свои сервера БД по адресам типа: vash_login.mysql.mchost.ru.

Я упоминаю про адреса базы данных, не для энциклопедических знаний, вам понадобится адрес вашего сервера MySQL при установки WordPress, на этапе инсталляции. Узнать адрес своего сервера базы данных вы можете в административной панели своего хостинга.

Теперь на практике рассмотрим, создание базы данных для WordPress.

> Кстати, версия MySQL должна быть выше 5.0.

## Создание базы данных для WordPress в панели ISPmanager

Авторизуйтесь в панели ISP вашего сервера. В левом, вертикальном меню найдите вкладку «Инструменты». Откройте пункт меню «Базы данных». На странице «Базы данных», жмете кнопку «Создать», в верхнем правом углу страницы.

[![Создание базы данных для WordPress в панели ISP](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/baza-dannyih-v-isp-paneli-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/baza-dannyih-v-isp-paneli-1.jpg)

[Читайте так же:  Хостинг для WordPress: параметры хостинга сайта Wordpress](https://www.wordpress-abc.ru/uroki-wordpress/hosting-dlya-wordpress.html)

Откроется форма для создания БД. Дайте базе данных

- Имя базы данных;
- Создаете пользователя (для безопасности лучше нового);
- Генерируете пароль базы данных.

[![база-данных-в-isp-панели-2](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/baza-dannyih-v-isp-paneli-2.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/baza-dannyih-v-isp-paneli-2.jpg)

Запоминаете пароль (посмотреть его будет нельзя, можно будет только поменять), сохраняет имя базы данных и имя пользователя.

Создаете базу данных.

[![база-данных-в-isp-панели-3](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/baza-dannyih-v-isp-paneli-3.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/baza-dannyih-v-isp-paneli-3.jpg)

База данных для WordPress создана, можно на нее взглянуть. На серверах управляется база данных из панели, которая называется phpmyadmin.

Ищем, в меню, ссылку phpmyadmin и переходим по ней. Для авторизации в панели phpmyadmin, нужны созданные имя пользователя и пароль. Войдя в панель phpmyadmin, видим, что база данных создана, но пока она пустая.

## Создание базы данных в панели DirectAdmin

Авторизуйтесь в панели DirectAdmin.

Откройте свой домен.

В меню панели (первая ее часть) ищите вкладку «Управление MySQL» . На вкладке, создаете базу данных для WordPress. База данных должна иметь: Имя базы, Имя пользователя и пароль доступа.

[Читайте так же:  WordPress плагин SumoMe, улучшаем юзабилити сайта](https://www.wordpress-abc.ru/plaginy/wordpress-plagin-sumome.html)

![Создание базы данных для WordPress в DirectAdmin](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/baza-dannyih-v-paneli-directadmin-1.jpg)

![база-данных-в-панели-directadmin-2](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/baza-dannyih-v-paneli-directadmin-2.jpg)

[![база-данных-в-панели-directadmin-3](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/baza-dannyih-v-paneli-directadmin-3.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/baza-dannyih-v-paneli-directadmin-3.jpg)

Все данные новой базы данных запоминаем. К этим записям добавляем адрес сервера MySQL.

Для контроля создания базы данных, со страницы меню панели переходим на вкладку «phpmyadmin» (она внизу). После авторизации, видим, что база данных создана, но она пустая.

## Создание базы данных в панели в CPanel

CPanel очень популярна на импортных серверах.

Никаких отличий, от создания базы в других панелях нет. Только пункты меню снабжены картинками и нужно пользователю, назначить полные привилегии для управления базой данных.

[![база-данных-в cPanel](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/baza-dannyih-v-cPane-3-shaga.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/baza-dannyih-v-cPane-3-shaga.jpg)

## Создание базы данных в панели в других панелях

Кроме стандартных панелей, многие хостинг компании разрабатывают свои административные панели.

Принцип создания базы данных в такой панели аналогичен. Главное, после создания базы данных для WP, чтобы база данных была реально создана и чтобы она была пустой.

[Читайте так же:  Визуальный редактор для виджетов Wordpress](https://www.wordpress-abc.ru/plaginy/vizualnyiy-redaktor-dlya-vidzhetov-wordpress.html)

Также вы должны иметь под рукой:

- Название базы – её имя (name);
- Пользователя, созданного для базы данных (user);
- Пароль именно, базы данных (password);
- Адрес размещения сервера MySQL (host).

В скобках я указал, как система WordPress обозначает эти данные в конфигурационном файле WordPress, который нужно будет заполнять при ее установке.

### Итоги урока Создание базы данных для WordPress

Теперь вы знаете. Как создать базу данных, для блога WordPress в разных панелях администрирования хостинга. Правда, также создаются базы данных для сайтов любой CMS платформы.

## Полезные ссылки

Сайт MySQL:  **http://www.mysql.com/**

Игорь Серов специально для сайта «[Как сделать сайт WordPress](https://www.wordpress-abc.ru/)»

### Другие Уроки WordPress

- [Что такое плагины WordPress](https://www.wordpress-abc.ru/uroki-wordpress/chto-takoe-plaginyi-wordpress-2.html)
- [Создаем меню WordPress: как создать меню WordPress](https://www.wordpress-abc.ru/uroki-wordpress/sozdaem-menyu-wordpress.html)
- [Как объединить два сайта WordPress](https://www.wordpress-abc.ru/uroki-wordpress/kak-obedinit-dva-sayta-wordpress.html)
- [Сайдбар и виджеты WordPress](https://www.wordpress-abc.ru/uroki-wordpress/saydbar-vidzhetyi-wordpress.html)
- [Первые настройки WordPress](https://www.wordpress-abc.ru/uroki-wordpress/pervyie-nastroyki-wordpress.html)
- [Домен для WordPress сайта](https://www.wordpress-abc.ru/uroki-wordpress/domen-dlya-wordpress-3.html)
- [Публикация статей в WordPress](https://www.wordpress-abc.ru/uroki-wordpress/publikatsiya-statey-v-wordpress.html)
- [Хостинг для WordPress: параметры хостинга сайта WordPress](https://www.wordpress-abc.ru/uroki-wordpress/hosting-dlya-wordpress.html)
- [Что такое тема WordPress](https://www.wordpress-abc.ru/uroki-wordpress/chto-takoe-tema-wordpress.html)
- [Установка и удаление плагина на WordPress](https://www.wordpress-abc.ru/uroki-wordpress/ustanovka-udalenie-plagina-na-wordpress.html)