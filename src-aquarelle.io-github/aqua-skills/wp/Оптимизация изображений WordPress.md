# Оптимизация изображений WordPress

[Главная](https://www.wordpress-abc.ru/) » [SEO оптимизация Wordpress](https://www.wordpress-abc.ru/seo-wordpress) » Оптимизация изображений WordPress

![Оптимизация изображений WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/Optimizatsiya-izobrazheniy-WordPress.jpg)

Здравствуйте! Уже давно не стоит вопрос, что нужно оптимизировать на сайте для «поисковой любви», а что может и так сойти. Действительность такова, что оптимизировать нужно всё. Причем одно цепляется за другое и все сотни правил индексации и ранжирования, работающие в поисковых алгоритмах, давно переплелись в единый клубок. Например, фотографии на сайте.

Содержание

- [Три части оптимизации изображений WordPress](https://www.wordpress-abc.ru/seo-wordpress/optimizatsiya-izobrazheniy-wordpress.html#__WordPress)
- Оптимизация изображений WordPress при вставки в статью, анкоры изображений
  - [Правила для анкора фотографии](https://www.wordpress-abc.ru/seo-wordpress/optimizatsiya-izobrazheniy-wordpress.html#i)
- [Оптимизация изображений до добавления на сайт](https://www.wordpress-abc.ru/seo-wordpress/optimizatsiya-izobrazheniy-wordpress.html#i-2)
- Массовая оптимизация изображений Вордпресс
  - [Другие статьи по теме](https://www.wordpress-abc.ru/seo-wordpress/optimizatsiya-izobrazheniy-wordpress.html#i-4)

## Три части оптимизации изображений WordPress

Если посмотреть расширенный анализ скорости загрузки сайта в сети, это можно сделать любым специальным онлайн сервером, то увидим, что львиная доля времени загрузки занимают неоптимизированные фотографии.

Кроме, влияния на скорость загрузки, а она сейчас поисковиками отслеживается очень внимательно, в фотографию можно добавить ключевые слова, которые будут читаться поисковиками и влиять на позиции статьи по запросу.

Разделим оптимизацию фотографий WordPress на три части:

- Оптимизация до добавления фото на сайт;
- Оптимизация при добавлении фото в статью;
- Массовая оптимизация фото.

## Оптимизация изображений WordPress при вставки в статью, анкоры изображений

[![атрибут-alt-img](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/atribut-alt-img.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/atribut-alt-img.jpg)При добавлении изображения на любой сайт, можно задать: анкор фотографии (анкор ссылки фотографии), её описание, заголовок и размер. Для поисковиков особое значение имеет анкор. Анкор фотографии задается атрибутом alt.

Полная HTML структура добавления фото в wordpress, выглядит так.

Без подписи фото:

```
<a href="http://domen.ru/wp-content/uploads/2015/09/foto.jpg"><img class="alignnone wp-image-1934 size-medium" title="Заголовок фотографии" src="http://domen.ru/wp-content/uploads/2015/09/foto-448x252.jpg" alt="Анкор фотографии" width="448" height="252" /></a>
```

С подписью фото:

```
<a href="Http://domen.ru/wp-content/uploads/2015/09/foto.jpg"><img class="wp-image-1934 size-medium" title="Заголовок фотографии" src="http://domen.ru/wp-content/uploads/2015/09/foto-448x252.jpg" alt="Анкор фотографии" width="448" height="252" /></a> Подпись фотографии
```

В WordPress все атрибуты фотографии, в том числе и анкор, задаются в визуальном режиме:

[![оптимизация изображений wordpress](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/optimizatsiya-izobrazheniy-wordpress-3-1-448x272.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/optimizatsiya-izobrazheniy-wordpress-3-1.jpg)

Атрибуты добавляются в режимах «[Добавить медиафайл](https://www.wordpress-abc.ru/administrirovanie/izobrazheniya-foto-i-galerei-v-statyax-wordpress.html)» или в режиме «Редактировать фото».

### Правила для анкора фотографии

- Атрибут alt (анкор) для изображения должен быть уникальным.
- В статье, желательно, чтобы один анкор фотографии (атрибут alt)  должен включать прямой ключ (ключевую фразу) статьи.
- Если хотите сгенерировать анкоры автоматом, идем на Majento.ru в генератор анкоров.

[![оптимизация изображений wordpress анкор](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/optimizatsiya-izobrazheniy-wordpress-1-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/optimizatsiya-izobrazheniy-wordpress-1-1.jpg)

[Читайте так же:  Страницы WordPress: всё про страницы Wordpress](https://www.wordpress-abc.ru/administrirovanie/stranitsyi-wordpress.html)

**Примечание:** Сервис Majento взят примера и не претендует на уникальность.

Вывод 1.

В системе WordPress полностью решен вопрос с оптимизацией кода изображений. При желании можно в визуальном режиме заполнить все необходимые атрибуты  изображения важные для её оптимизации, а система сама поставит размер фото в тегах: [width=»» height=»»].

## Оптимизация изображений до добавления на сайт

> Оптимизацию изображений нужно начинать до добавления на сайт. И главное, это уменьшить объем фотографии без потери качества.

На помощь в этом вопросе придут программы по уменьшению размера файлов изображений. Здесь несколько правил:

- Наиболее легкие фотографии в расширении jpeg.
- Формат png и скриншоты в pnp самые тяжелые.

Для постоянной работы с фотографиями нужно попробовать несколько программ и выбрать парочку из них для постоянной работы. Я использую следующие программы по редактированию и сжатию фотографий:

- Стандартный инструмент Microsoft Office (отличное сжатие при изменении размера до 448x);
- Отличная программа Fast Stone Image Viewer (отличный редактор с возможностью хорошего группового сжатия и изменения формата фото);
- Программа Caesium (Бесплатная программа, с лучшим одиночным или групповым сжатием фотографий в формате jpeg).

Вывод 2.

Сжимать фотографии нужно до добавления на сайт WordPress.

[Читайте так же:  Значение меток WordPress в продвижении сайта](https://www.wordpress-abc.ru/seo-wordpress/znachenie-metok-wordpress-v-prodvizhenii-sayta.html)

## Массовая оптимизация изображений Вордпресс

> С помощью WordPress можно оптимизировать всю медиабиблиотеку WordPress, без выгрузки фотографий.

Для оптимизации фотографий уже помещенных в медиабиблиотеку WordPress **используем плагин: EWWW Image Optimizer** (протестирован на версии 4.4.2.). Плагин простой, но рабочий  периодически обновляется. Плагин Cloud (2) позволяет оптимизировать фотографии с использованием облачных технологий и сжимает фото, без смены формата. Этот плагин платный, 0,005 $ за фото до 1000 фото.

[![оптимизация-изображений-wordpress-5-1](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/optimizatsiya-izobrazheniy-wordpress-5-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/optimizatsiya-izobrazheniy-wordpress-5-1.jpg)

Устанавливаете плагин стандартно, можно из панели WordPress на вкладке Плагины→Добавить новый→Поиск по имени.

После активации плагина он готов к работе, но можно пройтись по настройкам (Настройки→ EWWW Image Optimizer) Настройки на русском, опасные настройки выделены словом «Внимание!». Кстати, есть функция переформатирование фотографий из png и gif в jpeg. После настроек открываем страницу плагина и запускаем процесс оптимизации.

[![оптимизация изображений wordpress плагином ewww Image Optimizer](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/optimizatsiya-izobrazheniy-wordpress-4-1-448x210.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/03/optimizatsiya-izobrazheniy-wordpress-4-1.jpg)

[Читайте так же:  Установка и удаление плагина на WordPress](https://www.wordpress-abc.ru/uroki-wordpress/ustanovka-udalenie-plagina-na-wordpress.html)

Через некоторое время, смотрим результаты сжатия фотографий. Отмечу, что я всегда сжимаю фото до сайта, однако плагин EWWW Image Optimizer умудряется «выжать» из каждой фото, от 5% до 20 %.

Вывод 3.

WordPress, при помощи дополнительного плагина, позволяет оптимизировать фотографии всей медиабиблиотеки сайта, в любой момент.

*Как видите, в WordPress с оптимизацией фотографий всё отлажено, всё просто и легко.*

В завершении статьи, напомню, что для облегчения сайта, можно [очистить библиотеку](https://www.wordpress-abc.ru/administrirovanie/ochistit-biblioteku-mediafaylov-wordpress.html) и/или удалить неиспользуемые фотографии [плагином Media Cleaner](https://www.wordpress-abc.ru/plaginy/media-file-cleaner-plagin-wordpress-dlya-chistki-media-library.html).

Игорь Серов специально для сайта «[Как сделать сайт WordPress](https://www.wordpress-abc.ru/)»

### Другие статьи по теме

- [2 отличных и 1 известный сервисы проверки уникальности текстов](https://www.wordpress-abc.ru/seo-wordpress/servisyi-proverki-unikalnosti-tekstov.html)
- [Битые ссылки на WordPress сайте](https://www.wordpress-abc.ru/seo-wordpress/bityie-ssyilki-na-wordpress-sayte.html)
- [Как убирать ссылки автора темы WordPress  ](https://www.wordpress-abc.ru/seo-wordpress/kak-ubirat-ssyilki-avtora-temy-wordpress.html)
- [Разница между рубриками и метками WordPress](https://www.wordpress-abc.ru/seo-wordpress/raznitsa-mezhdu-rubrikami-metkami-wordpress.html)
- [Форматы записей WordPress](https://www.wordpress-abc.ru/administrirovanie/oformlenie-statej/formatyi-zapisey-wordpress.html)
- [Вставить видео с YouTube в WordPress](https://www.wordpress-abc.ru/administrirovanie/oformlenie-statej/vstavit-video-s-youtube-v-wordpress.html)