# Как сжать изображения WordPress: Плагин EWWW Image Optimizer

[Главная](https://www.wordpress-abc.ru/) » [Плагины](https://www.wordpress-abc.ru/plaginy) » Как сжать изображения WordPress: Плагин EWWW Image Optimizer

![сжать изображения WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer.jpg)

Содержание

- [Вступление](https://www.wordpress-abc.ru/plaginy/kak-szhat-izobrazheniya-wordpress-plagin-ewww-image-optimizer.html#i)
- [Где получить plugin EWWW Image Optimizer](https://www.wordpress-abc.ru/plaginy/kak-szhat-izobrazheniya-wordpress-plagin-ewww-image-optimizer.html#_plugin_EWWW_Image_Optimizer)
- Настройка плагина EWWW Image Optimizer
  - [Общие настройки плагина EWWW Image Optimizer](https://www.wordpress-abc.ru/plaginy/kak-szhat-izobrazheniya-wordpress-plagin-ewww-image-optimizer.html#__EWWW_Image_Optimizer)
  - [Дополнительные настройки плагина EWWW Image Optimizer](https://www.wordpress-abc.ru/plaginy/kak-szhat-izobrazheniya-wordpress-plagin-ewww-image-optimizer.html#__EWWW_Image_Optimizer-2)
  - [Настройки конвертирования плагина EWWW Image Optimizer](https://www.wordpress-abc.ru/plaginy/kak-szhat-izobrazheniya-wordpress-plagin-ewww-image-optimizer.html#__EWWW_Image_Optimizer-3)
- Работа плагина EWWW Image Optimizer, сжать изображения WordPress
  - [Дополнения](https://www.wordpress-abc.ru/plaginy/kak-szhat-izobrazheniya-wordpress-plagin-ewww-image-optimizer.html#i-2)
  - [Другие плагины WordPress](https://www.wordpress-abc.ru/plaginy/kak-szhat-izobrazheniya-wordpress-plagin-ewww-image-optimizer.html#_WordPress)

## Вступление

Фотографии занимают достаточно много места в объеме сайта. Это увеличивает время загрузки сайта, как следствие, косвенно мешает его продвижению. Для примера я посмотрел объем этого сайта. Объем его резервной копии равен 263 Мб, а объем всех картинок сайта составляет 160 Мб. Напомню, по умолчанию, все картинки и все медиафайлы загружаются в папку wp-content/uploads.

Субъективно, 160 Мб для сайта на WordPress, который сам по себе не отличается высокой скоростью, это много. Для объективной проверки посмотрим, что «говорят» сервисы проверки скорости загрузки сайта, например https://gtmetrix.com/ или//developers.google.com/speed/pagespeed/insights/.

[![плагин-EWWW-Image-Optimizer-12](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-12.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-12.jpg)сервис проверки скорости загрузки сайта https://gtmetrix.com/

[Читайте так же:  Как поменять абсолютные ссылки WordPress на относительные: SSL сертификация](https://www.wordpress-abc.ru/bezopasnost-wp/kak-pomenyat-absolyutnyie-ssyilki-wordpress-na-otnositelnyie.html)

[![плагин-EWWW-Image-Optimizer-11](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-11.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-11.jpg)сервис проверки скорости загрузки сайта, //developers.google.com/speed/pagespeed/insights/.

Обе проверки, объективно показывают, что изображения оптимизированы и не влияют на скорость загрузки сайта. Это и понятно, изображения я оптимизирую еще до вставки на сайт, а библиотеку медиафайлов я недавно оптимизировал (Читать: [Оптимизация изображений WordPress](https://www.wordpress-abc.ru/seo-wordpress/optimizatsiya-izobrazheniy-wordpress.html)). Как бы то ни было, для эксперимента, покажу, как сжать изображения WordPress (оптом) используя плагин EWWW Image Optimizer.

## Где получить plugin EWWW Image Optimizer

Сжать изображения WordPress нам поможет плагин EWWW Image Optimizer. В зависимости от вашего сервера, а вернее его настроек, возьмите плагин EWWW…:

- На странице административной панели: Плагины→Добавить новый→Поиск по имени→ EWWW Image Optimizer;

[![плагин-EWWW-Image-Optimizer-10](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-10.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-10.jpg)

Или

- Скачайте плагин на его официальной странице (https://wordpress.org/plugins/ewww-image-optimizer/)
- Залейте его по FTP в каталог wp-content/plugins
- Активируйте на странице: Плагины→Установленные→Активировать.

**Примечание 1:** за плагином EWWW Image Optimizer хорошо «ухаживают» поэтому вы всегда найдете обновленную версию плагина, актуальную для последних версий WordPress.

**Примечание 2:** Данный плагин постоянно обновляется, потому что, есть платная версия плагина, на которой оптимизация изображений проходит с использованием облачных технологий через сервис плагина.

После активации плагина на странице «Медиафайлы» появятся два новых пункта:

1. Массовая оптимизация;
2. Неоптимизированные.

[![плагин-EWWW-Image-Optimizer-9](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-9.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-9.jpg)

[Читайте так же:  Как экспортировать пользователей WordPress](https://www.wordpress-abc.ru/uroki-wordpress/kak-eksportirovat-polzovateley-wordpress.html)

Но для начала идем настраивать плагин: Настройки→EWWW… (есть другой вход в списке плагинов).

[![плагин-EWWW-Image-Optimizer-8](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-8.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-8.jpg)

## Настройка плагина EWWW Image Optimizer

Замечу, в бесплатной версии плагина вы несколько ограничены в настройках, и можете либо сжать изображения WordPress форматов (jpeg, gif, png) без потери качества (Lossless Compression), либо не сжимать их. Медифайлы pdf не обрабатываются.

### Общие настройки плагина EWWW Image Optimizer

[![плагин-EWWW-Image-Optimizer-7](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-7.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-7.jpg)

- API только в платной версии поэтому ничего не пишем;
- Выбираем, что сжимать (1-2-3);
- Если ваш сервер слабенький, то в пункте «Задержка» ставим вместо «0-отключено», 1 или 2 секунды.

### Дополнительные настройки плагина EWWW Image Optimizer

На странице «Дополнительные настройки» 18 пунктов. Все пункты выставлены по умолчанию достаточно грамотно, с одной стороны установленные настройки обеспечивают хорошую оптимизацию фото, с другой стороны, не перегружают сервер.[](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-4.jpg)[](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-5.jpg)[![плагин-EWWW-Image-Optimizer-6](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-6.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-6.jpg)

1. Уровень оптимизации, оставляем [2];
2. Отключение сервиса pingout, по умолчанию отключен. Pingout это бесплатный сервис сжатия изображений png. Отключен потому, что может перегрузить или просто не работать на вашем сервере.
3. Связан с включением пункта [2].
4. Качество сжатых фотографий jpeg. По умолчанию 82, можно поменять.
5. Параллельная оптимизация (Parallel optimization). По умолчанию включен. Нужен для более ускорения процесса оптимизации, оптимизируются сразу несколько фото. Данная настройка сильнее грузит сервер, поэтому могут быть проблемы. Кстати, время массовой оптимизации может занять несколько часов.
6. Оптимизация по расписанию. Нужно включить если у вас постоянно, по нескольку раз в день добавляются фото, причем много фото добавляется не вами.
7. Если ваши изображения хранятся не в папках по умолчанию (wp-content/uploads), то в этой настройке нужно указать полный путь до этих папок. Вверху будет подсказка именно вашего полного пути. Примечание: как вы можете догадаться, можно создать папку, в неё загрузить любые фото, не относящиеся к сайту. Выключить пункт [8], и оптимизировать изображения именно этой папки со сторонними фото.
8. Включаем в оптимизацию папки медиа библиотеки.

[![плагин-EWWW-Image-Optimizer-5](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-5.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-5.jpg)

[![плагин-EWWW-Image-Optimizer-4](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-4-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-4-1.jpg)

[Читайте так же:  Как добавить постраничную навигацию на сайт WordPress](https://www.wordpress-abc.ru/plaginy/kak-dobavit-postranichnuyu-navigatsiyu-na-sayt-wordpress.html)

9-10-11-Пункты настроек, касаются размеров изображений. Если вы загружали фото от 2000 px, то можете их сжать с изменением размера.

12-13 Можно указать минимальный размер (в байтах) фото, которые не нужно оптимизировать;

14-Можно исключить оптимизацию оригиналов с потерей качества (изменение размеров)

15-Можно исключить удаление мета данных на оригинальных фото.

**Примечание:** напомню, что загружая одно фото на сайт, система создает из него еще три фото: миниатюра, Средний, Большой. Если оригинал фото большой, то система создаст еще четыре фото. Настройка размеров каждого фото на странице: Настройки→Медиафайлы.

### Настройки конвертирования плагина EWWW Image Optimizer

[![Настройки конвертирования плагина EWWW Image Optimizer](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-3.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-3.jpg)Настройки конвертирования плагина EWWW Image Optimizer

Здесь обращаем внимание на удаление оригиналов фотографий. По умолчанию этот пункт включен. Тем самым не только оптимизируем фото WordPress, но и чистим медиабиблиотеку.

После сохранения всех настроек идем «на старт» плагина. Для эксперимента я оставлю настройки по умолчанию.

## Работа плагина EWWW Image Optimizer, сжать изображения WordPress

На странице: Медиафайлы→Массовая оптимизация, читаем, что сообщает система:

«В библиотеке обнаружено 1583 изображений (77 неоптимизированных), 7850 миниатюр (383 неоптимизированных). Ранее оптимизированные изображения будут пропущены».

Вижу по сообщению, что плагин помнит все ранее оптимизированные фото и находит новые фото, которые нужно оптимизировать, по установленным настройкам. Запускам процесс оптимизации и занимаемся своими делами. Мне ждать окончания придется долго, FTP моего хоста медленное.

[![плагин-EWWW-Image-Optimizer-2](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-2.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-2.jpg)

Сам процесс оптимизации отображается на странице при желании его можно остановить (1 на фото)

[![плагин-EWWW-Image-Optimizer-1](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/07/plagin-EWWW-Image-Optimizer-1.jpg)

Я ждал завершения процесса: 40 минут. После завершения оптимизации, идем на вкладку: Медиафайлы→Неоптимизированные и смотрим, что не смог оптимизировать плагин.

### Дополнения

- Плагин может работать и со сторонними галереями установленными на сайт. Для их сканирования есть вторая кнопка на вкладке: Массовая оптимизация.
- Все результаты сжатия видим в библиотеке Медиафайлов в строке для каждой фотографии.

[©www.wordpress-abc.ru](https://www.wordpress-abc.ru/)

### Другие плагины WordPress

- [Найти и удалить вирус на WordPress плагином Antivirus](https://www.wordpress-abc.ru/plaginy/nayti-i-udalit-virus-na-wordpress-plaginom-antivirus.html)
- [Как найти вирус на сайте — плагин безопасности Wordfence Security](https://www.wordpress-abc.ru/plaginy/kak-nayti-virus-na-sayte-plagin-bezopasnosti-wordfence-security.html)
- [Media File Cleaner плагин WordPress для чистки Media Library](https://www.wordpress-abc.ru/plaginy/media-file-cleaner-plagin-wordpress-dlya-chistki-media-library.html)
- [WordPress плагин Exploit Scanner безжалостный борец с вирусами](https://www.wordpress-abc.ru/plaginy/wordpress-plagin-exploit-scanner-bezzhalostnyiy-borets-s-virusami.html)
- [Как бороться со спамом в комментариях WordPress](https://www.wordpress-abc.ru/plaginy/kak-borotsya-so-spamom-v-kommentariyah-wordpress.html)
- [Плагин Google AdSense WordPress уникальный инструмент для размещения рекламы Google](https://www.wordpress-abc.ru/plaginy/plagin-google-adsense-wordpress-unikalnyiy-instrument-dlya-razmeshheniya-reklamyi-google.html)
- [Как добавить постраничную навигацию на сайт WordPress](https://www.wordpress-abc.ru/plaginy/kak-dobavit-postranichnuyu-navigatsiyu-na-sayt-wordpress.html)
- [Карта Google maps на WordPress](https://www.wordpress-abc.ru/plaginy/karta-google-maps-na-wordpress.html)
- [Плагин TAC WordPress ищет и удаляет зашифрованные ссылки в темах сайта](https://www.wordpress-abc.ru/plaginy/plagin-tac-wordpress-ishhet-i-udalyaet-zashifrovannyie-ssyilki-v-temah-sayta.html)
- [Как перевести URL адреса WordPress из кириллицы в латиницу](https://www.wordpress-abc.ru/plaginy/kak-perevesti-url-adresa-wordpress-iz-kirillitsyi-v-latinitsu.html)