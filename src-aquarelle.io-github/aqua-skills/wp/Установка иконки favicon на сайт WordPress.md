# Установка иконки favicon на сайт WordPress

[Главная](https://www.wordpress-abc.ru/) » [Плагины](https://www.wordpress-abc.ru/plaginy) » Установка иконки favicon на сайт WordPress

![Установка иконки favicon на сайт WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/add-favicon-wordpress.png)

Неразрывной  спутницей адреса сайта является картинка расположенная рядом  с ним. Это иконка сайта или favicon  (favorites icon). Видна иконка только в адресной строке открытой вкладки и при добавлении сайта в закладки браузера. Отсутствие иконки сайта делает его не отличимым от других сайтов особенно в закладках браузера.  А ведь заметная иконка сайта это дополнительный инструмент продвижения сайта.

Оригинальная и выделяющаяся иконка сайта запоминается лучше названия. Отличная от других иконка сайта  будут стимулировать ваших посетителей чаще к вам возвращаться. В этой статье я покажу, как установить свою индивидуальную иконку сайта WordPress.

Для установки  иконки на сайт WordPress нужно сделать несколько шагов:

- Сделать  иконку (Favicon) на генераторе Favicon;
- Загрузить Favicon на сервер хостинга в каталог сайта;
- Написать код с атрибутом rel и явным указанием на размещение Favicon;
- Вставить код в шаблон сайта.

Содержание

- [Как сделать Favicon для сайта WordPress](https://www.wordpress-abc.ru/plaginy/ustanovka-ikonki-favicon-na-sajt-wordpress.html#_Favicon__WordPress)
- [FAVICON GENERATOR & GALLERY](https://www.wordpress-abc.ru/plaginy/ustanovka-ikonki-favicon-na-sajt-wordpress.html#FAVICON_GENERATOR_GALLERY)
- [Favicon готов можно загружать его на сайт WordPress](https://www.wordpress-abc.ru/plaginy/ustanovka-ikonki-favicon-na-sajt-wordpress.html#Favicon____WordPress)
- [Загружаем новый Favicon в каталог сайта](https://www.wordpress-abc.ru/plaginy/ustanovka-ikonki-favicon-na-sajt-wordpress.html#_Favicon)
- [Остается последнее вставить прописанный код в шаблон сайта](https://www.wordpress-abc.ru/plaginy/ustanovka-ikonki-favicon-na-sajt-wordpress.html#i)
- [Еще один вариант добавить одинаковый  Favicon на сам сайт и на административную панель](https://www.wordpress-abc.ru/plaginy/ustanovka-ikonki-favicon-na-sajt-wordpress.html#___Favicon)

### Как сделать Favicon для сайта WordPress

Для иконки сайта WordPress нужна картинка размером 16×16 или 32×32 пикселя, лучше в формате favicon.ico.Вообще говоря, если в шаблоне, при помощи кода, указывать явное размещение иконки в каталоге сайта, то формат Favicona может быть отличным от [.ico] .

Считается, что некоторые современные браузеры могут самостоятельно  находить картинку в формате favicon.ico в корневом каталоге сайта и использовать ее как иконку сайта. Считаю ,что нужно вставлять код в шаблон сайта и  указать браузеру явный путь к иконке favicon, а не надеятся на «милость» браузеров.

[Читайте так же:  Плагин Admin columns: выводим дату регистрации пользователей WordPress и полностью контролируем настройку административной панели WordPress](https://www.wordpress-abc.ru/plaginy/plagin-admin-columns-vyivodim-datu-registratsii-polzovateley.html)

Для изготовления «фавикона» существует масса **online инструментов**. Предложу два из них. Я пользуюсь ими  давно, они стабильны и элементарны в своем исполнении.

### FAVICON GENERATOR & GALLERY

**![favicon-na-wordpress-01](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/favicon-na-wordpress-01-300x132.png)**

[![favicon-na-wordpress-02](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/favicon-na-wordpress-02-300x250.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/favicon-na-wordpress-02.png)

Dynamicdrive

[![favicon-na-wordpress-08](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/favicon-na-wordpress-08-300x197.png)](http://wordpress-abc.ru/plaginy/ustanovka-ikonki-favicon-na-sajt-wordpress.html/attachment/favicon-na-wordpress-08)

Чтобы сделать Favicon, нужно сначала указать нужный размер Favicona, загрузить в генератор любое изображение со своего компьютера и нажать изготовление favicona. Favicon генерируется за секунды, после чего его можно скачать опять на компьютер. Генерируются иконки с именем Favicon.ico.

### Favicon готов можно загружать его на сайт WordPress

Сначала попробуем найти в корневом каталоге сайта  ранее установленный  Favicon. **Favicon сайта может располагаться в двух основных местах каталога**.

- Первое место расположения Favicon это корень сайта, непосредственно папка [httpdocs] или [publ_html].
- При установке стороннего шаблона WordPress Favicon шаблона может размещаться в папке: /themes/НАЗВАНИЕ_ТЕМЫ_WP/images.

Проверяем эти два адреса. Если находим старый Favicon его удаляем или переименовываем.

### Загружаем новый Favicon в каталог сайта

Для работы с файлами сайта я как всегда пользуюсь FTP клиентом FileZilla.

Загрузить Favicon сайта можно в любую папку каталога, а потом прописать место его нахождения в коде. Но наиболее разумны два места загрузки Favicona.

Первое место это непосредственно  корневая папка сайта (папка [httpdocs] или [publ_html]). Второе место это папка [image] в рабочей теме вашего сайта. При втором размещении Favicon нужно будет менять каждый раз при смене темы (шаблона) сайта.

[![favicon-na-wordpress-03](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/favicon-na-wordpress-03-300x80.png)](http://wordpress-abc.ru/plaginy/ustanovka-ikonki-favicon-na-sajt-wordpress.html/attachment/favicon-na-wordpress-03)

После размещения Favicona в каталоге сайта понадобятся следующие коды

При размещении Favicona в корне сайта нужен такой код:

При размещении Favicona в теме сайта нужен такой код:

Этот  код можно использовать, если вы хотите сделать отдельную иконку для какого нибудь внутреннего  плагина WordPress.

В этих кодах можно изменить название и формат favicon,который вы загрузили в каталог.

[Читайте так же:  Что такое каталог Яндекс, адрес каталога, как попасть в каталог Яндекс](https://www.wordpress-abc.ru/seo-nachinayushhim/chto-takoe-katalog-yandeks-adres-kataloga-kak-popast-v-katalog-yandeks.html)

### Остается последнее вставить прописанный код в шаблон сайта

Авторизуемся в административной панели сайта. В консоли, слева, в вертикальном меню выбираем: Внешний вид →Редактор.

[![favicon-na-wordpress-04](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/favicon-na-wordpress-04-300x193.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/favicon-na-wordpress-04.png)

В открывшемся редакторе справа ищем и выбираем шаблон header.php. На странице header.php вставляем написанные коды <link rel=» внутрь элемента <head>,после всех уже стоящих кодов <link rel=»

[![favicon-na-wordpress-05](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/favicon-na-wordpress-05-300x254.png)](http://wordpress-abc.ru/plaginy/ustanovka-ikonki-favicon-na-sajt-wordpress.html/attachment/favicon-na-wordpress-05)

**Не забываем сохраняться.** Открываем сайт в браузере. Через несколько секунд появляется ваш favicon  рядом  с названием сайта. Было:

[![favicon-na-wordpress-06](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/favicon-na-wordpress-06-300x95.png)](http://wordpress-abc.ru/plaginy/ustanovka-ikonki-favicon-na-sajt-wordpress.html/attachment/favicon-na-wordpress-06)

  Стало:

[![favicon-wp](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/favicon-wp-300x151.png)](http://wordpress-abc.ru/plaginy/ustanovka-ikonki-favicon-na-sajt-wordpress.html/attachment/favicon-wp)

Как видно на фото в адресной строке иконка сайта не меняется. Меняется только иконка в закладках и в окне вкладки. Работа по размещению своего favicon  (favorites icon), иконки сайта завершены. **В итогах статьи отмечу:**

- Следите за совпадением названия и расширения favicon в коде и каталоге;


-  Вставляйте коды <link rel=» после всех уже имеющихся кодов <link rel=»;


-  Если иконка долго не появляется, очистите кэш вашего браузера (Ctrl+F5 в Chrom).

### Еще один вариант добавить одинаковый  Favicon на сам сайт и на административную панель

- Для этого удалите все старые коды с favicon (читать выше);
- Сделайте в генераторе favicon понравившуюся вам иконку в формате favicon.ico;
- Иконку favicon.ico загрузите в корневую папку вашего сайта [httpdocs] или [publ_html];
- Вставьте следующий код в шаблон вашего сайта между тегами <heаd> и </ heаd>;


- Для вставки кода войдите из консоли сайта WP в редактор: Консоль→Внешний вид→Редактор→header.php/;
- Найдите тег <heаd> и до тега </ heаd> вставьте код;
- Не забудьте сохраниться.

Все! Установлен одинаковый favicon  для основной части сайта и для консоли.

**Примечание:** Анимированнная иконка для сайта (формата .gif)  читается только последними версиями Firefox. Вставляется внутрь элемента <head> ,также как и коды для favicon:

На этом все!

[Читайте так же:  Переадресация на сайте WordPress, 301 редирект](https://www.wordpress-abc.ru/plaginy/pereadresatsiya-na-sayte-wordpress.html)

Игорь Серов специально для сайта «[Как сделать сайт WordPress](https://www.wordpress-abc.ru/)»

### Другие статьи раздела: Плагины

- Записи не найдены