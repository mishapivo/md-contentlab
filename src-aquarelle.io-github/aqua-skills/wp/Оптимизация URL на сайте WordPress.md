# Оптимизация URL на сайте WordPress

[Главная](https://www.wordpress-abc.ru/) » [Администрирование](https://www.wordpress-abc.ru/administrirovanie) » Оптимизация URL на сайте WordPress

![img](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/sef-wordpress.jpg)

Оптимизация URL на сайте WordPress нужна для того, чтобы адрес сайта не состоял из набора не читаемых знаков и цифр, а был читаемым и четко указывал на содержание статьи. Настройка URL на сайте WordPress называется  оптимизацией URL и является обязательным элементом общей SEO оптимизацией сайта. В этой статье я расскажу, как привести URL адреса сайта в удобный вид для поисковых машин и человека.

**Содержание статьи:**

- Структура URL-адресов;
- Создание своих шаблонов для ссылок в WordPress;
- Настройки постоянных ссылок на сайте WordPress;
- Обновление файла [.htaccess] после изменения структуры URL;
- Шаблон категорий и тегов WordPress;
- Плагин перевода URL **Cyr-to-Lat**.

Но вначале немного об URL.

Содержание

- Структура URL-адресов
  - [КАК искать адрес URL](https://www.wordpress-abc.ru/administrirovanie/optimizaciya-url-na-sajte-wordpress.html#__URL)
  - [ГДЕ искать адрес URL](https://www.wordpress-abc.ru/administrirovanie/optimizaciya-url-na-sajte-wordpress.html#__URL-2)
  - [ЧТО искать по адресу URL](https://www.wordpress-abc.ru/administrirovanie/optimizaciya-url-na-sajte-wordpress.html#__URL-3)
- [URL адреса WordPress](https://www.wordpress-abc.ru/administrirovanie/optimizaciya-url-na-sajte-wordpress.html#URL_WordPress)
- [Оптимизация URL на сайте WordPress](https://www.wordpress-abc.ru/administrirovanie/optimizaciya-url-na-sajte-wordpress.html#_URL__WordPress)
- Создание своих шаблонов для постоянных ссылок WordPress
  - Оптимизация URL на сайте WordPress настройками постоянных ссылок
    - [Ниже приведу список тегов для шаблона URL wordpress](https://www.wordpress-abc.ru/administrirovanie/optimizaciya-url-na-sajte-wordpress.html#___URL_wordpress)
  - [Шаблон категорий и тегов по умолчанию](https://www.wordpress-abc.ru/administrirovanie/optimizaciya-url-na-sajte-wordpress.html#i)
  - Обновление файла .htaccess после изменения структуры URL
    - [Вот содержание файла .htaccess по умолчанию для WP](https://www.wordpress-abc.ru/administrirovanie/optimizaciya-url-na-sajte-wordpress.html#__htaccess__WP)
- [Решает перевод URL плагин Cyr-to-lat](https://www.wordpress-abc.ru/administrirovanie/optimizaciya-url-na-sajte-wordpress.html#_URL_Cyr-to-lat)

## Структура URL-адресов

Аббревиатура URL (Uniform Resource Locator) это не более чем интернет адрес, какой либо информации размещенной в сети WWW (World Wide Web). Общая структура любого URL адреса показывает поисковым машинам, КАК, ГДЕ И ЧТО или КОГО искать в сети.

[Читайте так же:  Смена имени пользователя Wordpress](https://www.wordpress-abc.ru/administrirovanie/smena-imeni-polzovatelya-wordpress.html)

### КАК искать адрес URL

http, WAIS, file, telnet , gopher,ftp  все это протоколы доступа или метод поиска в сети. Синтаксис любого протокола поиска (**://**).Например:

(http://) или (file://)

### ГДЕ искать адрес URL

Это имя вашего домена на доменном узле хостинга, входящего в систему DNS. Синтаксис общеизвестен:

(www.vashdomain.net) или (vashdomain.net)

### ЧТО искать по адресу URL

Полный URL это прямой путь к информации, иначе это прямой путь к файлу с информацией на сервере вашего хостинга. Для любой страницы на сайте полный URL имеет следующую структуру:

httр://vashdomain.net/patch/имя статьи

Переменные значения в любом URL адресе это (patch/имя статьи), где patch это путь от корневого каталога сайта до статьи по созданной вами структуре сайта, из категорий (рубрик) и подрубрик. Все это и есть полный адрес любой статьи на вашем сайте WP. Если точнее, это преобразованный адрес статей сайта для отображения в адресной строке браузера. Именно по этому адресу, поисковики будут искать вашу статью, размещенную на сайте.

[Читайте так же:  Как создать меню Wordpress, простое и выпадающее меню WP](https://www.wordpress-abc.ru/administrirovanie/kak-sozdat-menyu-wordpress-prostoe-i-vypadayushhee-menyu-wp.html)

## URL адреса WordPress

URL адреса на WordPress называют постоянные ссылки (permalink). По умолчанию, то есть после установки, WordPress преобразовывает URL любой статьи в смесь цифр и знаков, которые визуально человеку не о чем не говорят. Кроме этого такие шифрованные URL не только непонятны человеку, но и для поисковиков они не связывают статью, ни со структурой сайта, ни с ключевыми словами, ни с темой сайта.

## Оптимизация URL на сайте WordPress

Оптимизация URL на сайте WordPress это изменение URL адреса статьи для понимания их человеком и лучшей индексации поисковыми машинами. Понятные для человека URL адреса носят название **SEF URL или ЧПУ (человекопонятные урлы)**, а оптимизация носит название SEF («search engine friendly») или ЧПУ оптимизация.

Оптимизация URL на сайте WordPress может проходить двумя принципиально разными способами.

1. Первый способ это оптимизация внутренними инструментами WordPress;
2. Второй способ это оптимизация сторонними плагинами, носящими название SEO плагины.

Оптимизация URL на сайте WordPress это хоть и небольшая, но очень важная часть общего SEO сайта (SEO -процесс улучшения рейтинга сайта в результатах поиска в Интернете).
Оптимизация URL на сайте WordPress принципиально отличается для новых (пустых) сайтов и для сайтов наполненных статьями, которые уже проиндексированы поисковиками.

В этой рассмотрим,  как можно настроить вид URL статей в «удобный» для поисковиков и человека вид, на чистых сайтах. Под чистым сайтом понимаем сайт без статей сразу после [установки WordPress](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-na-xosting.html).

[Читайте так же:  Вставляем произвольный код в посты и страницы WordPress](https://www.wordpress-abc.ru/plaginy/vstavlyaem-proizvolnyiy-kod-v-postyi-i-stranitsyi-wordpress.html)

## Создание своих шаблонов для постоянных ссылок WordPress

Все URL адреса в WordPress называются ссылками. Внешний вид адресов называют шаблоном ссылок. С помощью внутренних инструментов оптимизации, шаблон можно задать для всех статей и архивов сайта одновременно.

Настройка внешнего вида URL находится по пути: *Консоль →Параметры → Постоянные ссылки.*

[![Оптимизация URL на сайте WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-05.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-05.jpg)

Открыв пункт «Постоянные ссылки» видим окно, которое нам нужно. Это окно — «Настройки постоянных ссылок».

### Оптимизация URL на сайте WordPress настройками постоянных ссылок

По умолчанию WordPress отображает ссылки на статьи и архивы сайта в виде набора цифр и знаков. Выглядит это приблизительно так:

[![optimizatciy-url-wordpress-04](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-04.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-04.jpg)

В настройках «Постоянные ссылки» это первый вид шаблона URL, который так и называется «По умолчанию».

Следующие четыре пункта в списке, позволяют настроить все URL сайта по четырем определенным шаблонам.

[![optimizatciy-url-wordpress-07](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-07-381x400.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-07.jpg)

Интересен последний пункт настроек **«Произвольно»**.

В этом пункте можно самостоятельно сформировать шаблон URL адресов статей сайта (постоянных ссылок). Для этого WordPress предлагает серию тегов. Каждый тег будет отображать в URL определенную принадлежность и расположение статьи на сайте.

#### Ниже приведу список тегов для шаблона URL wordpress

- %year%Год сообщения,четыре цифры,
- %monthnum% Месяц года,
- %day% День месяца,
- %hour% Час дня,
- %minute% Минута часа,
- %second% Секунда
- %post_id% Уникальный ID # поста,
- %postname% Облагороженная версия названия статьи (название статьи в поле Edit Post)
- %category% Облагороженная версия названия категории. Вложенные подкатегории отображаются в виде вложенных каталогов в URI.
- %author% Облагороженное имя автора

[![optimizatciy-url-wordpress-10](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-10-400x158.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-10.jpg)

Располагать теги можно произвольным образом. Как построите шаблон ссылки, так она и будет отображаться. Если в пункт «Произвольно» ввести все теги из списка,то URL будет выглядеть так:

[![optimizatciy-url-wordpress-11](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-11-400x94.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-11.jpg)

Но для оптимизации сайта WordPress нужно сформировать шаблон URL в разумном виде, повторяющим структуру вашего сайта. Например: www.vashdomain.net/рубрика/название статьи, в шаблоне постоянных ссылок с тегами это выглядит так:

httр://www.vashdomain.net/%category%/%postname%

[![optimizatciy-url-wordpress-12](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-12-400x265.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-12.jpg)

[![optimizatciy-url-wordpress-15](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-15-400x126.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-15.jpg)

Для сайтов с большим количеством похожего материала, можно добавить в шаблон URL тег с индивидуальным номером (ID) статей (тег  **%post_id%**).

**Важно!** Заканчиваться шаблон URL должен тегом %post_id% или %postname%.

Если статья публикуется в категории с родительскими категориями, то в URL будет отражаться последняя категория. Это правило может не работать,если вы используете на сайте [SEO плагины](https://www.wordpress-abc.ru/seo-wordpress/4-luchshix-seo-plagina-wordpress.html) и в URL могут показываться все родительские категории статьи. В SEO плагинах шаблоны URL настраиваются по своему.

**Примечание:** При настройке вида постоянной ссылки нужно учесть следующее:

- Если в ссылку добавить дату выхода статьи, то вы не сможете перевыпустить статью через некоторое время. Например, статья через год или пару лет устареет, но тема будет востребована. Если отредактировать статью и обновить дату выпуска, то сменится URL статьи и она выпадет из индекса.
- Многие веб мастера, советуют делать шаблон постоянных сыылок, как **%category%/%postname%. **Такой шаблон ссылокдает хорошее предстваление о структуре сайта, но вы не сможете переносить статью из раздела в раздел, что бы она не выпадала из индеска.** **
- И еще одно. Как бы вы не меняли статью и её заголовок, единственное, что у неё не изменится это ID статьи (её уникальный номер).

### Шаблон категорий и тегов по умолчанию

По умолчанию шаблоны URL категорий и тегов МОГУТ выделяться префиксами category и tag. Выглядят это так:

- example.net/category/category_name
- example.net/tag/tag_name

, но их можно изменить в **дополнительных настройках** «Постоянные ссылки». Если ничего не заполнить, то в URL разделов и тегов будут отражаться префиксы по умолчанию.

[![optimizatciy-url-wordpress-20](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-20-400x153.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-20.jpg)

### Обновление файла .htaccess после изменения структуры URL

После каждого обновления структуры URL, движок WordPress в автоматическом режиме должен обновлять файл .htaccess. Для этого права владения на этот файл должен быть 666. Но постоянно такие права CHMOD устанавливать не стоит. Это серьезно ослабит безопасность сайта. Стандартные права на файлы системы должны быть 644.

Если система имеет доступ к файлу  .htaccess, то она сама переделает этот файл в соответствии с вашим шаблоном URL. Если системе не хватает прав на изменение файла, то она предложит скопировать новое содержание файла .htaccess, которое появится внизу окна настроек «Постоянные ссылки»

[![optimizatciy-url-wordpress-06](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-06-400x212.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-06.jpg)

и заменить им старое содержание файла .htaccess. Файл .htaccess находится в корневом каталоге вашего сайта, в папке (publ_html) или (httpdocs).

Если у вас нет файла **.htaccess** ,то для работы настройки «Постоянные ссылки» его нужно создать. Создайте его в текстовом редакторе Notepad++, под любым именем, например: Ahtaccess.txt, загрузите в корневую папку сайта и переименуйте в файл .htaccess.

#### Вот содержание файла .htaccess по умолчанию для WP

Если вы настроили всё правильно, то теперь URL статей будут отражаться по вашему шаблону, но русскими буквами. В принципе, на сегодня, поисковики читают русские названия статей и категорий в URL. Но традиционно лучше, чтобы названия в URL отражались в переводе транслит на латиницу.

## Решает перевод URL плагин Cyr-to-lat

Устанавливаете его на сайт одним из [удобных способов установки плагинов](https://www.wordpress-abc.ru/plaginy/ustanovka-plagina-na-wordpress.html). Все! Настройки [плагин Cyr-to-lat](https://www.wordpress-abc.ru/plaginy/kak-perevesti-url-adresa-wordpress-iz-kirillitsyi-v-latinitsu.html) не требует. Укажите только стандарт перевода URL. Если оставить настройки по молчанию плагин начнет работать сразу после установки.

[![optimizatciy-url-wordpress-17](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-17.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-17.jpg)

Важно! Плагин Rus-to-lat не будет переводить URL уже написанных статей. Он начинает работать только для статей написанных после его установки.

После написания новых статей URL статей будет выглядеть так:

[![optimizatciy-url-wordpress-19](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-19.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/optimizatciy-url-wordpress-19.jpg)

На этом дефолтная оптимизация URL на сайте WordPress завершена!

Игорь Серов специально для сайта «[Как сделать сайт WordPress](https://www.wordpress-abc.ru/)»

### Другие статьи раздела: Администрирование WordPress

- Записи не найдены