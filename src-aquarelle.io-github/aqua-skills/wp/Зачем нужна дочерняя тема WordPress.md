# Зачем нужна дочерняя тема WordPress

[Главная](https://www.wordpress-abc.ru/) » [Шаблоны WP](https://www.wordpress-abc.ru/temy-wordpress) » Зачем нужна дочерняя тема WordPress

![дочерняя тема wordpress](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/dochernyaya-tema-wordpress.jpg)

WordPress всегда удивляла меня скрытыми возможностями. И удивляла не столько наличием этих возможностей, сколько простотой их реализации. Конечно, скрытые возможности не относятся к великим тайнам системы, просто до поры до времени, ты даже не знаешь, что «такое» можно сделать на WordPress. Доступность для редактирования кодов рабочих тем WordPress, позволяют изменять и дополнять внешний вид сайта от смены оформления до создания дополнительных виджетов и плагинов. Только есть одно маленькое неудобство: любые прямые корректировки кода темы, исчезают, а вернее возвращаются к первоисточнику, после каждого обновления шаблона. Чтобы избежать таких откатов, создается дочерняя тема WordPress, которая позволяет редактировать код  темы без угрозы потерять все изменения при плановом обновлении. О создании дочерней темы WordPress  и пойдет речь далее.

Содержание

- [Что такое дочерняя тема WordPress](https://www.wordpress-abc.ru/temy-wordpress/zachem-nuzhna-dochernyaya-tema-wordpress.html#__WordPress)
- [Создаем дочернюю тему WordPress – практический пример](https://www.wordpress-abc.ru/temy-wordpress/zachem-nuzhna-dochernyaya-tema-wordpress.html#__WordPress-2)
- [Как наполнить дочернюю тему](https://www.wordpress-abc.ru/temy-wordpress/zachem-nuzhna-dochernyaya-tema-wordpress.html#i)
- Другие файлы темы
  - [Другие стати раздела: Установка WordPress](https://www.wordpress-abc.ru/temy-wordpress/zachem-nuzhna-dochernyaya-tema-wordpress.html#__WordPress-3)

## Что такое дочерняя тема WordPress

Дочерняя [тема WordPress](https://www.wordpress-abc.ru/uroki-wordpress/chto-takoe-tema-wordpress.html) (child theme, тема-потомок) это инструмент, позволяющий вносить любые корректные изменения внешнего вида (редакция файла style.css) и функционала сайта (файлы functions.php и другие файлы шаблона) и не потерять редакции при обновлении шаблона.

Стили и разметка темы родителя подкачиваются в тему потомок, а изменения в child theme наслаиваются на них. Все изменения мы вносим в дочернюю тему, а основная тема остается неизменной.

[Читайте так же:  Вышла новая версия 4,3 WordPress](https://www.wordpress-abc.ru/novosti/vyishla-novaya-versiya-4-3-wordpress.html)

## Создаем дочернюю тему WordPress – практический пример

Напомню, все темы системы «лежат» в каталоге wp-content/themes. Далее по шагам.

- В каталоге themes создаем папку с произвольным названием дочерней темы. Для примера создаю папку: first-child-theme. Название нам скоро понадобится.
- В любимом текстовом редакторе (я использую Notepad++) создаем текстовой файл с расширением css и названием style. Название не меняем, а содержание файла должно содержать, пока, только заголовок:

Здесь, важна только, последняя строка, это название папки с родительской темой. Именно из нее, система будет подкачивать стили шаблона.

- Файл сохраняем и заливаем в папку дочерней темы, first-theme.
- В консоли сайта появляется дочерняя тема. Название совпадает с названием указанным в строке: Theme Name. При открытии темы показывается  указанное описание темы — строка Description.

[![дочерняя тема wordpress](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/dochernyaya-tema-wordpress-1-400x199.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/dochernyaya-tema-wordpress-1.jpg)

[![дочерняя-тема-wordpress-2](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/dochernyaya-tema-wordpress-2-400x193.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/dochernyaya-tema-wordpress-2.jpg)

[Читайте так же:  Почтовая служба WordPress.com, бесплатная рассылка на любом WordPress сайте](https://www.wordpress-abc.ru/administrirovanie/nastrojki-wordpress/pochtovaya-sluzhba-wordpress-com.html)

Тема еще пустая и нужно ее наполнить и активировать. Можно наоборот: активировать, а потом наполнить.

## Как наполнить дочернюю тему

Напоминаю задачу, нам не нужна пустая дочерняя тема, а нужна тема, дублирующая родительскую тему, чтобы в ней менять стили и разметку.

Для дублирования темы выбираем из двух вариантов исполнения:

- Копируем родительский файл style.css и переносим его в аналогичный файл дочерней темы (пока он всего один).
- Или в  файле style.css дочерней темы вписываем дополнительную строку:

```
@import url(“../zeefocus/style.css”);<\pre>
```

Где, zeefocus – основная, родительская тема.

[![дочерняя-тема-wordpress-4](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/dochernyaya-tema-wordpress-4.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/dochernyaya-tema-wordpress-4.jpg)

[Читайте так же:  Метки Wordpress, как с ними работать](https://www.wordpress-abc.ru/administrirovanie/metki-wordpress-kak-s-nimi-rabotat.html)

Важно!

Этой строкой мы подгружаем стили основной темы. Теперь, не нужно копировать файл стиля, можно вносить изменения в пустой файл дочерней темы и он будет записываться поверх стилей основной темы. Редактировать style.css можно из админки сайта на вкладке Внешний вид→Редактор.

Не забываем, функцию import вынести из заголовка файла style.css.

[![дочерняя-тема-wordpress-3](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/dochernyaya-tema-wordpress-3.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/dochernyaya-tema-wordpress-3.jpg)

## Другие файлы темы

Опять два варианта,

- создаем пустые файлы с аналогичными названиями пустым содержимым: (<?php …. ?>) и пишим их, как нужно;
- или, проще, переносим файлы основной темы в дочернюю тему и их редактируем, как нужно.

Игорь Серов, специально для сайта «[Как создать сайт WordPress](https://www.wordpress-abc.ru/)»

### Другие стати раздела: Установка WordPress

- Записи не найдены