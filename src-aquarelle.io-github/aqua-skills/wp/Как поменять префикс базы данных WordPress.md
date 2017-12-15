# Как поменять префикс базы данных WordPress

[Главная](https://www.wordpress-abc.ru/) » [Хостинг](https://www.wordpress-abc.ru/hosting) » Как поменять префикс базы данных WordPress

![поменять префикс базы данных Wordpress](https://www.wordpress-abc.ru/wp-content/uploads/2014/09/prefiks-bazyi-danyih-wordpress.png)

По умолчанию все таблицы базы данных WordPress имеют префикс wp_. Если вы не задали другой префикс при установке системы система присвоит именно этот префикс базе данных и соответственно всем её таблицам. Для повышения безопасности сайта и практической защиты от хакерских SQL инъекций, принято менять префикс базы данных WordPress, и задавать произвольный набор букв и цифр. Не знаю почему, но система рекомендует длину префикса в четыре символа. Поменять префикс базы данных WordPress можно несколькими способами, о которых и пойдет речь в этой статье.

Для начала разберемся, зачем, вообще, менять префикс базы данных.

Содержание

- [Зачем менять префикс базы данных WordPress](https://www.wordpress-abc.ru/hosting/kak-pomenyat-prefiks-bazyi-dannyih-wordpress.html#___WordPress)
- [Замена префикса базы данных в phpMyAdmin](https://www.wordpress-abc.ru/hosting/kak-pomenyat-prefiks-bazyi-dannyih-wordpress.html#___phpMyAdmin)
- [Замена префикса базы данных в текстовом редакторе](https://www.wordpress-abc.ru/hosting/kak-pomenyat-prefiks-bazyi-dannyih-wordpress.html#i)
- [Редакция файла wp-cofig.php](https://www.wordpress-abc.ru/hosting/kak-pomenyat-prefiks-bazyi-dannyih-wordpress.html#_wp-cofigphp)

## Зачем менять префикс базы данных WordPress

Ответ, на вопрос, Зачем менять префикс базы данных WordPress, до банальности прост: Чтобы усложнить взлом сайта. Кроме этого, на одной базе данных можно запустить несколько копий сайта WordPress, и у каждой копии должна быть своя база данных со своим префиксом.

По умолчанию, при [установке WordPress](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-na-xosting.html) задается префикс базы данных wp_.  Его можно поменять, еще на этапе установки WordPress.

[![поменять префикс базы данных WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2014/09/prefiks-BD-wordpress-4_0-640x422.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2014/09/prefiks-BD-wordpress-4_0-640x422.jpg)

[Читайте так же:  Перенос сайта Wordpress на другой хостинг](https://www.wordpress-abc.ru/hosting/perenos-sajta-wordpress-na-drugoj-xosting.html)

Но, при установке, вы могли этого не сделать или не знали, что это лучше сделать. Будем считать, что нужно поменять префикс на рабочем сайте WordPress.

Не нужно устанавливать лишние плагины для изменения префикса БД. Это лишнее. Конечно, если установили плагин безопасности, в котором есть инструмент замены префикса базы данных, то этот вопрос решен. Например, в плагине безопасности iThemes Security есть такой инструмент. А вот как изменить префикс базы данных без плагинов, так сказать «руками» разберем дальше.

> Самый простой и надежный способ внизу статьи. Можете сразу идти туда.

## Замена префикса базы данных в phpMyAdmin

Если на вашем сервере есть phpMyAdmin, то можно поменять префикс БД там.

- Войдите панель вашего хостинга, а из нее в  phpMyAdmin. Откройте [базу данных](https://www.wordpress-abc.ru/hosting/baza-dannyih-wordpress.html)вашего сайта WordPress.
- Отметьте все таблицы (внизу есть поле «Отметить все»).
- Далее в фильтре действий выберите «Изменить префикс БД».

[![префикс-БД-wordpress-foto5](https://www.wordpress-abc.ru/wp-content/uploads/2014/09/prefiks-BD-wordpress-foto5.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2014/09/prefiks-BD-wordpress-foto5.jpg)

Для префикса можно использовать любой набор латинских букв и цифр. Если хотите совсем зашифроваться, используйте любой инструмент формирования паролей и сформируйте префикс в виде пароля. Например, в таком виде:  E2g2yJ3J.

Но это еще не все. В таблицах базы данных нужно найти все таблицы с префиксом wp_, которые не видны в обзоре таблиц. Это особенно важно, для таблицы  «wp_usermeta». Алгоритм простой, ищите все таблицы с префиксом «wp_»  и меняете на свой префикс.

[![префикс-БД-wordpress-foto4](https://www.wordpress-abc.ru/wp-content/uploads/2014/09/prefiks-BD-wordpress-foto4.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2014/09/prefiks-BD-wordpress-foto4.jpg)

[Читайте так же:  Пользователи Wordpress: группы и роли пользователей](https://www.wordpress-abc.ru/administrirovanie/polzovateli-wordpress.html)

Как видите, замена  префикса базы данных в [phpMyAdmin](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html) хоть и не сложное занятие, но требует некоторого навыка. Поэтому поменяем префикс, немного по-другому.

## Замена префикса базы данных в текстовом редакторе

Считаем, что резервная копия БД и сайта у вас уже сделана.

- Идем в phpMyAdmin.
- Открываем структуру базу данных сайта.
- Делаем копию базы данных без сжатия, в формате sql. Кнопка «Экспорт» в панели инструментов.

[![префикс-БД-wordpress-foto2](https://www.wordpress-abc.ru/wp-content/uploads/2014/09/prefiks-BD-wordpress-foto2.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2014/09/prefiks-BD-wordpress-foto2.jpg)

- Открываете файл базы данных sql, в текстовом редакторе, например Notepad++.
- Поиском в редакторе ищите «wp_» и меняете на свой префикс.
- Сохраняете отредактированный файл.
- Идете, назад, в phpMyAdmin.
- Удаляете старую БД ( выделяете все таблицы и удаляете отмеченные).
- Заливаете отредактированный файл sql, на сервер. Кнопка «Импорт» в панели инструментов.

[![префикс-БД-wordpress-foto2](https://www.wordpress-abc.ru/wp-content/uploads/2014/09/prefiks-BD-wordpress-foto2.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2014/09/prefiks-BD-wordpress-foto2.jpg)

[![поменять префикс базы данных WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2014/09/prefiks-BD-wordpress-foto3.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2014/09/prefiks-BD-wordpress-foto3.jpg)

[Читайте так же:  Общие советы по оптимизации сайта](https://www.wordpress-abc.ru/seo-nachinayushhim/obshhie-sovetyi-po-optimizatsii-sayta.html)

Все база данных с новым префиксом залита на сервер. Осталось отредактировать файл wp-cofig.php, сайта.

## Редакция файла wp-cofig.php

*Редактировать файл wp-config.php нужно при любом варианте изменения префикса.*

- По FTP заходите в каталог сайта.
- Копируете файл wp-cofig.php на компьютер и открываете его для редактирования в текстовом редакторе.
- Ищите строку (№62) и меняет старый префикс «wp_» на новый префикс.

[![префикс-БД-wordpress-foto6](https://www.wordpress-abc.ru/wp-content/uploads/2014/09/prefiks-BD-wordpress-foto6.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2014/09/prefiks-BD-wordpress-foto6.jpg)

- Сохраняете отредактированный файл в кодировке «кодировать в UTF-8 без BOM» и заливаете его по FTP обратно в каталог сайта, в режиме перезаписи.

Все готово. Теперь вы знаете, как поменять префикс базы данных WordPress

*Понятно, что исходный префикс может быть любой, и не обязательно «wp_» и менять префикс можно несколько раз.*

Игорь Серов специально для сайта «[Как сделать сайт WordPress](https://www.wordpress-abc.ru/)»

### Другие статьи раздела: Хостинг для WordPress

- Записи не найдены