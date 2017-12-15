##### Epsilon Notepad - mishapivo.github.io

## MARKDOWN | CSS | STYLE

### Markdown стили на сайт mishapivo.github.io

# THEME: MATERIAL

# COLOR PALETE:



H1
H2
H3
H4
H5
H6




```
code

html { background:white; color:black; word-wrap: break-word; margin:5px; line-height:150%; } code, pre, blockquote { background:#eee; color:black; -moz-tab-size: 1; -o-tab-size: 1; tab-size: 1; } h1,h2,h3,h4,h5,h6{ line-height:150%; } h1 { color:#268bd2; } h2,h3,h4,h5,h6 { color:#268bd2; } a { color:#268bd2; white-space: pre-wrap; white-space: -moz-pre-wrap; white-space: -pre-wrap; white-space: -o-pre-wrap; word-wrap: break-word; text-decoration:none; } :active, :focus { outline: none; -moz-outline-style: none; } pre { padding: 10px 10px 10px 10px; font-family: monospace; font-size: 95%; line-height: 140%; white-space: pre; white-space: pre-wrap; white-space: -moz-pre-wrap; white-space: -o-pre-wrap; border:1px solid #eee; border-radius:10px; box-shadow: 0 3px 6px rgba(0,0,0,0.16), 0 3px 6px rgba(0,0,0,0.23); } code { font-family: monospace; font-size: 95%; line-height: 140%; white-space: pre; white-space: pre-wrap; white-space: -moz-pre-wrap; white-space: -o-pre-wrap; } table{ width:100%; box-shadow: 0 3px 6px rgba(0,0,0,0.16), 0 3px 6px rgba(0,0,0,0.23); } table, th, td { border-collapse:collapse; padding:10px; border:1px solid #ccc; vertical-align: top; } tbody tr:nth-child(odd) { background:#eee; } noheader th {display:none;} blockquote { border-left: 10px solid #ccc; margin: 0px 0px 0px 10px; padding: 5px; box-shadow: 0 3px 6px rgba(0,0,0,0.16), 0 3px 6px rgba(0,0,0,0.23); } img { width: 80%; display: block; border: solid #ccc 1px; height: auto; margin-left: auto; margin-right: auto; box-shadow: 0 3px 6px rgba(0,0,0,0.16), 0 3px 6px rgba(0,0,0,0.23); } center p{text-align:center;} left p{text-align:left;} right p{text-align:right;} img[title=right]{width:40%; float:right; padding: 1px;margin: 10px;} img[title=left]{width:40%; float:left; padding: 1px;margin: 10px;} kbd { padding:0.1em 0.6em; border:1px solid #ccc; font-size:11px; font-family:Arial,Helvetica,sans-serif; background-color:#f7f7f7; color:#333; border-radius:3px; display:inline-block; margin:0 0.1em; white-space:nowrap; }

```



# Typora - лучший markdown редактор для Windows. Подробный обзор

![img](http://scriptify.ru/img/post-image/typora.png)

 15.04.2017  [markdown](http://scriptify.ru/blog/tags/markdown)

## Введение

Чем этот редактор отличается от других, что я решил посвятить ему целую статью? Для сравнения, у большинства markdown редакторов идет разделение на окно исходной разметки и окно предварительного просмотра.

![img](http://scriptify.ru/img/md/md-hp.png)

Мне непонятно, почему сложилась такая практика, которая повторяется в каждом редакторе. Минусы такого подхода:

- Уменьшается полезное пространство. Особенно это может быть заметным на маленьких мониторах
- Бесполезно дублируется контент. Зачем два окна, если можно работать в одном?
- Текст становится труднее для восприятия. Гораздо приятнее видеть текст, который будет наиболее близко к оригиналу

## Typora - Distraction Free редактор markdown

В Typora присутствует полноценный WYSIWYG режим. Преимущества тут очевидны:

1. Больше времени уделяешь содержанию, а не оформлению
2. Больше полезного пространства, особенно для маленьких мониторов
3. Лучшее визуальное восприятие текста

GIF

И это не единственное преимущество редактора. Здесь я хочу описать все возможности более подробно.

## Интерфейс редактора

Есть два варианта оформления программы. Они указываются в настройке *Windows Style*.

![img](http://scriptify.ru/img/typora/typora-6.png)

System Native - это более привычный и консервативный стиль:

![img](http://scriptify.ru/img/typora/typora-1.png)

Unibody - более современный и минималистичный:

GIF

Окно программы делится на левую панель и собственно область контента. Левая панель содержит две вкладки. *File* содержит информацию о файле. *Outline* показывает структуру файла, которая составляется из заголовков. Клик по заголовку позволяет быстро перейти к нужной части файла.

GIF

## Настройки программы

Настройки программы делятся на стандартные и расширенные. Стандартные указываются прямо в программе:

![img](http://scriptify.ru/img/typora/typora-4.png)

Расширенные хранятся в json файле `conf.user.json`. Получить файл можно, нажав на меню *Open Advanced Settings*

![img](http://scriptify.ru/img/typora/typora-5.png)

Рассмотрим наиболее полезные настройки:

**Custom Themes.** Открывает папку с CSS темами. Здесь можно отредактировать темы или создать свою.

**Save & Recover**. Автосохранение файлов. В `conf.user.json` указывается интервал автосохранения

JSON

```
"autoSaveTimer" : 1
```

**Auto Pair.** Автозавершение кавычек, скобок, markdown символов. Благодаря этой настройке удобно вставлять блоки кода.

GIF

**Developer.** Режим разработчика. Добавляет в контекстное меню функцию *Inspect Element*, благодаря ей можно просмотреть выбранный элемент в консоли разработчика

![img](http://scriptify.ru/img/typora/typora-3.png)

**Расширенные настройки.** Расширенных настроек не так много, все они интуитивно понятны

JSON

```
{
  "width" : null, // ширина программы в пикселях при загрузке
  "height" : null, // высота программы в пикселях при загрузке
  "directWrite": true, // поддержка DirectWrite API, необходима для лучшего отображения шрифтов
  "defaultFontFamily": { // семейство шрифтов по умолчанию
    "standard": null,
    "serif": null,
    "sansSerif": null,
    "monospace": null
  },
  "autoHideMenuBar": false, // автоматическое скрытие меню
  "searchService": [
    ["Search with Google", "https://google.com/search?q=%s"] // добавление поисковых систем в контекстное меню
  ],
  "keyBinding": { // переназначение горячих клавиш
        "Code Fences": "Ctrl+`",
        "Unordered List": "Ctrl+-",
        "Quote": "Ctrl+Q",
        "Paste As Plain Text": "Ctrl+Shift+Z",
  },
  "autoSaveTimer" : 1 // интервал автосохранения
}
```

## Возможности

### Автоматическое преобразование HTML в Markdown

Если текст был скопирован с сайта, в этом случае HTML разметка будет автоматически преобразована в Markdown. Можно вставлять текст и без форматирования, для этого есть функция *Edit - Paste As Plain Text*.

### Работа с изображениями

**Drag & Drop.** Изображения можно вставлять методом Drag & Drop или функцией *Edit - Image Tools - Insert Local Images*

GIF

**Использование относительной ссылки на изображение**. Изображения можно вставлять локально с компьютера. При этом можно указывать как абсолютную, так и относительную ссылку на файл. Для относительных ссылок нужно указать корневую папку: *Edit - Image Tools - Use Image Root Path*. Теперь изображения можно указывать в виде `![alt](/img/img.jpg)`. Это может быть очень удобным, если вы будете потом переносить статью на свой сайт.

GIF

### Вставка ссылок

Для вставки ссылки выделяем нужный текст и нажимаем `ctrl+K` *(Format - Hyperlink)*

GIF

### Вставка таблиц

По умолчанию вставка таблиц осуществляется комбинацией `ctrl+T`. В диалоговом окне указываем количество колонок и строк:

GIF

### Создание собственных тем оформления

Создавать собственные темы очень просто, если вы хорошо знакомы с CSS. Также можно быстро переключаться между темами.

GIF

### Экспорт в множество форматов

Список форматов, в который может конвертировать Typora из markdown, довольно впечатляющий: PDF, HTML, .docx, Epub и многое другое.

![img](http://scriptify.ru/img/typora/typora-10.png)

## Итог

В то время как другие разработчики умудряются просить денег за свои недоделки, Typora на данный момент остается хорошим бесплатным редактором. Но даже если и он станет платным, я не пожалею средств, чтобы поддержать автора. Рассмотрев десяток подобных программ, я по праву назову Typora лучшим Markdown редактором для Windows.

← Предыдущая статья

Макросы в Laravel

 

Следующая статья →

Обзор Markdown редакторов для Windows



tools - инструменты

markdown - 

soft - 

efectivity
