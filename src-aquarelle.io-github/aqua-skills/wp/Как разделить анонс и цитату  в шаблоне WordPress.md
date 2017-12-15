# Как разделить анонс и цитату  в шаблоне WordPress

[Главная](https://www.wordpress-abc.ru/) » [SEO оптимизация Wordpress](https://www.wordpress-abc.ru/seo-wordpress) » Как разделить анонс и цитату  в шаблоне WordPress

![разделить анонс и цитату](https://www.wordpress-abc.ru/wp-content/uploads/2016/06/razdelit-tsitatu-anons-wordpress.jpg)

Содержание

- [Введение](https://www.wordpress-abc.ru/seo-wordpress/kak-razdelit-anons-i-tsitatu-v-shablone-wordpress.html#i)
- [Основные понятия](https://www.wordpress-abc.ru/seo-wordpress/kak-razdelit-anons-i-tsitatu-v-shablone-wordpress.html#i-2)
- Как разделить анонс и цитату
  - [Важно понять идею!](https://www.wordpress-abc.ru/seo-wordpress/kak-razdelit-anons-i-tsitatu-v-shablone-wordpress.html#i-4)
- [Как убрать цитату и анонс из текста статьи](https://www.wordpress-abc.ru/seo-wordpress/kak-razdelit-anons-i-tsitatu-v-shablone-wordpress.html#i-5)

## Введение

В этой статье мы разделяем анонс и цитату в шаблоне WordPress, для того, чтобы в блоге последних записей выводить анонс статьи (текст до тега more), а в архивах сайта выводить заранее заданную цитату. При этом сделаем так, чтобы анонс не попадал в саму статью. Тем самым мы создадим три различных уникальных содержания: анонс, цитата, статья.

## Основные понятия

**Анонс** – вступление к статье, от статьи отделяется тегом [more]. По умолчанию анонс виден на главной странице, страницах архивов и в самой статье.

**Цитата** — дополнительное поле, необязательное к заполнению. В зависимости от верстки шаблона может выводиться в архивах сайта.

Проблему дублирования анонсов я недавно поднимал в статье: Проблема дублирования WordPress.

**Итак, анонс и цитата.** Идея этой статьи, разделить анонс и цитату и четко сделать так, чтобы:

- Анонс показывался в блоке последние записи (главная страница сайта),
- Цитата выводилась в архивах сайта (архив разделов, тегов, автора).

> Тема статьи связана с редакцией кода шаблона, поэтому перед работой нужно [сделать полную резервную копию сайта](https://www.wordpress-abc.ru/administrirovanie/kak-bezopasno-redaktirovat-fajly-wordpress.html).

Часто, при заполнении цитаты, которая не обязательна, но предусмотрена в WordPress, на главной странице выводится вместо анонса цитата. Такая верстка шаблона ломает основную идею статьи: использования цитаты, как вступление в архивах сайта, а анонса, как вступление в блоге главной страницы. Дополнительная идея: исключить из текста статьи анонс и цитату.

[Читайте так же:  Wordpress плагин Exploit Scanner безжалостный борец с вирусами](https://www.wordpress-abc.ru/plaginy/wordpress-plagin-exploit-scanner-bezzhalostnyiy-borets-s-virusami.html)

## Как разделить анонс и цитату

Цитату из статьи убирать не нужно. Я не встречал, чтобы так верстали шаблон. Другое дело, анонс статьи. Под анонсом понимаем часть статьи отделенного от основной статьи тегом [more]. Синтаксис тега:

```
<!--more-->
```

Итак, установив тег [more] вы отделяете анонс статьи. При этом, по умолчанию, анонс будет виден в блоге последних записей и одновременно будет показан в основной части статьи.

Идея этой статьи, разделить анонс, цитату и основное содержание. Тем самым, повысить уникальность сайта. При это не нужно будет закрывать в файле [robots.txt](https://www.wordpress-abc.ru/veb-instrumenty/fajl-robots-txt-dlya-wordpress.html)от поисковиков архивы сайта и получим уникальный блок анонсов последних записей. Если учесть, что этот блог делают  главной страницы сайта, получаем уникальную главную страницу сайта. Для решения задачи, нам нужно последовательно посмотреть два файла:

1. Файл Архивы (archive.php): выводит архивы сайта;
2. Файл  шаблона рубрик (category.php) – его может и не быть. Если этого файла в шаблоне нет, архив категорий выводит файл archive.php;

В archive.php, ищем функцию [get_template_part]. Эта функция «берет» часть шаблона с другого файла и применяет в архивах. Покажу на примере:

get_template_part( ‘content’, get_post_format() );

Читаем: это значит, что в архиве будет выводится часть текста определенного в файле под названием [content].

[![файл-архивы-wordpress-1](https://www.wordpress-abc.ru/wp-content/uploads/2016/06/fayl-arhivyi-wordpress-1-596x350.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/06/fayl-arhivyi-wordpress-1.jpg)

- Открываем файл [content] для дальнейшего редактирования.


- Для безопасности копируем файл [content] и открываем его в текстовом редакторе (например, Notepad++).
- В файле [content]  нам нужно найти функции [the_excerpt()] и [the_content()]. Они или она, будут после блока [head].

[![разделить-анонс-и-цитату-3](https://www.wordpress-abc.ru/wp-content/uploads/2016/06/razdelit-anons-i-tsitatu-3-593x350.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/06/razdelit-anons-i-tsitatu-3.jpg)

### Важно понять идею!

Мы не будем исправлять файлы шаблона (код шаблона). Мы дополним шаблон новым файлом. Это простой способ, не требует особых знаний php и не тянет за собой целую цепочку исправлений.

Для этого:

- Копию файла [content], открываем в Notepad++ и переименовываем, в файл, например [content-abc];
- Функцию [the_content()] меняем на [the_excerpt()];
- Сохраняем новый файл [content-abc] в формате [php];
- Заливаем файл [content-abc] по FTP в каталог сайта, в папку themes/ваша_тема.

[![разделить-анонс-и-цитату-2](https://www.wordpress-abc.ru/wp-content/uploads/2016/06/razdelit-anons-i-tsitatu-2-593x350.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/06/razdelit-anons-i-tsitatu-2.jpg)

- Идем в редактор административной части сайта Внешний вид→Редактор, и видим появление этого файла;
- Открываем файл archive.php. В той самой функции [get_template_part], которую мы нашли ранее, меняем название, в моем примере, [content] на [content-abc];

[![разделить-анонс-и-цитату-1](https://www.wordpress-abc.ru/wp-content/uploads/2016/06/razdelit-anons-i-tsitatu-1-598x350.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/06/razdelit-anons-i-tsitatu-1.jpg)

*Нам удалось разделить анонс и цитату  в шаблоне WordPress. Теперь в архивах вместо анонса будут выводиться цитаты.*

[![разделить анонс и цитату](https://www.wordpress-abc.ru/wp-content/uploads/2016/06/glavnaya-wordpress.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/06/glavnaya-wordpress.jpg)

[![архивы-wordpress](https://www.wordpress-abc.ru/wp-content/uploads/2016/06/arhivyi-wordpress.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/06/arhivyi-wordpress.jpg)

[Читайте так же:  Чужой код в теме WordPress](https://www.wordpress-abc.ru/bezopasnost-wp/chuzhoy-kod-v-teme-wordpress.html)

Важно! Шаблон может быть сверстан в сложном варианте. Автор шаблона мог разделить вывод:  архивов, категорий, тегов и т.д.  Поэтому блок категорий может выводить не файл archive.php, а файл category.php. Для примера я взял шаблон nirvana. В нем вместо стандартного набора из 18 файлов, автор создал, аж 40 файлов php.

## Как убрать цитату и анонс из текста статьи

Осталось последнее замечание. Если хотите чтобы анонс статьи не попадал в саму статью, то отделяйте анонс не тегом [more], а двойным тегом [more][noteaser]. Об этом читайте отдельную статью: тут.

[©wordpress-abc.ru](https://www.wordpress-abc.ru/)

### Другие статьи раздела: SEO оптимизация WordPress

- [Оптимизация изображений WordPress](https://www.wordpress-abc.ru/seo-wordpress/optimizatsiya-izobrazheniy-wordpress.html)
- [Как убирать ссылки автора темы WordPress  ](https://www.wordpress-abc.ru/seo-wordpress/kak-ubirat-ssyilki-avtora-temy-wordpress.html)
- [2 отличных и 1 известный сервисы проверки уникальности текстов](https://www.wordpress-abc.ru/seo-wordpress/servisyi-proverki-unikalnosti-tekstov.html)
- [Разница между рубриками и метками WordPress](https://www.wordpress-abc.ru/seo-wordpress/raznitsa-mezhdu-rubrikami-metkami-wordpress.html)
- [Проблема дублирования WordPress: уникальный блог последних записей](https://www.wordpress-abc.ru/seo-wordpress/problema-dublirovaniya-wordpress.html)
- [Битые ссылки на WordPress сайте](https://www.wordpress-abc.ru/seo-wordpress/bityie-ssyilki-na-wordpress-sayte.html)