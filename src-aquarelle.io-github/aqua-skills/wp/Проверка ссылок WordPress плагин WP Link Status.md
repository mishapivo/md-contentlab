# Проверка ссылок WordPress: плагин WP Link Status

[Главная](https://www.wordpress-abc.ru/) » [Плагины](https://www.wordpress-abc.ru/plaginy) » Проверка ссылок WordPress: плагин WP Link Status

![Проверка ссылок WordPress, плагин WP Link Status](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/WP-Link-Status.jpg)

Здравствуйте! Продолжаем бороться с битыми ссылками WordPress. В прошлой статье по этой теме ([Битые ссылки на WordPress сайте](https://www.wordpress-abc.ru/seo-wordpress/bityie-ssyilki-na-wordpress-sayte.html)), я искал битые ссылки, на запрос которых веб-сервер дает 404 ответ. В статье я показал, как искать битые ссылки программой XENU и/или использовать популярный плагин «Broken link checker».

В этой статье пойдем несколько дальше и не только найдем неправильные, ошибочные (битые) ссылки, но и сделаем проверку ссылок WordPress, на все коды ответов и ошибок веб-сервера:

- Все 200-е Success (Правильно);
- Все 300-е Redirections (Переадресация);
- Все 400-е Errors (Ошибка);
- Все 500-е Server Error (Ошибка сервера).

А поможет в такой проверке ссылок WordPress, плагин WP Link Status

Содержание

- Плагин WP Link Status —  проверка ссылок WordPress
  - [Настройка (Setting) WP Link Status](https://www.wordpress-abc.ru/plaginy/proverka-ssyilok-wordpress-plagin-wp-link-status.html#_Setting_WP_Link_Status)
  - [Запуск нового сканирования](https://www.wordpress-abc.ru/plaginy/proverka-ssyilok-wordpress-plagin-wp-link-status.html#i)
- Настройка отдельного сканирования WP Link Status
  - [General настройки](https://www.wordpress-abc.ru/plaginy/proverka-ssyilok-wordpress-plagin-wp-link-status.html#General)
  - [Настройки Content Options](https://www.wordpress-abc.ru/plaginy/proverka-ssyilok-wordpress-plagin-wp-link-status.html#_Content_Options)
  - [Настройки Content filters](https://www.wordpress-abc.ru/plaginy/proverka-ssyilok-wordpress-plagin-wp-link-status.html#_Content_filters)
  - [Настройки Links status](https://www.wordpress-abc.ru/plaginy/proverka-ssyilok-wordpress-plagin-wp-link-status.html#_Links_status)
  - [Настройки Advanced](https://www.wordpress-abc.ru/plaginy/proverka-ssyilok-wordpress-plagin-wp-link-status.html#_Advanced)
- [Сканирование ссылок](https://www.wordpress-abc.ru/plaginy/proverka-ssyilok-wordpress-plagin-wp-link-status.html#i-2)
- Работа с проверенными ссылками
  - [Выводы](https://www.wordpress-abc.ru/plaginy/proverka-ssyilok-wordpress-plagin-wp-link-status.html#i-4)
  - [Другие плагины в статьях сайта](https://www.wordpress-abc.ru/plaginy/proverka-ssyilok-wordpress-plagin-wp-link-status.html#i-5)
  - [Регистрация на сайте](https://www.wordpress-abc.ru/plaginy/proverka-ssyilok-wordpress-plagin-wp-link-status.html#i-6)
  - [Подписка на новые статьи по email](https://www.wordpress-abc.ru/plaginy/proverka-ssyilok-wordpress-plagin-wp-link-status.html#___email)

## Плагин WP Link Status —  проверка ссылок WordPress

В отличие от плагина «Broken link checker», который, не обновлялся 4 месяца, плагин «WP Link Status» обновляется постоянно и тестировался для последней версии WordPress 4.5.3. На момент написания статьи.

**Примечание:** Несмотря на крайне плохое обновление, «Broken link checker» работает на версии 4.5.3 и на всех прошлых версиях WordPress.

1.

2.

- идем на страницу плагина: https://ru.wordpress.org/plugins/wp-link-status,
- скачиваем его,
- заливаем по FTP в каталог plugins,
- активируем плагин из административной панели сайта.

После активации плагин готов к работе, а в меню консоли появится новый пункт WP Link Status с 4 вкладками:

1. Scan;
2. New Scan;
3. Setting;
4. Extensions

[Читайте так же:  Редактор CKEditor для WordPress](https://www.wordpress-abc.ru/plaginy/redaktor-ckeditor-dlya-wordpress.html)

### Настройка (Setting) WP Link Status

Вкладка Setting это общие настройки плагина. Относятся они к работе робота сканирования. Для первого знакомства, менять ничего не будем и оставляем настройки по умолчанию.

### Запуск нового сканирования

Жмем вкладку «New Scan» и запускаем новое сканирование, **после предварительной настройки каждого сканирования**.

## Настройка отдельного сканирования WP Link Status

Создавая каждое сканирование плагина WP Link Status, вы может выставить настройки этого сканирования. В настройках  сканирования 5 пунктов: General, Content Options, Content filters, Links status, Advansed.

### General настройки

[![проверка ссылок WordPress, плагин WP Link Status, генеральная настройка](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/novoe-skanirovaniya-generalnaya-nastroyka-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/novoe-skanirovaniya-generalnaya-nastroyka-1.jpg)Настройка сканирования (General) WP Link Status

[Читайте так же:  Визуальный редактор для виджетов Wordpress](https://www.wordpress-abc.ru/plaginy/vizualnyiy-redaktor-dlya-vidzhetov-wordpress.html)

Общие настройки сканирования достаточно разнообразны и показывают, богатые возможности этого плагина. Здесь:

- Даем сканированию имя (любое, лучше по дате) (2),
- Выделяем, что сканируем (посты и/или фото) (3),
- Отмечаем, сканировать всё или только внутренние или внешние ссылки (4);
- Можно указать временной период выпуска ссылок (5);
- Отмечаем определение Redirect и сканирование неправильно написанных ссылок (7).

Настройки сохраняем, но скан не запускаем, продолжаем настройки (Save scan changes).

### Настройки Content Options

[![новое-сканирования-настройка-контента-1](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/novoe-skanirovaniya-nastroyka-kontenta-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/novoe-skanirovaniya-nastroyka-kontenta-1.jpg)Настройка сканирования (Content Options) WP Link Status

Выбираем, что должен сканировать робот. По умолчанию стоит сканирование опубликованных записей и страниц.

[Читайте так же:  3+ Плагины кнопки наверх wordpress](https://www.wordpress-abc.ru/plaginy/3-plaginyi-knopki-naverh-wordpress.html)

### Настройки Content filters

[![новое-сканирования-фильтр-url](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/novoe-skanirovaniya-filtr-url-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/novoe-skanirovaniya-filtr-url-1.jpg)Настройка сканирования (Content Filters) WP Link Status

Здесь, можно отфильтровать статьи по анкору, URL, HTML разметке. По умолчанию, пусто.

### Настройки Links status

[![Настройки WP Link Status - Links status](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/novoe-skanirovaniya-nastroyka-ssyilok-skanirovaniya-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/novoe-skanirovaniya-nastroyka-ssyilok-skanirovaniya-1.jpg)Основные настройки WP Links status

Эти настройки «визитная карточка» плагина. Вы очень точно можете определить, статус все ссылок сайта. Выставив точную настройку ответов веб-сервера, можно определить, какой ответ дает веб-сервер при запросе той или иной ссылки. Например, вы точно хотите определить, как настроен редирект на сайте, и какой ответ дают переадресованные ссылки 301 или 302. Для этого убираете, галочки из настроек по умолчанию, а это все статусы ответов от 200 дл 500 и ставите галочки в чекбоксах 301 и 302. Запускаете сканирование и смотрите результат.

### Настройки Advanced

 

Чтобы не было проблем с хостером, настройки Advansed не трогаем.

## Сканирование ссылок

После выставления всех настроек запускаем сканировние, кнопка «Save and run Crowler» и смотрим результат. Если сканирование затянулось или  что-то пошло не так, его можно остановить и удалить.

[![сохранить и запустить-1](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/sohranit-i-zapustit-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/sohranit-i-zapustit-1.jpg)Запуск сканирования WP Link Status

## Работа с проверенными ссылками

После сканирования, смотрим результаты. Прежде всего, нас интересуют битые ссылки, ошибка 404. У меня таких не было, зато были ссылки неправильно написанные.

[![управление сканером WP Link Status](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/upravlenie-skanerom-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/upravlenie-skanerom-1.jpg)Управление сканированием WP Link Status

[![сканирование-запущено-1](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/skanirovanie-zapushheno-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/skanirovanie-zapushheno-1.jpg)Сканирование WP Link Status завершено сообщение системы

[![результаты-сканирования-1](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/rezultatyi-skanirovaniya-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/rezultatyi-skanirovaniya-1.jpg)Сканирование WP Link Status завершено результаты

[![результат-сканирования-wp-link-status](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/rezultat-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/rezultat-1.jpg)Сканирование WP Link Status завершено ответы веб сервера

 

Под каждой ссылкой всплывают три кнопки управления:

- Изменить (переходим в редактор);
- Trash (Удалить);
- Перейти (смотрим ссылку в браузере).

Используя кнопки управления меняем, редактируем или удаляем нерабочую ссылку.

### Выводы

В качестве вывода скажу свои ощущения от плагина. Плагин WP Link Status полностью подходит для поиска битых ссылок. Более того с его помощью можно найти ссылки любого статуса ответов веб-сервера от 200 до 500. Настройки интуитивно просты. Сканирование проходит достаточно быстро: 2000 ссылок 3 минуты. Определение ошибок точное, для повторного сканирования не требуется временной перерыв.

[©www.wordpress-abc.ru](https://www.wordpress-abc.ru/)

### Другие плагины в статьях сайта

- Записи не найдены

### Регистрация на сайте