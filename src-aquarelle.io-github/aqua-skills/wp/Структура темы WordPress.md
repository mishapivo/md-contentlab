# Структура темы WordPress

[Главная](https://www.wordpress-abc.ru/) » [Шаблоны WP](https://www.wordpress-abc.ru/temy-wordpress) » Структура темы WordPress

![img](https://www.wordpress-abc.ru/wp-content/uploads/2016/01/struktura-temyi-vordpress.jpg)

Шаблон или тема WordPress, задает внешний вид сайта, блога или магазина созданного с помощью CMS WordPress. Шаблон задает внешний вид сайта по задумкам автора шаблона. Автор определяет цвета шаблона, расположение виджетов и сайдбара, наполненность нижней и верхней части сайта. Большинство шаблонов WordPress открыты для редактирования, и вы можете менять и расположение виджетов, и цвета шаблона и фоновые изображения, а также делать другие изменения. Чтобы заниматься редактированием шаблона своего сайта, нужно не только знать основы HTML, PHP и CSS, но и как минимум, понимать, как построена структура темы WordPress. Этим и займемся в этой статье.

В этой статье мы не будем глобально редактировать или верстать заново шаблон WordPress. Для начала достаточно будет разобраться с общим устройством [темы (шаблона)](https://www.wordpress-abc.ru/administrirovanie/tema-wordpress.html).

Содержание

- [Структура темы WordPress  или как строится шаблон WordPress](https://www.wordpress-abc.ru/temy-wordpress/struktura-temyi-wordpress.html#_WordPress___WordPress)
- [Основные файлы шаблона WordPress](https://www.wordpress-abc.ru/temy-wordpress/struktura-temyi-wordpress.html#__WordPress)
- [Как редактировать файлы шаблона WordPress](https://www.wordpress-abc.ru/temy-wordpress/struktura-temyi-wordpress.html#__WordPress-2)

## Структура темы WordPress  или как строится шаблон WordPress

Если вы посмотрите на любой сайт WordPress, то даже визуально увидите, разделение его на своеобразные зоны. Легко можно выделить верхнюю часть (шапку или header) шаблона, боковую (боковые) части, так называемые [виджеты](https://www.wordpress-abc.ru/uroki-wordpress/saydbar-vidzhetyi-wordpress.html), нижнюю часть сайта, так называемый футер (footer, подвал) шаблона. Структурная схема самого простого шаблона выглядит так.

[![тема-wordpress-структура](https://www.wordpress-abc.ru/wp-content/uploads/2016/01/tema-wordpress-struktura.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/01/tema-wordpress-struktura.jpg)Если вы устанавливали шаблон по FTP или хотя бы смотрели корневой каталог сайта, то знаете, что все темы, установленные на сайт «лежат» в каталоге **wp-content/templates/название_шаблона**. Посмотрим, какие файлы образуют шаблон WordPress.

[![шаблон-wordpress](https://www.wordpress-abc.ru/wp-content/uploads/2016/01/shablon-wordpress.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/01/shablon-wordpress.jpg)

[Читайте так же:  Как сделать кнопку плавного прокручивания «Наверх»](https://www.wordpress-abc.ru/plaginy/wordpress-bez-plugins/kak-sdelat-knopku-plavnogo-prokruchivaniya-naverx.html)

## Основные файлы шаблона WordPress

Современные темы WordPress объемные и файлов в теме много. Однако есть основные файлы, без которых невозможно создать не одну тему.

Перед тем, как их перечислить, давайте посмотрим на структуру шаблона (фото выше).

Чтобы создать такую структуру, нужны файлы:

1. header.php;
2. footer.php;
3. sidebar.php

Это файлы создающие блоки окружающие основное (меняющееся) содержание сайта. То есть, окружающий статьи (посты) и страницы.

Но кроме шапки, подвала и сайдбаров, на сайте должны быть:

- Главная страница;
- Страницы;
- Посты;
- Страницы архивов (рубрик и тегов);
- Страница показа результатов поиска;
- Страница ошибок;
- Комментарии.

[Читайте так же:  Админка Wordpress: все про административную панель WordPress сайта](https://www.wordpress-abc.ru/administrirovanie/adminka-wordpress.html)

Все эти элементы контента выводятся в шаблоне с помощью следующих файлов входящих в структуру шаблона WordPress:

1. index.php
2. page.php
3. single.php
4. archive.php
5. search.php
6. 404.php
7. comments.php

Количество файлов в шаблоне может гораздо больше, внешний вид значительно разнообразнее.

Но есть еще три файла в шаблоне, без которых он не будет работать. Это файлы: functions.php, loop.php и style.css.

- functions.php – основной файл сайта, определяющий его функциональность.
- loop.php – файл [основного цикла сайта](https://www.wordpress-abc.ru/funkcii-wordpress/cikl-wordpress.html).
- [style.css](https://www.wordpress-abc.ru/cms-woprdpress/codex-wp/kak-redaktirovat-css-sayta-wordpress.html) – файл задающий внешний вид сайта, его цвета, шрифты и другие каскадные таблицы стилей данного шаблона.

Все файлы шаблона связаны друг с другом тегами шаблонов WordPress.

## Как редактировать файлы шаблона WordPress

В процессе использования шаблона Worpress приходится его редактировать. Связано это и с желанием что-либо поменять или дополнить. Так же, некоторые плагины «требуют» вставлять дополнительные коды в то или иное место шаблона.

[Читайте так же:  Файл robots.txt для wordpress](https://www.wordpress-abc.ru/veb-instrumenty/fajl-robots-txt-dlya-wordpress.html)

Для редактирования файлов шаблона нужно соблюдать следующие правила:

1. Никогда не делайте редакцию файлов шаблона без резервной копии сайта. Как минимум сделайте резервную копию шаблона;
2. Никогда не редактируйте файлы шаблона в блокнотах Word. Для редактирования используйте только текстовые блокноты типа Notepad++ в кодировке UTF-8 без BOOM.
3. Осторожно используйте редактор административной части: Внешний вид→Редактор.

Игорь Серов, специально для сайта «[Как сделать сайт WordPress](https://www.wordpress-abc.ru/)».

### Другие статьи раздела: Шаблоны WordPress

- [ColorMag журнальная тема WordPress](https://www.wordpress-abc.ru/temy-wordpress/colormag-zhurnalnaya-tema-wordpress.html)
- [WordPress шаблон для строительной компании, Build Lite  ](https://www.wordpress-abc.ru/temy-wordpress/shablon-wordpress-dlya-stroitelnoy-kompanii-build-lite.html)
- [Зачем нужна дочерняя тема WordPress](https://www.wordpress-abc.ru/temy-wordpress/zachem-nuzhna-dochernyaya-tema-wordpress.html)
- [Установка и замена шаблонов WordPress](https://www.wordpress-abc.ru/temy-wordpress/ustanovka-i-zamena-shablonov-wordpress.html)