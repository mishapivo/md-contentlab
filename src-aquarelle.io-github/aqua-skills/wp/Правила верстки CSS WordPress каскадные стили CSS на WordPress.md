# Правила верстки CSS WordPress: каскадные стили CSS на WordPress

[Главная](https://www.wordpress-abc.ru/) » [CMS Wordpress](https://www.wordpress-abc.ru/cms-woprdpress) » [Файлы Wordpress](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress) » Правила верстки CSS WordPress: каскадные стили CSS на WordPress

![правила верстки CSS WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2016/12/cssjockey-css.png)

Содержание

- [Вступление](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/pravila-verstki-css-wordpress-kaskadnyie-stili-css-na-wordpress.html#i)
- [Зачем нужно соблюдать правила верстки CSS WordPress](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/pravila-verstki-css-wordpress-kaskadnyie-stili-css-na-wordpress.html#___CSS_WordPress)
- [Структура CSS WordPress](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/pravila-verstki-css-wordpress-kaskadnyie-stili-css-na-wordpress.html#_CSS_WordPress)
- [Синтаксис структуры css wordpress](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/pravila-verstki-css-wordpress-kaskadnyie-stili-css-na-wordpress.html#_css_wordpress)
- Правила верстки CSS WordPress: CSS Селекторы
  - [Синтаксис для селекторов css wordpress](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/pravila-verstki-css-wordpress-kaskadnyie-stili-css-na-wordpress.html#__css_wordpress)
  - [Синтаксис для свойств css wordpress](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/pravila-verstki-css-wordpress-kaskadnyie-stili-css-na-wordpress.html#_css_wordpress-2)
  - [Указание цвета в css wordpress](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/pravila-verstki-css-wordpress-kaskadnyie-stili-css-na-wordpress.html#__css_wordpress-2)
- Синтаксис для значений css wordpress
  - [Выводы](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/pravila-verstki-css-wordpress-kaskadnyie-stili-css-na-wordpress.html#i-2)
  - [Полезные ссылки](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/pravila-verstki-css-wordpress-kaskadnyie-stili-css-na-wordpress.html#i-3)

## Вступление

Для создания и изменения внешнего вида сайта WordPress служит специальный файл шаблона, обычно называемый [style.css](https://www.wordpress-abc.ru/temy-wordpress/struktura-temyi-wordpress.html). В этом файле (их может быть несколько) автор шаблона задает каскадные стили CSS этого шаблона. Для CMS WordPress нет каких-то своих особых стилей CSS. Однако, есть несколько «корпоративных» правил, которые нужны для единообразия CSS файлов в раках сотрудничества разработчиков и распространения продуктов WordPress.

## Зачем нужно соблюдать правила верстки CSS WordPress

> Правила верстки CSS WordPress не выходят за рамки стандартного CSS кодирования, но имеют свои особенности для придания единых видов для всех сайтов, созданных на WordPress.

Если вы разработчик или стремитесь создать свою тему WordPress нужно «подчиниться» единым правилам WordPress сообщества и создавать свои CSS стили, придерживаясь этих правил.

Если вы пользователь и хотите несколько корректировать внешний вид сайта, то соблюдение этих правил необязательно, но крайне желательно, для их корректного применения.

> Правила перечисленные в этой статье простые и касаются правильного синтаксиса при составлении файла каскадных стилей.

## Структура CSS WordPress

Само понятие каскадный стиль предполагает последовательное применение указанных правил. Отсюда, в структурировании таблицы стилей важно сохранить высокую степень разборчивости документа и четкое представление о последовательности применения стилей.

Напомню на фото, что такое селектор, свойство и значение.

[![img](https://www.wordpress-abc.ru/wp-content/uploads/2016/12/selektor-svoystva-znacheniya.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/12/selektor-svoystva-znacheniya.jpg)

## Синтаксис структуры css wordpress

- Выравнивать свойства нужно кнопкой [Tab], кнопку «пробел» не трогаем;
- Между секциями нужно вставлять 2 пустые строчки. После блока нужно вставить 1 пустую строчку;
- Любое название селектора писать на отдельной строчке. Эту строчку заканчивать запятой, лучше фигурной скобкой «открыто»;
- Свойство вместе со значением размещать на новых строчках и заканчивать точка-запятая;
- Фигурная скобка, закрывающая значение, должна располагаться слева на одном вертикальном уровне с отступом селектора открытия.

[Читайте так же:  Отдельная страница для тэгов WordPress сайта: лист меток](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/otdelnaya-stranitsa-dlya-tegov-wordpress-sayta.html)

Правила совсем простенькие, но требуют демонстрации.

[![img](https://www.wordpress-abc.ru/wp-content/uploads/2016/12/selektor.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/12/selektor.jpg)

## Правила верстки CSS WordPress: CSS Селекторы

*Селектор css это описание элемента (можно группы элементов), к которым применяется данное правило стиля.*

Не корректное расположение селектора приводит к игнорированию стилей и влияет на скорость загрузки таблицы стилей.

### Синтаксис для селекторов css wordpress

[![img](https://www.wordpress-abc.ru/wp-content/uploads/2016/12/selektor1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/12/selektor1.jpg)

- Имена селекторов должны быть строчные;
- Для селекторов применять читаемые названия, описывающие элементы к которым применяются.

### Синтаксис для свойств css wordpress

[![img](https://www.wordpress-abc.ru/wp-content/uploads/2016/12/svoystva.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/12/svoystva.jpg)

- За свойством должны следовать двоеточие с пробелом;
- Все свойства и значения писать в нижнем регистре. Исключения составляют имена шрифтов и уникальные свойства;

### Указание цвета в css wordpress

- Для указания цвета используйте шестнадцатеричный код.
- Стандарт RGBA (), применяется только для указания непрозрачности. В других случаях RGB-формат не применять.
- Не использовать для цвета заглавных букв.
- Также сокращайте значение цвета, когда это возможно: например, вместо #DDDDDD указывайте #ddd.

Для указания цвета фона использовать не цифры, а стенографические значения. (Для справки *https://codex.wordpress.org/CSS_Shorthand*.). Кроме толщины шрифта.

**Например:** вместо цифрового размера шрифта указываем (medium, small, large и т.д.), вместо цифр цвета указываем: red, blue и т.д. (только для фона).

## Синтаксис для значений css wordpress

[![img](https://www.wordpress-abc.ru/wp-content/uploads/2016/12/znacheniya.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2016/12/znacheniya.jpg)

CMS WordPress рекомендованы следующие выводы значений для свойств.

- Перед значением двоеточие, далее пробел, потом значение;
- Всегда значение заканчивать точкой с запятой без пробела;
- Несколько значений заключаем в простые скобки;
- Для свойств значений применяются не двойные, а одинарные кавычки. Двойные кавычки применять, как исключение, например, когда указываете двойные названия шрифтов;
- Толщину шрифтов, по возможности, указывать только числовыми значениями. Например, указывать 400, а не normal, или 700, а не bold;
- Не указывать единиц для нулевых значений. Не нужно писать: 0px. Достаточно указать значение 0.
- Для стандарта RGBA, значения, разделяются запятыми и пробелами  или переводом строки.
- Высота линии line-height лучше указывать в кратных числах, а не в пикселях.

[Читайте так же:  Как ускорить загрузку JS скриптов, CSS и HTML сайта WordPress: плагин Autoptimize](https://www.wordpress-abc.ru/plaginy/kak-uskorit-zagruzku-js-skriptov-css-i-html-sayta-wordpress-plagin-autoptimize.html)

### Выводы

Несоблюдение вышеизложенные правила верстки CSS WordPress не приведет к пропаданию сайта, но может влиять на скорость обработки файла и некорректно отображать задуманный внешний вид страниц сайта.

### Полезные ссылки

- Сервис проверки CSS от W3C (формат CSS3): http://jigsaw.w3.org/css-validator/

©Wordpress-abc.ru

### Другие статьи по теме

- Записи не найдены