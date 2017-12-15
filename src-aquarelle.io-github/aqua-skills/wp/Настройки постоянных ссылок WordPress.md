# Настройки постоянных ссылок WordPress

[Главная](https://www.wordpress-abc.ru/) » [Уроки WordPress](https://www.wordpress-abc.ru/uroki-wordpress) » Настройки постоянных ссылок WordPress

![Настройки постоянных ссылок WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2015/02/Nastroyki-postoyannyih-ssyilok-WordPress.jpg)

Здравствуйте. Сегодня в разделе «Уроки создания WordPress» блога WordPress-abc.ru, новая тема: Настройки постоянных ссылок WordPress. В статье я расскажу, что такое постоянные ссылки WordPress, какие виды ссылок возможны по умолчанию и как, настроить внешний вид ссылок WordPress.

Для начала разберемся, что такое постоянные ссылки в WordPress.

Содержание

- [Что такое постоянная ссылка](https://www.wordpress-abc.ru/uroki-wordpress/nastroyki-postoyannyih-ssyilok-wordpress.html#i)
- [Настройки постоянных ссылок WordPress в консоли](https://www.wordpress-abc.ru/uroki-wordpress/nastroyki-postoyannyih-ssyilok-wordpress.html#__WordPress)
- Перевод постоянных ссылок
  - [Другие Уроки WordPress](https://www.wordpress-abc.ru/uroki-wordpress/nastroyki-postoyannyih-ssyilok-wordpress.html#_WordPress)

## Что такое постоянная ссылка

Постоянная ссылка (Permalinks) в WordPress, это вид URL адреса любого содержимого сайта: статьи, рубрики, метки, архивов. Внешний вид постоянной ссылки настраивается.

## Настройки постоянных ссылок WordPress в консоли

Настройки постоянных ссылок WordPress, нужно сделать при первых настройках блога. После выставления настроек для ссылок их менять не следует, потому что смена вида ссылок уберет содержимое сайта из поисковой выдачи.

Делается настройка внешнего вида постоянных ссылок на вкладке *Настройки→Постоянные ссылки*.

WordPress предлагает 5 вариантов внешнего вида ссылок. Остановлюсь на некоторых.

[![настройки](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/nastroyki.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/vidyi-ssyilok.jpg)

Ссылка по-умолчанию, имеет самый не привлекательный внешний вид, как для пользователей, так и для поисковиков. Внешний вид ссылок по умолчанию следующий:

- Ссылка статьи: http://vash_domen.ru/?p=IDстатьи
- Метка по умолчанию: http://vash_domen.ru/?tag=IDтега
- Рубрика по умолчанию: http://vash_domen.ru/?cat=IDрубрики (не зависит от вложения категорий).

Если вы оставите постоянные ссылки в виде по-умолчанию, дополнительные настройки, которые есть на этой странице, работать не будут.

Посмотрим, как изменятся постоянные ссылки, статей, рубрик и меток, если вид постоянных ссылок установить: Название статьи.

[![название записи](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/nazvanie-zapisi1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/nazvanie-zapisi1.jpg)

Те же ссылки преобразуются:

- http://vash_domen.ru/название статьи;
- http://vash_domen.ru/tag/название тега;
- http://vash_domen.ru/category/родительская рубрика/дочерняя рубрика;

tag и category вставляются в ссылку по-умолчанию, если не заполнять поля дополнительных настроек.

[![дополнительные настройки ссылок](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/dopolnitelnyie-nastroyki-ssyilok.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/dopolnitelnyie-nastroyki-ssyilok.jpg)

Если в дополнительные настройки поставить свои префиксы, например rubriki и metki , то те же ссылки будут в виде:

[Читайте так же:  ID WordPress страницы, поста, раздела, пользователя](https://www.wordpress-abc.ru/uroki-wordpress/id-wordpress-stranitsyi-posta-razdela-polzovatelya.html)

[![дополнительный-настройки](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/dopolnitelnyiy-nastroyki.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/dopolnitelnyiy-nastroyki.jpg)

- http://vash_domen.ru/metki/название метки;
- http://vash_domen.ru/rubriki/родительская рубрика/дочерняя рубрика.

Можно пойти дальше и установить вид ссылки в произвольной форме (5 на фото). В этих настройках, можно задать практически любой вид постоянной ссылки.  Синтаксис ссылки посмотрите [ТУТ](http://codex.wordpress.org/Using_Permalinks).

![виды ссылок](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/vidyi-ssyilok.jpg)

Как видите, ничего сложного в настройках постоянных ссылок нет. Остается только один вопрос, как сделать ссылку не на русском языке, а в транлитерном переводе латинскими буквами.

## Перевод постоянных ссылок

Для перевода URL не обойтись без стороннего плагина. Самый простой и самый популярный плагин для перевода постоянных ссылок это плагин: Cyr-And-Lat. Плагин достаточно старый, но работает без проблем.

Плагин настроек не имеет, нужно его установить и все ссылки будут переведены автоматом.

> Повторюсь, настроить ссылки и установить плагин перевода url это нужно при первых настройках блога, до начала наполнения его материалами.

Кроме описанных выше настроек постоянных ссылок, можно включить в URL  дату: пункты день и название (1 на фото), и месяц и название(2 на фото). Также можно добавить в URL порядковый номер: настройка Цифры(3 на фото).

Игорь Серов специально для сайта «[Как сделать сайт WordPress](https://www.wordpress-abc.ru/)»

### Другие Уроки WordPress

- [Хостинг для WordPress: параметры хостинга сайта WordPress](https://www.wordpress-abc.ru/uroki-wordpress/hosting-dlya-wordpress.html)
- [Публикация статей в WordPress](https://www.wordpress-abc.ru/uroki-wordpress/publikatsiya-statey-v-wordpress.html)
- [Домен для WordPress сайта](https://www.wordpress-abc.ru/uroki-wordpress/domen-dlya-wordpress-3.html)
- [Создаем меню WordPress: как создать меню WordPress](https://www.wordpress-abc.ru/uroki-wordpress/sozdaem-menyu-wordpress.html)
- [Что такое тема WordPress](https://www.wordpress-abc.ru/uroki-wordpress/chto-takoe-tema-wordpress.html)
- [Установка WordPress на сервер хостинга](https://www.wordpress-abc.ru/uroki-wordpress/ustanovka-wordpress-na-server-hostinga.html)
- [Создание базы данных для WordPress](https://www.wordpress-abc.ru/uroki-wordpress/sozdanie-bazyi-dannyih-dlya-wordpress.html)
- [Что такое плагины WordPress](https://www.wordpress-abc.ru/uroki-wordpress/chto-takoe-plaginyi-wordpress-2.html)
- [Первые настройки WordPress](https://www.wordpress-abc.ru/uroki-wordpress/pervyie-nastroyki-wordpress.html)
- [Как объединить два сайта WordPress](https://www.wordpress-abc.ru/uroki-wordpress/kak-obedinit-dva-sayta-wordpress.html)