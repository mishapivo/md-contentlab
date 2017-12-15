# Практичные SQL запросы к базе данных WordPress

[Главная](https://www.wordpress-abc.ru/) » [Хостинг](https://www.wordpress-abc.ru/hosting) » Практичные SQL запросы к базе данных WordPress

![img](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/wordpress-SQL.jpg)

Содержание

- [Вступление](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html#i)
- [Как сделать SQL запрос](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html#_SQL)
- SQL запросы к базе данных WordPress
  - [Удалить все ревизии статей](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html#i-2)
  - [Изменить URL главной страницы и URL сайта](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html#URL__URL)
  - [Изменить индетификатор URL (GUID)](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html#_URL_GUID)
  - [Изменить URL в контенте](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html#_URL)
  - [Изменить URL картинок](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html#_URL-2)
  - [Смена Meta информации сообщений](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html#_Meta)
  - [Изменение имени пользователя «Admin»](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html#__171Admin187)
  - [Смена пароля WordPress](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html#_WordPress)
  - [ Поменять автора статей](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html#i-3)
  - [Удаление следов плагинов WordPress](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html#__WordPress)
  - [Удаление всех пингбеков (pingback)](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html#__pingback)
  - [Удаление всех СПАМ комментариев](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html#i-4)
  - [ Найти неиспользуемые теги](https://www.wordpress-abc.ru/hosting/praktichnyie-sql-zaprosyi-k-baze-dannyih-wordpress.html#i-5)

## Вступление

SQL запросы к базе данных WordPress позволяют без лишних плагинов осуществить действие применимое ко всему содержанию сайта. Кроме копирования, удаления отдельных таблиц и всей базы в целом, SQL запросы позволяют менять URL страниц, менять автора, менять пароли, удалять устаревшую информацию и т.п.

## Как сделать SQL запрос

SQL это специальный структурированный язык запросов ((Structured Query Language) для работы с базами данных.

Сделать SQL запрос у БД можно в панели управления базой данных, phpMyAdmin. Для этого войдите в    phpMyAdmin из административной панели хостинга, используя имя и пароль пользователя этой базы данных. Панель откроется в браузере.

Далее откройте нужную базу данных, нажав на  кнопку «Структура». Чтобы сделать SQL запрос воспользуйтесь кнопкой SQL запрос.

[![SQL запросы к базе данных WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/SQL_zapros.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/SQL_zapros.png)

## SQL запросы к базе данных WordPress

Во всех приведенных примерах Полезные SQL запросы к базе данных WordPress, делаются к базе данных с префиксом wp_. Чтобы использовать приведенные запросы к своей базе данных, измените префикс wp_ на префикс своей БД. На некоторых фото префикс wp_ заменен на wop_.

### Удалить все ревизии статей

При редактировании статей WordPress, система сохраняет в базе данных все ревизии статей. Парой их скапливается до нескольких тысяч.

[![Ревизии_статей](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/Revizii_statey.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/Revizii_statey.png)

Удалить ревизии статей из панели сайта нельзя. Поэтому, чтобы удалить все ревизии статей, которые скопились на данный момент, делаем следующий SQL запрос (вверху код):

```
DELETE a,b,c FROM wp_posts a
LEFT JOIN wp_term_relationships b ON (a.ID = b.object_id)
LEFT JOIN wp_postmeta c ON (a.ID = c.post_id)
WHERE a.post_type = 'revision'
```

После нажатия «ОК» видим результаты выполненного SQL запроса.

[![SQL запросы для WP](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/SQL-zaprosyi-dlya-WP-400x199.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/SQL-zaprosyi-dlya-WP.png)

[Читайте так же:  Перенести бесплатный сайт WordPress.com на коммерческий хостинг](https://www.wordpress-abc.ru/hosting/perenesti-besplatnyj-sajt-wordpress-com-na-kommercheskij-xosting.html)

### Изменить URL главной страницы и URL сайта

При переносе сайта WordPress с локального сервера меняется   URL главной страницы и URL сайта. Система WordPress сохраняет эти абсолютные URL в базе данных. После переноса сайта старые URL нужно удалить. Для этого сделайте следующий SQL запрос:

```
UPDATE wp_options SET option_value = replace(option_value,
 'http://www.СТАРЫЙУРЛ.com', 'http://www.НОВЫЙУРЛ.com') 
WHERE option_name = 'home' OR option_name = 'siteurl';
```

### Изменить индетификатор URL (GUID)

Каждый URL в базе данных имеет свой уникальный идентификатор (GUID -Globally Unique Identifier). После переноса сайта с локального компьютера или смене домена, нужно изменить URL в поле GUID в таблице wp_posts, сделав следующий SQL запрос

```
UPDATE wp_posts SET guid = REPLACE (guid, 'http://www.СТАРЫЙУРЛ.com', 
'http://www.НОВЫЙУРЛ.com');
```

### Изменить URL в контенте

Система WordPress сохраняет в базе данных и старые абсолютные пути ссылок сайта в базе данных. Их также нужно изменить:

```
UPDATE wp_posts SET post_content = REPLACE 
(post_content, 'http://www.СТАРЫЙУРЛ.com', 'http://www.НОВЫЙУРЛ.com');
```

### Изменить URL картинок

После [миграции сайта](https://www.wordpress-abc.ru/hosting/perenos-sajta-wordpress-na-drugoj-xosting.html) меняются и URL картинок в медиа библиотеке. Чтобы их поменять делаем следующий SQL запрос.

```
UPDATE wp_posts SET post_content = REPLACE (post_content, 
'src="http://www.СТАРЫЙУРЛ.com', 'src="http://www.НОВЫЙУРЛ.com');
```

Не забываем про GUID прикрепленных файлов.

```
UPDATE wp_posts SET  guid = REPLACE (guid, 
'http://www.СТАРЫЙУРЛ.com', 'http://www.НОВЫЙУРЛ.com') 
WHERE post_type = 'attachment';
```

### Смена Meta информации сообщений

Все аналогично смене URL

```
UPDATE wp_postmeta SET meta_value = REPLACE (meta_value, 
'http://www.СТАРЫЙУРЛ.com','http://www.НОВЫЙУРЛ.com');
```

### Изменение имени пользователя «Admin»

При [установке WordPress](https://www.wordpress-abc.ru/ustanovka-wordpress/ustanovka-wordpress-na-xosting.html) вы задаете имя и пароль для владельца сайта, администратора. Ранее по – умолчанию, система предлагала имя  «Admin». Чтобы [поменять имя «Admin»](https://www.wordpress-abc.ru/administrirovanie/smena-imeni-polzovatelya-wordpress.html), которое просто подарок взломщику, сделайте следующий SQL запросы к базе данных WordPress.

```
UPDATE wp_users SET user_login = 'НОВОЕ ИМЯ' WHERE user_login = 'Admin';
```

### Смена пароля WordPress

Потеряли пароль для авторизации, не беда. Можно сменить [пароль user](https://www.wordpress-abc.ru/administrirovanie/vosstanovit-parol-administratora-wordpress.html)(администратора) WordPress, делая следующий запрос SQL.

**Примечание:** MD5- способ кодирования. **Новый пароль вписывается в простом, не закодированном виде. **

```
UPDATE wp_users SET user_pass = MD5( 'НОВЫЙ ПАРОЛЬ' ) WHERE user_login = 'ВАШ ЛОГИН';
```

###  Поменять автора статей

Чтобы поменять автора  «А» на автора  «Б», сразу на всем сайте и не заниматься этим вручную, достаточно сделать следующие SQL запросы к базе данных WordPress.

```
UPDATE wp_posts SET post_author = 'НОВЫЙ АВТОР-id' WHERE post_author = 'СТАРЫЙ АВТОР-id';
```

Чтобы определить «Имя автора_id»  в  профиле автора наведите курсор на поле «Изменить» и внизу в адресной строке, посмотрите «user_id» (смотрим фото).

[![user_id](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/user_id-400x179.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/user_id.png)

[Читайте так же:  Бесплатный хостинг: понятие бесплатного хостинга, плюсы и минусы](https://www.wordpress-abc.ru/hosting/besplatnyiy-hosting-2.html)

### Удаление следов плагинов WordPress

Некоторые плагины после [удаления плагина](https://www.wordpress-abc.ru/uroki-wordpress/ustanovka-udalenie-plagina-na-wordpress.html) оставляют записи в таблице post_meta. Чтобы их удалить, сделайте следующий SQL запрос к БД:

```
DELETE FROM wp_postmeta WHERE meta_key = 'your-meta-key';
```

### Удаление всех пингбеков (pingback)

Пинкбек это уведомление о ссылке на веб-документ. В админке пинкбеки по умолчанию не выводятся. Однако  записываются в базе данных. Большое количество пинкбеков, загружают базу данных, и чтобы их  удалить делаем SQL запрос:

```
DELETE FROM wp_comments WHERE comment_type = 'pingback';
```

### Удаление всех СПАМ комментариев

Спам комментарии тоже пишутся в базу данных. Если вы пользуетесь плагином Akismet, то об удалении спам комментариев можно не беспокоиться. Однако их можно удалить и из панели phpMyAdmin, сделав следующий SQL запрос (ставим spam -удаляем спам; вместо spam ставим 0 — удаляем комментарии на одобрении; ставим  1 — удаляем одобренные комментарии):

```
DELETE FROM wp_comments WHERE comment_approved = 'spam';
```

###  Найти неиспользуемые теги

Теги к статьям одновременно помогают и вредят в  оптимизации сайта WordPress. Основной вред от тегов, создание дублей страниц. Именно из- за этого, теги закрывают от поисковиков, прописывая соответствующее правило в файле robots.txt или устанавливая SEO плагин WP.

Кроме этого теги не удаляются с удалением статей сайта. Чтобы найти не используемые теги сделайте следующий SQL запрос

```
SELECT * From wp_terms wt
INNER JOIN wp_term_taxonomy wtt ON wt.term_id=wtt.term_id 
WHERE wtt.taxonomy='post_tag' AND wtt.count=0;
```

, который и закроет  практичные SQL запросы к базе данных WordPress этой статьи.

[![теги](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/tegi-400x250.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/tegi.png)

[![теги-результат](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/tegi-rezultat-395x400.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/tegi-rezultat.png)

После этого удалите неиспользуемые теги войдя в административную панель сайта и сделайте повторный запрос для контроля:

[![SQL после чистки](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/SQL-posle-chistki-400x214.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/SQL-posle-chistki.png)

[Читайте так же:  Поиск хостинга и планирование бизнеса](https://www.wordpress-abc.ru/hosting/poisk-hostinga-i-planirovanie-biznesa.html)

Важно! Любое «общение» с базой данных WordPress, начните с создания резервной копии базы данных  для восстановления сайта в случае фатальных ошибок.

Игорь Серов специально для сайта «[Как сделать сайт WordPress](https://www.wordpress-abc.ru/)»

### Другие статьи раздела: Хостинг для WordPress

- Записи не найдены