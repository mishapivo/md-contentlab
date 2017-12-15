# Как редактировать CSS сайта WordPress

[Главная](https://www.wordpress-abc.ru/) » [CMS Wordpress](https://www.wordpress-abc.ru/cms-woprdpress) » [Кодекс WP](https://www.wordpress-abc.ru/cms-woprdpress/codex-wp) » Как редактировать CSS сайта WordPress

![редактировать CSS сайта WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress.jpg)

Содержание

- [Вступление](https://www.wordpress-abc.ru/cms-woprdpress/codex-wp/kak-redaktirovat-css-sayta-wordpress.html#i)
- [CSS это](https://www.wordpress-abc.ru/cms-woprdpress/codex-wp/kak-redaktirovat-css-sayta-wordpress.html#CSS)
- [Где лежит файл style.css WordPress](https://www.wordpress-abc.ru/cms-woprdpress/codex-wp/kak-redaktirovat-css-sayta-wordpress.html#__stylecss_WordPress)
- Три способа редактировать CSS сайта WordPress
  - [Редактирование из панели администратора](https://www.wordpress-abc.ru/cms-woprdpress/codex-wp/kak-redaktirovat-css-sayta-wordpress.html#i-2)
  - [Редактирование файла style.css по FTP](https://www.wordpress-abc.ru/cms-woprdpress/codex-wp/kak-redaktirovat-css-sayta-wordpress.html#_stylecss_FTP)
  - [Дочерняя тема WordPress](https://www.wordpress-abc.ru/cms-woprdpress/codex-wp/kak-redaktirovat-css-sayta-wordpress.html#_WordPress)
  - [Редактирование файла style.css WordPress с помощью плагинов](https://www.wordpress-abc.ru/cms-woprdpress/codex-wp/kak-redaktirovat-css-sayta-wordpress.html#_stylecss_WordPress)
- Как понять, что нужно редактировать
  - [Полезные ссылки](https://www.wordpress-abc.ru/cms-woprdpress/codex-wp/kak-redaktirovat-css-sayta-wordpress.html#i-4)

## Вступление

Изменить оформление сайта, можно в файлах активной темы WordPress, а именно в файле под названием style.css. Это простой текстовой файл в расширении CSS. Переводится CSS как Cascading Style Sheets — каскадные таблицы стилей. Согласен, перевод мало о чем говорит. Какими способами можно редактировать [CSS сайта WordPress](https://www.wordpress-abc.ru/cms-woprdpress/fajly-wordpress/pravila-verstki-css-wordpress-kaskadnyie-stili-css-na-wordpress.html) пойдет речь далее.

## CSS это

С одной стороны CSS это расширение текстового файла. С другой стороны CSS это язык программирования, на котором пишется это файл. С третьей стороны CSS это свод правил для задания шрифта, цвета сайта, относительного расположения блоков сайта (влево, центр, право, отступы от верха и низа) и других представлений внешнего вида страниц сайта, которые в этом файле и прописаны.

Сразу замечу, файлы CSS могут иметь пугающие размеры, но в них нет ничего сложного. Это очень простые, хотя и разнообразные, правила, написанные в простом синтаксисе.

Я не собираюсь обучать основам CSS, это отлично делают на специальных сайтах. Нам понадобиться только справочник HTML: *http://htmlbook.ru/*.

Также замечу, что запоминать все правила CSS наизусть совершенно не обязательно. Достаточно понимать синтаксис написания правил CSS. Этого достаточно, чтобы редактировать файл CSS, да и справочник всегда поможет. Главное знать, что править и как править. Кроме справочника есть инструменты в браузерах, о них чуть ниже, которые позволяют редактировать CSS онлайн.

## Где лежит файл style.css WordPress

Несколько прописных истин:

- Каждая тема WordPress имеет свой файл определяющий ее внешний вид.
- Редактирования файла style.css одной темы не затрагивает другие темы установленные на сайт;
- Перед редактированием любых файлов активной темы, сделайте резервную копию сайта, на случай фатальных ошибок редактирования и возвращения сайту рабочего состояния.

А лежит файл style.css WordPress в папке с темой (шаблоном) WP. Полный адрес, одинаков для всех тем: *wp-content/themes/название_темы/style.css*.

## Три способа редактировать CSS сайта WordPress

Предложу три варианта редактирования файла style.css.

### Редактирование из панели администратора

Вам, наверное, известно, что система WordPress имеет внутренний редактор файлов установленных тем. Войти в него можно из консоли сайта через вкладку: Внешний вид→Редактор.

[![редактировать-CSS-сайта-WordPress-1](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-1.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-1.jpg)

[![редактировать-CSS-сайта-WordPress-01](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-01.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-01.jpg)

[Читайте так же:  Как скрыть статьи отдельных категорий с главной страницы Wordpress](https://www.wordpress-abc.ru/cms-woprdpress/codex-wp/kak-skryt-stati-otdelnyx-kategorij-s-glavnoj-stranicy-wp.html)

Справа вы видите список файлов темы, в поле редактора открывается содержимое файлов. Если у вас установлено несколько тем, обратите внимание на правый верхний угол. Там есть поле выбора темы. По умолчанию откроется активная тема, но редактировать можно любую установленную тему без её активации.

Совет:

Ошибки в редактировании style.css не могут обрушить сайт, вы можете изуродовать только внешний вид. Поэтому, перед прямым редактированием из консоли можно обойтись и без резервной копии сайта, достаточно сделать копию самого файла style.css и в случае неудачного редактирования вернуть файлу прежний вид.

### Редактирование файла style.css по FTP

Говорят, что есть хостинги, которые не поддерживают редактирование файлов темы из административной панели сайта. Не беда. Можно и на самом деле это правильно, редактировать файл style.css по FTP. Правильно, потому что безопасно и у вас всегда есть оригинальная копия файла.

- Входите в каталог сайта по FTP;
- Добираетесь до wp-content/themes/название_темы/style.css и копируете его на компьютер;
- Далее редактируете его в текстовом редакторе типа Notepad++, сохраняете, оставляя оригинальную копию, и заливаете обратно в каталог. Согласен, немного дольше, но безопаснее и удобнее. Можно спокойно почитать файл и не спеша разобраться с его синтаксисом.

Оба способа редактирования относятся к прямому редактированию, «живого» файла активной темы. У прямого редактирования есть большой недостаток: при обновлении темы все ваши изменения потеряются и тема примет исходный внешний вид. Чтобы этого избежать используется способ дочерней темы.

[Читайте так же:  Браузер Lynx — установка и работа с Lynx Browser](https://www.wordpress-abc.ru/browsers/brauzer-lynx-ustanovka-i-rabota.html)

### Дочерняя тема WordPress

Система WordPress позволяет создавать дочерние темы, для родительской активной темы. Дочерняя тема может полностью быть копией родительской темы или с помощью функции import, «забирать» и переопределять стиль родительской темы. То есть, после создания и активации темы наследницы редактируется файл style.css дочерней темы и изменения не пропадают после обновления шаблона. О дочерней теме я писал подробную статью: [Зачем нужна дочерняя тема WordPress](https://www.wordpress-abc.ru/temy-wordpress/zachem-nuzhna-dochernyaya-tema-wordpress.html).

На этом принципе основан и третий способ редактирования стилей.

### Редактирование файла style.css WordPress с помощью плагинов

Есть несколько плагинов для улучшения редактора файлов темы. Для редактирования стилей мне нравится плагин Jetpack. О плагине я писал подробную статью: [Плагин Jetpack заменит 33 плагина WordPress](https://www.wordpress-abc.ru/plaginy/plagin-jetpack-zamenit-33-plagina-wordpress.html). Плагин очень большой и для редактирования стилей темы нужно активировать модуль Custom CSS.

[![редактировать-CSS-сайта-WordPress-2](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-2.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-2.jpg)

После его активации в меню консоли в пункте Внешний вид появляется вкладка «Редактировать CSS».

[![редактировать-CSS-сайта-WordPress-3](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-3.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-3.jpg)

[![редактировать-CSS-сайта-WordPress-4](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-41.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-41.jpg)редактировать CSS сайта WordPress

Теперь не нужно редактировать style.css напрямую, достаточно вписать кусок кода css в поле редактора и изменения появятся на сайте. Причем при обновлении темы они не потеряются.

## Как понять, что нужно редактировать

> Если вы бегло не читаете CSS нужно воспользоваться онлайн инструментами, для чтения CSS и понять, что нужно редактировать.

Самый простой инструмент, это инструмент в любом браузере: «Просмотр кода элемента» в Chrom. В других браузерах название похожее.

Доступ к инструменту через правую кнопку мыши или короткими клавишами.

**Показываю, как им пользоваться:**

Например, хотим поменять заголовок сайта.

- Наводим на него мышь, через правую кнопку открываем «Код элемента»;

[![редактировать-CSS-сайта-WordPress-5](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-5.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-5.jpg)редактировать CSS сайта WordPress начало

- Видим код HTML в правом поле и код CSS в левом поле;


- Можно «наживую» поиграть с кодом CSS и сразу посмотреть, как это выглядит;
- Чтобы открыть CSS в основном поле, жмем на название файла CSS (на фото цифра 2).

![редактировать-CSS-сайта-WordPress-6](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-6.jpg)редактировать CSS сайта WordPress

Для примера, я поменял онлайн размер шрифта названия.

[![редактировать-CSS-сайта-WordPress-7](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-7.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-7.jpg)

[Читайте так же:  Хостинг и сайт WordPress: выбор хостинга для сайта](https://www.wordpress-abc.ru/hosting/hosting-i-sayt-wordpress.html)

[![редактировать-CSS-сайта-WordPress-8](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-8.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/10/redaktirovat-CSS-sayta-WordPress-8.jpg)

Но это еще не все.

- Нашли нужный кусок кода css;
- Копируем его;
- Переносим в текстовой редактор;
- Редактируем и переносим кусок кода в style.css дочерней темы или в поле редактора Jetpack.
- Таким образом, меняем любые стили активной темы.

### Полезные ссылки

- Сервис проверки CSS от W3C (формат CSS3): http://jigsaw.w3.org/css-validator/

©www.wordpress-abc.ru

### Другие статьи раздела: CMS WordPress

- Записи не найдены