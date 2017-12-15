# Установка WordPress на хостинг, создание базы MySQL, сайт на WP

[Главная](https://www.wordpress-abc.ru/) » [Установка WordPress](https://www.wordpress-abc.ru/ustanovka-wordpress) » Установка WordPress на хостинг, создание базы MySQL, сайт на WP

![Установка Wordpress на хостинг, создание базы MySQL](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Ustanovka-wordpress.jpg)

В статьи использованы скриншоты снятые с установки WordPress 3.5

Содержание

- [Вступление](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-na-xosting.html#i)
- [Требования WordPress к программному обеспечению хостинга](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-na-xosting.html#_WordPress)
- Установка WordPress на хостинг
  - [Скачать дистрибутив WordPress](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-na-xosting.html#_WordPress-3)
- [Создать базу MySQL на хостинге](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-na-xosting.html#_MySQL)
- [Редактировать (изменить) несколько файлов](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-na-xosting.html#i-2)
- Установка WordPress на хостинг через FTP-клиент
  - [FTP-клиент FileZilla](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-na-xosting.html#FTP-_FileZilla)
- [Окончание установки WordPress](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-na-xosting.html#_WordPress-4)
- Вывод
  - [Другие стати раздела: Установка WordPress](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-na-xosting.html#__WordPress)

## Вступление

Перед установкой и даже перед выбором WordPress в качестве рабочей CMS для своего сайта, нужно понимать, что [хостинг](https://www.wordpress-abc.ru/hosting/hosting-i-sayt-wordpress.html) должен иметь определенное программное обеспечение для поддержания стабильной работы WordPress.

## Требования WordPress к программному обеспечению хостинга

У CMS WordPress не завышенные требования по программному обеспечению хостинга и с гарантией можно сказать, что большинство хостингов  соответствуют требованиям WordPress. Для запуска WordPress рекомендуется чтобы хост поддерживал:

- PHP версии 5.6 или выше
- MySQL версии 5.6 или выше
- или OR MariaDB версии 10.0 или выше
- Рекомендовано, чтобы хостинг использовал HTTP сервер: Apache или Nginx, однако запустится и на любом другом с поддержкой PHP и MySQL.

*Такое программное обеспечение имеет любой современный хостинг. Первый вопрос решен.*

Следующее. Для установки WordPress на хостинг понадобятся два веб инструмента.

- Первый инструмент это текстовой редактор (например, Notepad++). Он нужен для правки файлов и пригодится в дальнейшей работе.
- Второй инструмент это клиент для соединения по FTP. Например, FTP-клиент FiltZilla или WinSCP.

*Если такие инструменты есть в вашем арсенале, то можно приступать к установке WordPress на свой хостинг.*

**Примечание:** Установить WordPress можно не только по стороннему FTP соединению, но и из файлового менеджера в административной панели хостинга, например из [через ISPmanager](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-cherez-ispmanager.html).

## Установка WordPress на хостинг

Установка WordPress на хостинг включает следующие этапы:

- Скачать дистрибутив WordPress;
- Создать базу MySQL на хостинге;
- Редактировать (изменить) несколько файлов;
- Разместить папки и файлы WordPress на хостинге;
- Закончить установку переходом в административную панель сайта.

### Скачать дистрибутив WordPress

**Совет:** Все расширения WordPress (шаблоны, плагины и сам дистрибутив) скачивайте с официальных сайтов WordPress : wordpress.org, или лучше **wordpress.ru**.

[Читайте так же:  Переадресация на сайте WordPress, 301 редирект](https://www.wordpress-abc.ru/plaginy/pereadresatsiya-na-sayte-wordpress.html)

В этом примере скачиваем дистрибутив WordPress с русскоязычного WordPress. Дистрибутив это  форма распространения системного программного обеспечения.

[![Установка WordPress на хостинг](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/1-300x181.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/1.png)Картинка устарела, но новая картинка почти такая же, только черная.

Скачиваем дистрибутив WordPress архивом, который, для закачки по FTP, нужно сразу распаковать архиватором на своем компьютере.

## Создать базу MySQL на хостинге

Любой сайт состоит из двух частей. Одна часть сайта это некоторое количество папок и файлов, которые хранятся на сервере хостинга в корневой папке сайта. Вторая часть сайта это база данных сайта, которая храниться сервере MySQL. Сервер MySQL, обычно, находится на сервере вашего хостинга. База данных сайта это сложно структурированная база данных, состоящая из таблиц с информацией. Желательно, для одного сайта создавать одну базу данных.

Для сайта WordPress так же нужна отдельная база данных.

- Для создания базы данных для сайта, авторизуйтесь и войдите в свою административную панель на хостинге.
- На панели найдите значок,  где есть надпись MySQL или «Базы данных».

[![база MySQL](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/2.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/2.png)

- Нажимаем на иконку. Открывается окно управления базами данных в котором нужно создать новую базу данных.

[![Кнопка созданя базы MySQL](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/3.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/3.png)

На разных хостингах интерфейс панели и надписи отличаются, но принцип понятен. Нужно создать базу данных, которая должна иметь три обязательных параметра:

- Имя базы данных;
- Имя пользователя базой данных;
- Пароль базы данных.

Также нужно знать имя сервера MySQL. Чаще всего сервер MySQL это localhost, но возможно и набор цифр или имя типа: ваш_Аккаунт.mysql.ваш_Хостинг.ru.

**Создаем базу данных.** Ищем кнопку  типа «Создать базу данных». Нажимаем ее, открывается окно с простой формой для заполнения.

[![форма базы данных](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/4-300x229.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/4.png)

[![база данных MySQL](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/5-300x213.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/5.png)

В зависимости от хостинга, имя базы данных и пользователь базы данных могут быть одинарными или двойными именами, разделенными префиксом. Первая часть двойного имени это ваш аккаунт на хостинге, вторую часть вам нужно заполнить самостоятельно. Вписывается любое имя латинскими буквами.

Пароль базы данных подбирается самостоятельно или, если есть на хостинге, автоматически. Не пугайтесь, если пароля сначала не видно, он будет показан после создания базы на следующей странице.

После заполнения формы, нажимаем «Создать». После создания базы, откроется форма, сообщающая, что база данных создана и будут показаны ваши данные.

[Читайте так же:  Как настроить DNS сервера на VDS, VPS сервере](https://www.wordpress-abc.ru/ustanovka-wordpress/kak-nastroit-dns-servera-na-vds-vps-servere.html)

Важно! Запомните все данные базы данных, они нужны на следующем этапе установки WordPress.

## Редактировать (изменить) несколько файлов

*Этот параграф несколько устарел и версии WordPress 4+ не требуют отдельного редактирования файла wp-config. Всё делается из окна браузера при установке WordPress.*

На этом этапе понадобиться текстовой редактор. Я использую Notepad++ или Sublime Text2. В распакованном архиве WordPress, ищем файл wp-config-sample.php. Его нужно переименовать в  файл wp-config.php. В редакторе Notepad++ открываем файл wp-config.php. Это файл конфигурации WordPress. При установке в этом файле прописывается начальная настройка WordPress, и прежде всего, это данные созданной ранее базы данных MySQL.

В открытом в Notepad++ файле wp-config.php ищем строки MySQL и вписываем свои данные базы данных.

[![файла wp-config.php](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/6-300x291.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/6.png)

Не забываем сохраняться в кодировке UTF-8 без BOM.

Важно! Не редактируйте файл wp-config.php в Блокноте Windows и тем более не используйте редакторы Word.

## Установка WordPress на хостинг через FTP-клиент

Возникает вопрос. А **куда собственно переносить файлы WordPress**? Вернее, в какую папку хостинга следует закачать весь каталог WordPress.

Обычно, закачивается WordPress в корневую папку хостинга. В зависимости от хостинга это каталоги *httpdocs* или *public_html* или папка с названием вашего домена. При установке WordPress в корневую паку сайта, сайт будет открываться при написании доменного имени в строке браузера: http:// example.com. Есть более простое правило определения корневой папки сайта: В корневой папке лежит файл index.php.

Если у вас уже есть информация в папке  (public_html), например, другой сайт, то в корневой папке нужно создать  отдельную папку с любым именем, например ABC. Далее, по FTP, закачать папки и файлы WordPress с локального компьютера в папку “ABC”. При таком размещении WordPress, ваш cайт будет открываться по адресу: http:// example.com /ABC.

*Куда закачивать файлы WordPress определили. Осталось определить, как. Для этого используем любой FTP-клиент. В моем примере это FileZilla.*

### FTP-клиент FileZilla

Для работы с FTP вам понадобятся учетные данные FTP клиента. Эти данные предоставляет хостинг-провайдер при покупке его услуг.

[Читайте так же:  Установка Wordpress через ISPmanager](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-cherez-ispmanager.html)

Открываем FileZilla. Во  вкладке «Файл»→»Менеджер сайтов» или в горизонтальной строке «Быстрого соединения» вводим свои данные для работы с FTP-клиентом. Нажимаем «Соединиться» или «Быстрое соединение».

[![FileZilla](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/7-300x71.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/7.png)

Если данные верны, справа на панели FileZilla откроется «дерево» вашего сайта. Слева колонка папок и файлов вашего компьютера.

Слева выделяете все файлы и папки WordPress (используйте кнопку Ctrl). Далее простым перетаскиванием переносите все папки WordPress в корневую папку сайта (httpdocs или public_html) своего сайта. Контролируется перекачка внизу экрана.

[![Установка WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/8a-300x174.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/8a.png)

Об удачной закачке, как и о проблемах, FileZilla сообщит.

## Окончание установки WordPress

Заканчиваем  установку переходом в инсталлятор WP. Для этого вводим в строку браузера:~~ http:// example.com/wp-admin/install.php~~. Для этого вводим в браузер домен сайта.

Важно! Некоторые хостинги не дадут вам доступ к сайту, пока вы не удалите  файл-заглушку index.html из корневого каталога сайта.

Видим результат, совсем не 5 минутной работы.

[![сайт WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/10a-277x300.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/10a.png)

Важно! Имя пользователя и пароль это ваши данные для входа в административную панель сайта. Их нужно запомнить, без них войти в административную панель сайта не получиться. Забыли пароль администратора, читаем статью: [Восстановить пароль администратора WordPress](https://www.wordpress-abc.ru/administrirovanie/vosstanovit-parol-administratora-wordpress.html).

[![Инсталяция wordpress-1](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Instalyatsiya-wordpress-1-400x264.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Instalyatsiya-wordpress-1.png)

На этом Установка WordPress на хостинг закончена!

## Вывод

В завершении замечу, что со временем установка Wordpress на хостинг несколько меняется в сторону упрощения, но суть установки изложенная в этой статье неизменна: скачать и распаковать последний дистибутив WordPress, [создать базу данных](https://www.wordpress-abc.ru/uroki-wordpress/sozdanie-bazyi-dannyih-dlya-wordpress.html) ([лучше отдельную](https://www.wordpress-abc.ru/hosting/kak-pomenyat-prefiks-bazyi-dannyih-wordpress.html)), залить дистрибутив в корень сайта.

Игорь Серов, специально для сайта «[Как создать сайт WordPress](https://www.wordpress-abc.ru/)»

### Другие стати раздела: Установка WordPress

- Записи не найдены