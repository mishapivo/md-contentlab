# Форматы записей WordPress

[Главная](https://www.wordpress-abc.ru/) » [Администрирование](https://www.wordpress-abc.ru/administrirovanie) » [Оформление статей](https://www.wordpress-abc.ru/administrirovanie/oformlenie-statej) » Форматы записей WordPress

![формат записи](https://www.wordpress-abc.ru/wp-content/uploads/2014/02/format-pages-wordpress-1.jpg)

Форматы записей WordPress это предоставленная разработчиками WordPress, возможность стилизовать заметки сайта под 10 форматов. Почему возможность? Потому-то, не во всякой теме активирована поддержка этой функции или активирована поддержка не всех, а одного или нескольких форматов. Давайте разберемся с этим вопросом.

Содержание

- [Где включить форматы записей WordPress](https://www.wordpress-abc.ru/administrirovanie/oformlenie-statej/formatyi-zapisey-wordpress.html#__WordPress)
- [Поддерживает ли ваша тема форматы записей WordPress](https://www.wordpress-abc.ru/administrirovanie/oformlenie-statej/formatyi-zapisey-wordpress.html#___WordPress)
- [Как проверить, какие форматы записей поддерживает ваша тема?](https://www.wordpress-abc.ru/administrirovanie/oformlenie-statej/formatyi-zapisey-wordpress.html#i)
- [Стили формата записи WordPress](https://www.wordpress-abc.ru/administrirovanie/oformlenie-statej/formatyi-zapisey-wordpress.html#__WordPress-2)

## Где включить форматы записей WordPress

Если вы войдете в [административную панель](https://www.wordpress-abc.ru/administrirovanie/konsol-sajta-wordpress.html) своего сайта, откроете страницу добавления/редактирования записи и в выезжающем модуле «Настройки» вверху страницы, отметите чекбокс «Форматы», то на странице редактора вы увидите модуль «Форматы», максимально с десятью форматами, на выбор.

[![Форматы записей WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Nastroyka_e%60krana_format-400x60.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Nastroyka_e%60krana_format.png)

[![Виды_формата_wordpress](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Vidyi_formata_wordpress.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/Vidyi_formata_wordpress.png)

## Поддерживает ли ваша тема форматы записей WordPress

Но наличие модуля «Форматы» в окне редактора WordPress, не означает, что вы сможете его использовать. Разработчики шаблонов могут не включить в функционал шаблона поддержку всех десяти возможных форма записей. Почему? Не знаю, принципиальных запретов нет.

## Как проверить, какие форматы записей поддерживает ваша тема?

Для проверки идем на вкладку Внешний вид→Редактор. Открываем файл темы: Функции темы (functions.php) и ищем строку:

 В отличие от приведенного кода, на фото вы можете видеть, что в  показанном файле темы поддерживаются  не все возможные форматы записей WordPress, отсутствует чат (chat), видео, аудио.

[![add_theme_support](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/add_theme_support-400x77.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/add_theme_support.png)

Его отсутствие отражается на модуле «Форматы» в окне редактора. В списке форматов нет форматов «Чат», «Видео»,»Аудио».

[![форматы_без_chat](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/formatyi_bez_chat.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/formatyi_bez_chat.png)

Если форматы не поддерживаются, то вы можете добавить вышеуказанный код в файл функции темы (functions.php) и тем самым активировать  форматы записей WordPress. Не обязательно добавлять все форматы, можно добавить (или удалить) отдельные форматы.

[Читайте так же:  Сайдбар и виджеты Wordpress](https://www.wordpress-abc.ru/uroki-wordpress/saydbar-vidzhetyi-wordpress.html)

Также из кода вы видите, как правильно  «обзываются» форматы записей WordPress:

- aside (Стандартная запись)
- gallery (Галерея)
- link (Ссылка)
- image (Фото)
- quote (Цитата)
- status (Статус)
- video (Видео)
- audio (Аудио)
- chat (Чат).

Отмечу, по-умолчанию, если не активирован или неисправен один из форматов записи, или выключен «Формат» в настройках, то  будет применен формат «Стандартная запись».

## Стили формата записи WordPress

Но это еще не все. Для каждой записи, в файле стилей CSS шаблона, должен быть определен стиль для каждого формата записи. Как будут прописаны стили для каждого формата записей, зависит от авторов шаблона. Вполне вероятно, что вообще стили не будут прописаны, и поэтому  ко всем форматам записей будет применен стиль стандартной записи.

[![Пример CSS форматов записи](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/CSS-formatov-zapisi-400x94.png)](https://www.wordpress-abc.ru/wp-content/uploads/2014/01/CSS-formatov-zapisi.png)

Прописать или [редактировать CSS](https://www.wordpress-abc.ru/cms-woprdpress/codex-wp/kak-redaktirovat-css-sayta-wordpress.html) стили для форматов записи вы можете самостоятельно, соблюдая синтаксис языка CSS, на котором написан файл таблица стилей (style.css).

Игорь Серов специально для сайта «[Как сделать сайт WordPress](https://www.wordpress-abc.ru/)»

### Другие статьи раздела: Администрирование WordPress

- Записи не найдены