# Три плагина карта сайта WordPress: карты сайта для посетителей и поисковиков

[Главная](https://www.wordpress-abc.ru/) » [Плагины](https://www.wordpress-abc.ru/plaginy) » Три плагина карта сайта WordPress: карты сайта для посетителей и поисковиков

![карта сайта Wordpress](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Sitemap-wordpress.jpg)

Содержание

- [Вступление](https://www.wordpress-abc.ru/plaginy/tri-plagina-karta-sajta-wordpress.html#i)
- Карта сайта WordPress для посетителей — Плагин WP Realtime Sitemap
  - [Установка плагина  WP Realtime Sitemap](https://www.wordpress-abc.ru/plaginy/tri-plagina-karta-sajta-wordpress.html#_WP_Realtime_Sitemap)
  - [Отображение карты сайта на сайте WordPress](https://www.wordpress-abc.ru/plaginy/tri-plagina-karta-sajta-wordpress.html#___WordPress)
  - [Настройки плагина WP Realtime Sitemap](https://www.wordpress-abc.ru/plaginy/tri-plagina-karta-sajta-wordpress.html#_WP_Realtime_Sitemap-2)
- Плагин Google XML Sitemaps: карта сайта Wordpres для поисковиков
  - [Настройка плагина Google XML Sitemaps](https://www.wordpress-abc.ru/plaginy/tri-plagina-karta-sajta-wordpress.html#_Google_XML_Sitemaps)
  - [Определитесь с содержанием карты сайта](https://www.wordpress-abc.ru/plaginy/tri-plagina-karta-sajta-wordpress.html#i-2)
  - [Можно создать дополнительную карту-сайта при помощи плагина Sitemap Generator](https://www.wordpress-abc.ru/plaginy/tri-plagina-karta-sajta-wordpress.html#__-__Sitemap_Generator)

## Вступление

Карта сайта WordPress это важнейший инструмент ускоряющий индексацию  страниц сайта. При помощи различных плагинов WordPress можно создать карту сайта различных форматов (XML,HTML,CVS). Для поисковиков важен формат XML. При этом нужно помнить, что карта сайта в формате XML не видна посетителям. Для посетителей карту сайта можно создать при помощи специальных плагинов. В этой статье я приведу три плагина для создания карты сайта, как для поисковиков, так и для посетителей.

## Карта сайта WordPress для посетителей — Плагин WP Realtime Sitemap

Плагин WP Realtime Sitemap позволяет отображать на сайте сформированную им же карту сайта. Этот плагин не создает карту сайта в формате XML и  не передает поисковикам созданную карту сайта. Плагин WP Realtime Sitemap создает карту сайта для внутреннего пользования и может отображать карту сайта  в любом месте сайта WP.

### Установка плагина  WP Realtime Sitemap

Устанавливается плагин  любым из трех стандартных способов (Подробно об установке плагинов читать [ТУТ](https://www.wordpress-abc.ru/uroki-wordpress/ustanovka-udalenie-plagina-na-wordpress.html)).

1. Скачиваем  Zip архив плагина и устанавливаем на сайт WP при помощи загрузчика в административной панели;
2. Ищем плагин в окне «Поиск» и затем устанавливаем автоматом;
3. Закачиваем распакованный архив плагина по FTP в каталог сайта.

Будем считать, что плагин установлен. Можно приступать к настройкам плагина WP Realtime Sitemap.

[Читайте так же:  Плагин Jetpack заменит 33 плагина Wordpress](https://www.wordpress-abc.ru/plaginy/plagin-jetpack-zamenit-33-plagina-wordpress.html)

### Отображение карты сайта на сайте WordPress

Для вставки карты сайта на страницы сайта нужно в визуальном редакторе добавить строку: **wp-realtime-sitemap, **в квадратных скобках при написании статьи.

Для вывода карты сайта в меню сайта, нужно создать Страницу на вкладке Консоль→Страницы→Создать новую. Дать странице имя, например, карта-сайта. В окне визуального редактора ввести код:

Поместить  сделанную страницу в любое созданное меню сайта (*Консоль→ Внешний вид → Меню*).

### Настройки плагина WP Realtime Sitemap

Заходим по адресу: *Консоль→Параметры→WP Realtime Sitemap*.

[![Плагин WP Realtime Sitemap](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-05-300x235.png)](http://wordpress-abc.ru/plaginy/tri-plagina-karta-sajta-wordpress.html/attachment/karta-sajta-wp-05)

В открывшемся окне настройки плагина WP Realtime Sitemap заполняете нужные пункты. Вот несколько принципиальных настроек:

Можно включить/выключить показ страниц, категорий, сообщений и архивов на катре сайта.

[![WP Realtime Sitemap](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-07-300x122.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-07.png)

[Читайте так же:  4 Способа рассылка писем с Wordpress](https://www.wordpress-abc.ru/uroki-wordpress/4-sposoba-rassyilka-pisem-s-wordpress.html)

При включении этих пунктов можно убрать из показа отдельную информацию, указав ID (идентификационный номер) ненужных к отражению материалов.

В настройках WP Realtime Sitemap можно включить показ категорий и мета тегов в виде облака. Выбрать можно либо показ облаком, либо списком.

[![WP Realtime Sitemap](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-08-300x236.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-08.png)

В настройках плагина можно изменить заголовки всех элементов карты сайта: сообщения, страницы, меню, архивы, категории, теги.

[![WP Realtime Sitemap](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-06-300x160.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-06.png)

Также можно поменять все пункты меню местами.

[![WP Realtime Sitemap](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-09-300x240.png)](http://wordpress-abc.ru/plaginy/tri-plagina-karta-sajta-wordpress.html/attachment/karta-sajta-wp-09)

По умолчанию иерархия карты сайта следующая:

- Меню;
- Страницы;
- Сообщения;
- Пользовательские типы сообщений;
- Архивы;
- Категории;
- Теги.

## Плагин Google XML Sitemaps: карта сайта Wordpres для поисковиков

Прежде всего, не путайте плагин Google XML Sitemaps с плагином  Google XML Sitemap. Здесь речь пойдет о плагине Google XML Sitemaps.

В отличие от плагина WP Realtime Sitemap плагин Google XML Sitemaps при установке генерирует  специальную карту сайта в формате XML и информирует  поисковые машины  Google, Bing, Yahoo  о созданной  карте сайта. Этот плагин работает в режиме on-line. Карта сайта WordPress постоянно пополняется и отправляется поисковым машинам по мере публикации материала на сайте. Настройка плагина делается один раз при установке плагина.

[Читайте так же:  Плагин Google AdSense WordPress уникальный инструмент для размещения рекламы Google](https://www.wordpress-abc.ru/plaginy/plagin-google-adsense-wordpress-unikalnyiy-instrument-dlya-razmeshheniya-reklamyi-google.html)

### Настройка плагина Google XML Sitemaps

После установки плагина  Google XML Sitemaps в меню «Параметры» появиться новый пункт «XML Sitemap». Это пункт настройки плагина Google XML Sitemaps.Открываем его.

[![Google XML Sitemaps](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-11-300x266.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-11.png)

В первой строке настройки видим запись с предложением, создать карту сайта в первый раз. Не спешите нажимать  эту кнопку. Ознакомьтесь со всеми настройками плагина по умолчанию.

[![Google XML Sitemaps](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-12-300x116.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-12.png)

Сейчас нас интересует пункт «Расположение Вашего файла с картой сайта».

[![Google XML Sitemaps](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-14-300x163.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-14.png)[](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-14.png)В настройке можно указать плагину, где расположена карта сайта XML. Возможны два варианта расположения карты сайта WordPress для плагина Google XML Sitemaps.

1.

1.

**Примечание**: Права доступа CHMOD меняются в FTP клиенте. Для этого кликните правой кнопкой по файлу и в строке «Права доступа к файлу» изменить права доступа CHMOD.

### **Определитесь с содержанием карты сайта**

[![Карта-сайта-WP-15](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-15-300x266.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-15.png)

В настройках Google XML Sitemaps можно  изменить частоту отправки карты поисковикам.Правда этот пункт настройки не является командой.а носит только рекомендательный характер.

[![Google XML Sitemaps](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-161.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-161.png)

В пункте «Постройте карту сайта заново при обновлении дневника»  должна стоять галочка.

Поставьте галочки в двух пунктах. **Записывать карту как обычный файл XML и записывать карту как упакованный файл**. Упакованный файл немного снижает нагрузку на сервер.

[![Google XML Sitemaps](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-13-300x224.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-13.png)

После заполнения этого пункта, не трогая остальные можно нажимать  **«Создать  карту сайта первый раз».**

Больше трогать ничего не нужно. Нужно  запастись терпением и ждать итогов работ плагина Google XML Sitemaps. Если все нормально плагин сообщит, что карта сайта создана, покажется число создания и в настройках будет указан адрес, где карта сайта расположена.

[![Google XML Sitemaps](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-19-300x123.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-19.png)

Плагин Google XML Sitemaps создает карту сайта по адресу**: Ваш_сайт/sitemap.xml**. Кликнув по адресу можно  посмотреть, как ваша карта выглядит. После создания карт сайта можно добавить их размещение в файл [Rotots.txt](http://wordpress-abc.ru/veb-instrumenty/fajl-robots-txt-dlya-sajta-wordpress.html).

### Можно создать дополнительную карту-сайта при помощи плагина Sitemap Generator

Устанавливаете плагин Sitemap Generator одним из удобных способов. В меню консоли появляется пункт «Sitemap Generator». Этот плагин создает карту-сайта в трех форматах: XML,HTML,CVS. Для поисковиков важен формат XML. При открытии пункта меню Sitemap Generator → Generator вы можете увидеть фактические адреса созданных карт.

[![Sitemap Generator](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-17-300x171.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-17.png)

Также можно настроить содержание карты расставив приоритеты в настройках. Значение «0» исключит пункт из карты сайта. Нормальный приоритет 0.5.

[![Sitemap Generator](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-18-300x261.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/%D0%9A%D0%B0%D1%80%D1%82%D0%B0-%D1%81%D0%B0%D0%B9%D1%82%D0%B0-WP-18.png)

Этот плагин (Sitemap Generator) только создает карты сайта, но не поддерживает связи с поисковиками. URL карты сайта XML можно и нужно отправлять  в веб-инструменты Google WebMasters и Яндекс Вебмастер вручную.

**Подведем итог выше изложенного**

- WordPress предлагает массу инструментов для создания карты сайта. Для поисковых машин важны карты сайта в формате XML и xml.gz.
- При добавлении материала на сайт карта сайта должна обновляться. Чтобы не делать это вручную, лучше установить  плагин с автоматическим обновлением карты сайта (Google XML Sitemaps).
- Карта сайта WordPress для посетителей создается при помощи сторонних плагинов, например WP Realtime Sitemap. Я использую плагин: SEO HTML Sitemap. [Карта сайта www.wordpress-abc.ru](https://www.wordpress-abc.ru/karta-sajta) в две колонки.

Вот такие Три плагина карта сайта WordPress! Успехов  в изучении WordPress.

Игорь Серов специально для сайта «[Как сделать сайт WordPress](https://www.wordpress-abc.ru/)»

### Другие статьи раздела: Плагины

- Записи не найдены