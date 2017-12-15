# Favicon для сайта WordPress

[Главная](https://www.wordpress-abc.ru/) » [Администрирование](https://www.wordpress-abc.ru/administrirovanie) » Favicon для сайта WordPress

![img](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/wordpress-favicon.png)

Содержание

- [Вступление](https://www.wordpress-abc.ru/administrirovanie/favicon-dlya-sajta-wordpress.html#i)
- favicon для сайта WordPress: этапы установки
  - [Сделать картинку favicon.ico на любом генераторе favicon](https://www.wordpress-abc.ru/administrirovanie/favicon-dlya-sajta-wordpress.html#_faviconico__favicon)
  - [Загрузить картинку favicon.ico в корневой каталог сайта](https://www.wordpress-abc.ru/administrirovanie/favicon-dlya-sajta-wordpress.html#_faviconico)
  - [Разместить код в файле functions.php](https://www.wordpress-abc.ru/administrirovanie/favicon-dlya-sajta-wordpress.html#__functionsphp)

## Вступление

Favicon для сайта WordPress (favorites icon) или иконка сайта, придает сайту индивидуальность и, через узнаваемость закладок, может влиять на его посещаемость. Однако, неудачно установленный **favicon** может увеличивать время загрузки сайта. В этой статье рассмотрим установку иконки сайта через файл functions.php.

## favicon для сайта WordPress: этапы установки

Одним из вариантов установки иконки является размещение иконки в корневом каталоге, с добавлением кода в файл functions.php. Для этого способа установки favicon на сайт нужно сделать три шага.

- Сделать картинку favicon.ico на любом генераторе favicon;
- Загрузить картинку favicon.ico в корневой каталог сайта;
- Поместить код в файле functions.php.

Остановимся на каждом шаге подробнее.

### Сделать картинку favicon.ico на любом генераторе favicon

В статье [«Установка иконки favicon на сайт WordPress»](https://www.wordpress-abc.ru/plaginy/ustanovka-ikonki-favicon-na-sajt-wordpress.html) я подробно рассказывал, как сделать картинку favicon.ico. В этом нет ничего сложного. Делается она на любом генераторе иконок, в режиме on-line. Не требуется устанавливать на компьютер дополнительных программ. Делается картинка в формате .ico из картинки любого размера и любого формата.

Если вы хотите сами нарисовать свою иконку, можно воспользоваться расширенным online сервисом для изготовления иконок **favicon.cc. **На нем можно не только сделать иконку из заранее подготовленной фотографии, но и попробовать себя в точечном рисовании.

[![Favicon для сайта WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/WP-favicon-kod-v-function-php-3-400x199.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/WP-favicon-kod-v-function-php-3.jpg)

[![WP-favicon-kod-v-function-php-2](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/WP-favicon-kod-v-function-php-2-400x269.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/WP-favicon-kod-v-function-php-2.png)

Еще один расширенный инструмент для создания иконок это **favicon.ru**.На нем можно не только рисовать, но и заказать изготовление уникального favicon.

[![Favicon для сайта WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/WP-favicon-kod-v-function-php-4-400x216.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/WP-favicon-kod-v-function-php-4.jpg)

Будем считать, что свой favicon вы сделали. Будем размещать его на сайте.

Мало? Держите список сервисов для создания иконок:

[Читайте так же:  Метки Wordpress, как с ними работать](https://www.wordpress-abc.ru/administrirovanie/metki-wordpress-kak-s-nimi-rabotat.html)

•  iconfinder.com
•  freepik.com/free-icons
•  fian.my.id
•  ru.iconka.com
•  genericons.com
•  materialdesignicons.com
•  flaticons.net
•  iconbird.com
•  iconizer.net
•  webhostinghub.com
•  iconspedia.com
•  iconsearch.ru
•  icons8.com
•  glyphicons.com
•  findicons.com
•  icomoon.io
•  iconarchive.com
•  themify.me
•  fontawesome.io
•  thenounproject.com
•  flaticon.com
•  fontello.com

### Загрузить картинку favicon.ico в корневой каталог сайта

Сделанный Favicon для сайта WordPress, при помощи FTP соединения, закачиваем в корневой каталог вашего сайта, скорее всего в папку [publ-html] или [httpdocs].

Проверьте, чтобы в этой папке не было старых иконок. Если они есть,  удалите их. Жалко удалять, переименуйте. Также проверьте папку с рабочим шаблоном. Из нее также удалите файл ico если есть.

### Разместить код в файле functions.php

Остается поместить код в шаблоне сайта. Для этого авторизуемся в административной панели. В консоли открываем: Внешний вид →Редактор.

В редакторе справа из списка файлов шаблона доступных для редактирования, ищем файл [functions.php]. Открываем его для редактирования. Не забывайте, перед редактированием сделать резервную копию сайта. Также, без опыта, редактируйте файлы на из консоли, а в любом текстовом редакторе, например, Notepad++.

В любое место раздела THEME SETUP вставляем следующий код

```
// add a favicon to your
function my_favicon() {
echo '<link rel="shortcut Icon" type="image/x-icon"
 href="'.get_bloginfo('wpurl').'/favicon.ico" />';
}
add_action('wp_head', 'my_favicon');
```

[![WP-favicon-kod-v-function-php-1](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/WP-favicon-kod-v-function-php-1-400x351.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/02/WP-favicon-kod-v-function-php-1.png)

**Не забываем сохраняться.**

После перегрузки страницы сайта иконка появляется рядом с вашим сайтом. Если вы удалили все «чужие» иконки из каталога сайта, включая каталоги тем, а ваша иконка все равно не появляется, очистите кэш вашего браузера.

На этом все! Тему Favicon для сайта WordPress закрываю. На сайте получились три статьи, где я рассказывал о трех вариантах установки уникальной иконки на свой сайт WP. Читать другие статьи:

- [Установка иконки favicon на сайт WordPress](https://www.wordpress-abc.ru/plaginy/ustanovka-ikonki-favicon-na-sajt-wordpress.html),
- [Плагины WP для установки favicon (иконок) на сайт WordPress](https://www.wordpress-abc.ru/plaginy/plaginy-wp-dlya-ustanovki-favicon-ikonok-na-sajt-wordpress.html)

[Читайте так же:  Изображения, фото и галереи в статьях Wordpress](https://www.wordpress-abc.ru/administrirovanie/izobrazheniya-foto-i-galerei-v-statyax-wordpress.html)

 

©www.wordpress-abc.ru

### Другие статьи раздела: Администрирование WordPress

- Записи не найдены