# Отдельная страница для тэгов WordPress сайта: лист меток

[Главная](https://www.wordpress-abc.ru/) » [CMS Wordpress](https://www.wordpress-abc.ru/cms-woprdpress) » [Файлы Wordpress](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress) » Отдельная страница для тэгов WordPress сайта: лист меток

![страница для тэгов WordPress сайта](https://www.wordpress-abc.ru/wp-content/uploads/2016/09/stranitsa-dlya-te%60gov-WordPress-sayta.jpg)

Содержание

- [Вступление](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/otdelnaya-stranitsa-dlya-tegov-wordpress-sayta.html#i)
- [Страница для тэгов WordPress](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/otdelnaya-stranitsa-dlya-tegov-wordpress-sayta.html#__WordPress)
- Второй способ создать страницу меток
  - [Примечание](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/otdelnaya-stranitsa-dlya-tegov-wordpress-sayta.html#i-3)
- [Создаем страницу с облаком всех меток сайта](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/otdelnaya-stranitsa-dlya-tegov-wordpress-sayta.html#i-4)
- [Показываем страницу меток в меню сайта](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/otdelnaya-stranitsa-dlya-tegov-wordpress-sayta.html#i-5)

## Вступление

Недавно я понял, что не уделял тэгам (меткам) WordPress должного внимания. Вчера посмотрел в консоли страницу «Метки» и увидел, что их более 500 и это после удаления не прикрепленных меток. Пора делать для них отдельную страницу. Как всегда даю практическое решение. Для сохранения изменений в шаблоне используем [дочернюю тему](https://www.wordpress-abc.ru/temy-wordpress/zachem-nuzhna-dochernyaya-tema-wordpress.html).

Для безопасности, чтобы не потерять сайт, делаем резервную копию сайта. Как это сделать читаем [тут](https://www.wordpress-abc.ru/administrirovanie/kak-bezopasno-redaktirovat-fajly-wordpress.html).

## Страница для тэгов WordPress

В создании страницы идем практическим путем. Для шаблона страницы берем файл вашего шаблона, выводящий страницы (page) сайта. Копируем его и переносим для редактирования в текстовой редактор типа Notepad++.

-Ищем в файле функцию, которая выводит контент. Скорее всего это будет функция:

```
<?php the_content(); ?>
```

-Вместо неё вписываем стандартную функцию WP для вывода облака меток:

```
<?php wp_tag_cloud( $args ); ?> //, где $args это аргументы функции.
```

-Например, укажем такой аргумент:

```
<?php wp_tag_cloud('number=2000'); ?>
```

, где 2000 это количество меток.

-Сохраняем файл под именем [tag.php]. Если такой файл уже есть, даем ему другое имя;

-Заливаем этот файл в каталог рабочего шаблона.

-В шаблоне появится название нового файла, что мы и видим на странице «Редактор» в консоли сайта.

[Читайте так же:  Как убрать ссылку на author wordpress](https://www.wordpress-abc.ru/cms-woprdpress/kak-ubrat-ssyilku-na-author-wordpress.html)

## Второй способ создать страницу меток

Если [шаблон сайта](https://www.wordpress-abc.ru/administrirovanie/tema-wordpress.html) сложный, то могут возникнуть сложности с использованием шаблонного файла для страницы. В этом случае идем вторым путем.

- В текстовом редакторе создаем такой файл:

*В начале файла задаем его название: The template name: Tag. Получаем в консоли название «Шаблон метки». Если ничего не писать, получим просто файл: tag.php.*

- Сохраняем под именем [tag.php]
- Заливаем созданный файл в каталог шаблона.

### Примечание

В файле, который я привел для примера функция [wp_tag_cloud] указана с атрибутами:

- smallest=12&largest=36 (минимальный и максимальный разметы шрифтов меток);
- number=1500 (количество выводимых меток);
- format=flat (включает, параметр separator;)
- separator=| (разделитель)
- orderby=name (сортировка по имени, можно не указывать).

## Создаем страницу с облаком всех меток сайта

Страница для тэгов WordPress создана. После создания файла страницы для вывода облака меток, остается эту страницу создать.

- Идем на вкладку: Создать страницу;
- В спойлере страницы «Настройка» (вверху), включаем «Атрибуты страницы»;
- Пишем вступление, например: Это общее облако меток сайта;
- В «Атрибутах страницы» указываем шаблон, созданный нами ранее «Tag»;
- Не забываем дать странице название и опубликовать;
- Далее идем на Внешний вид→Меню и добавляем пункт меню с созданной страницей. Сохраняемся;
- Смотрим результат.

[![sozdat-stranitsu-metok-1](https://www.wordpress-abc.ru/wp-content/uploads/2016/09/sozdat-stranitsu-metok-1-448x241.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/09/sozdat-stranitsu-metok-1.jpg)Создаем страницу меток

## Показываем страницу меток в меню сайта

- Идем на вкладку Меню;
- Выбираем нужно меню для редактирования;
- Добавляем в это меню созданную страницу вывода меток;
- Назовем её «Лист меток»;
- Сохраняем изменения в меню и смотрим результат. Страница для тэгов WordPress создана.

[![menyu-lista-metok-1](https://www.wordpress-abc.ru/wp-content/uploads/2016/09/menyu-lista-metok-1-448x241.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/09/menyu-lista-metok-1.jpg)Показываем лист меток в меню

[![list-metok-1](https://www.wordpress-abc.ru/wp-content/uploads/2016/09/list-metok-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/09/list-metok-1.jpg)страница для тэгов WordPress

### Статьи по теме

- [Похожие записи WordPress без плагина](https://www.wordpress-abc.ru/plaginy/wordpress-bez-plugins/plagin-i-kod-dlya-poxozhie-zapisi-wordpress.html)
- [Как разделить анонс и цитату  в шаблоне WordPress](https://www.wordpress-abc.ru/seo-wordpress/kak-razdelit-anons-i-tsitatu-v-shablone-wordpress.html)
- [Проблема дублирования WordPress: уникальный блог последних записей](https://www.wordpress-abc.ru/seo-wordpress/problema-dublirovaniya-wordpress.html)
- [Как редактировать CSS сайта WordPress](https://www.wordpress-abc.ru/cms-woprdpress/codex-wp/kak-redaktirovat-css-sayta-wordpress.html)
- [Связанные материалы без плагина](https://www.wordpress-abc.ru/plaginy/wordpress-bez-plugins/svyazannyie-materialyi-bez-plagina.html)
- [Как сделать кнопку плавного прокручивания «Наверх»](https://www.wordpress-abc.ru/plaginy/wordpress-bez-plugins/kak-sdelat-knopku-plavnogo-prokruchivaniya-naverx.html)
- [Кнопка наверх в виде картинки](https://www.wordpress-abc.ru/plaginy/wordpress-bez-plugins/knopka-naverx-v-vide-kartinki.html)
- [6 Проверенных размещения рекламы в WordPress без плагина](https://www.wordpress-abc.ru/plaginy/wordpress-bez-plugins/6-proverennyx-razmeshheniya-reklamy-v-wordpress-bez-plagina.html)
- [Как вывести список статей нужной категории в любом месте шаблона WordPress](https://www.wordpress-abc.ru/plaginy/wordpress-bez-plugins/kak-vyvesti-spisok-statej-nuzhnoj-kategorii-v-lyubom-meste-shablona-wordpress.html)
- [Перенос комментариев между постами без плагина](https://www.wordpress-abc.ru/plaginy/wordpress-bez-plugins/perenos-kommentariev-mezhdu-postami-bez-plagina.html)