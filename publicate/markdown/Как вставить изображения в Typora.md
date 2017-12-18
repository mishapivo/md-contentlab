![img](https://material.io/icons/static/images/icons-share.png)



## Как вставить изображения в Typora

### Вставка в Markdown

Вы можете просто записать синтаксис разметки, чтобы вставить изображение. Или нажмите «изображение» из меню или нажмите комбинацию клавиш. Когда вы это сделаете, и между тем, если в буфере обмена есть URL-адрес изображения, то URL-адрес будет непосредственно вставлен в `src`.

### Перетаскивания - Drag & Drop

Конечно, есть более простой способ - перетащить и сбросить, как и скринкаст ниже.

![drag-img](img/drag-img.gif)



![img](https://material.io/icons/static/images/icons-share.png)



Вы также можете одновременно перетаскивать несколько файлов изображений.

### Выбрать из локальных файлов

Вы можете щелкнуть пункт меню `Edit` → `Image Tools` → `Insert Local Images…` в строке меню, чтобы открыть диалоговое окно для выбора и вставки локального изображения.

Если вы часто используете этот пункт меню, мы предложим вам повторно назначить комбинацию клавиш для этой команды "insert image", следуя [Custom Key Binding](http://support.typora.io/Custom-Key-Binding/).

### Вставить изображения из буфера обмена

Поскольку файл Markdown является только текстовым файлом, пользователи не могут вставлять данные изображения в файл Markdown напрямую, но могут вставлять ссылку на изображение в file/url.

Typora поддерживает вставку данных изображения из буфера обмена **, после того, как расскажет typora, куда поместить эти изображения **. Typora помещает данные изображения в заданную папку или сервер, а затем вставляет изображения, относящиеся к этому сохраненному файлу или URL-адресу. См. Раздел **[При вставке локального изображения ...](# когда-вставить-локальный-образ ...)** для более подробной информации.

> ** Советы **: на macOS пользователи могут копировать файл изображения из finder, а затем вставлять в typora. Он имеет такое же поведение при перетаскивании.
>
> ** Советы **: на macOS вы также можете копировать изображения с iPhone, а затем вставлять в Typora после настройки местоположения для размещения файлов изображений.

## При вставке локального изображения ...

Typora поддерживает копирование файлов изображений в данную папку или веб-сервер (требуется [iPic][]) при вставке локальных изображений с помощью перетаскивания или из строки меню. Ниже приведены инструкции по настройке.

### Поведение по умолчанию

По умолчанию, когда вы вставляете или перетаскиваете файл изображения в Typora, мы будем использовать путь к файлу изображения для атрибута `src`.

### Использовать относительный путь

Если вы включите `Editor` → `Image Insert` →  `Use relative path if possible` в панели настроек, и ваша запись была сохранена в файл, тогда при перетаскивании локального изображения атрибут `src` будет установить как относительный путь к текущему файлу (папке).

### Скопировать файлы изображений в целевую папку при вставке локального изображения

> Чтобы использовать эту функцию, вам нужно выбрать опцию «Разрешить копирование изображений в указанную папку» на панели настроек.

Одним из распространенных сценариев является редактирование сообщений `*.md` в статических сайтах (например, Jekyll) с использованием Typora. Например, если файл `. * Md` помещается в папку `_posts`, в то время как файлы изображений попадают в папку  `_media`, вы можете скопировать файлы изображений в папку `_media`, когда вы перетаскиваете или вставляете изображения в Файл Markdown автоматически. Вот как:

1. Сохраните файл на каком-то пути.

2. Включите «Редактор» → «Вставка изображения» → «Разрешить копирование изображений в указанную папку» на панели настроек.

   ! [Snip20161117_2] (IMG / Snip20161117_2.png)

3. Выберите «Редактировать» → «Инструменты изображения» → «При вставке локальных изображений» → «Копировать файл изображения в папку» из меню выберите целевую папку.

   ! [Snip20161117_6] (IMG / Snip20161117_6.png)

На шаге 3 новый элемент `typora-copy-images-to: {relative path}` будет вставлен в блок [YAML Front Matter] [] текущего документа. Таким образом, вы можете вручную добавить ** свойство typora-copy-images-to ** в YAML Front Matter, чтобы включить это поведение.

После этого, если вы перетащите ** локальные ** изображения или вставьте изображения в Typora, файл изображения будет скопирован в целевой файл и обновлен соответствующий `src`.

> To use this feature, you need to opt-in the option `Allow copy images to given folder` in preferences panel.

One common scenario is to edit `*.md` posts in static sites (like Jekyll) using Typora. For example, if the `.*md` file is put under `_posts` folder while the image files goes into `_media` folder, you may want to copy images files into folder `_media` when you drag/drop or paste images into Markdown file automatically. Here's how:

1. Save your file into some path.

2. Enable `Editor` → `Image Insert` → `Allow copy images to given folder` in preferences panel.

   ![Snip20161117_2](img/Snip20161117_2.png)

3. Select `Edit` → `Image Tools` → `When Insert Local Images` → `Copy Image File to Folder` from menubar, pick the target folder.

   ![Snip20161117_6](img/Snip20161117_6.png)

In step 3, a new item `typora-copy-images-to: {relative path}` will be inserted into the [YAML Front Matter][] block of current document. So you could also manually add **typora-copy-images-to** property in YAML Front Matter to enable this behaviour.

After that, if you drag & drop **local** images or paste images into Typora, the image file will be copied into the target file and update related `src`.

### Загрузите файл изображения на веб-сервер. (только для macOS) - Upload image file to web server. (macOS only)

> ** Требования **: установка macOS ≥ 10.11 и [iPic] []. Кроме того, вам нужно включить `Allow upload to given server` в панели настроек.
>
> ** Предупреждение **: По умолчанию iPic будет анонимно загружать изображения на общедоступный веб-сервер, и вы не сможете удалять файлы изображений с этого веб-сервера после его загрузки в него. Поэтому, пожалуйста, настройте iPic заранее, если вы хотите включить эту функцию и управлять всеми загруженными вами файлами изображений.

Вот как включить эту функцию:

1. Установите [iPic] [] и ** config ** соответствующую службу онлайн-изображения.
2. Включите «Редактор» → «Вставка изображения» → «Разрешить копирование изображений в указанную папку» на панели настроек.
3. Проверьте элемент «Редактировать» → «Инструменты изображения» → «При вставке локальных изображений» → «Загрузить изображение через iPic» из меню.

На шаге 3 новый элемент `typora-copy-images-to: ipic` будет вставлен в блок [YAML Front Matter] [] текущего документа.

Таким образом, вы также можете вручную добавить ** typora-copy-images-to: ipic ** свойство в YAML Front Matter, чтобы включить это поведение.

Советы. Если вы хотите переместить файл изображения в папку `ipic`, вы должны использовать` typora-copy-images-to:. / Ipic`.

> **Requirements**: macOS ≥ 10.11 and [iPic][] to be installed. Also, you need to enable `Allow upload to given server` in preferences panel.
>
> **Warning**: By default, iPic will upload images to a public web server anonymously, and you won't be able to delete image files from that web server once you upload into it. So please config iPic in advance if you want to enable this feature and control all image files you uploaded.

Here's how to enable this function:

1. Install [iPic][] and **config** a proper online image service.
2. Enable `Editor` → `Image Insert` → `Allow copy images to given folder` in preferences panel.
3. Check item `Edit` → `Image Tools` → `When Insert Local Images` → `Upload Image via iPic` from menubar.

In step 3, a new item `typora-copy-images-to: ipic` will be inserted into the [YAML Front Matter][] block of current document. 

So you could also manually add **typora-copy-images-to: ipic** property in YAML Front Matter to enable this behaviour.

Tips: If you want to move image file to folder `ipic`, you should use `typora-copy-images-to: ./ipic`.

## Отображение изображений в относительном пути - Display images in relative path - (H2)

### Относительный путь к текущему файлу / папке (поведение по умолчанию) - Relative path to current file/folder (default behavior)

По умолчанию пользователи могут ссылаться на локальное изображение по относительному пути к текущему файлу `* .md`. Например, если файл `* .md` находится в` / User / typora / desktop / test.md`, тогда `! [Img] (image.png)` будет отображать изображение из `/ User / typora / desktop / image.png `как тег` <img> `в HTML. Кроме того, для `../ download / image.png` будет загружено изображение из` / User / typora / download / image.png`.

By default, users could refer to local image by relative path to current `*.md` file. For example, if the `*.md` file is at `/User/typora/desktop/test.md`, then the `![img](image.png)` will display image from `/User/typora/desktop/image.png` just like the `<img>` tag in HTML. Also, for `../download/image.png`, image from `/User/typora/download/image.png` will be fetched.

### Относительный путь к определенной папке - Relative path to certain folder

Если вы используете уценку для создания веб-сайтов, вы можете указать префикс url для предварительного просмотра изображения на локальном компьютере с свойством `typora-root-url` в YAML Front Matters.

Например, введите `typora-root-url: / User / Abner / Website / typora.io /` в YAML Front Matters, а затем `! [Alt] (/ blog / img / test.png)` будет рассматриваться как `! [alt] (файл: ///User/Abner/Website/typora.io/blog/img/test.png)` in typora.

В новой версии вместо того, чтобы вручную вводить свойство typora-root-url`, вы можете просто щелкнуть элемент из меню «Редактировать» → «Инструменты изображения» → «Использовать корневой путь изображения», чтобы сообщить Typora создать «typora-root-url» `свойство автоматически.

If you’re using markdown for building websites, you may specify a url prefix for image preview in local computer with property `typora-root-url` in YAML Front Matters. 

For example, input `typora-root-url:/User/Abner/Website/typora.io/` in YAML Front Matters, and then `![alt](/blog/img/test.png)` will be treated as `![alt](file:///User/Abner/Website/typora.io/blog/img/test.png)` in typora.

In new version, instead of manually input `typora-root-url` property, you could just click item from menubar `Edit` → `Image Tools` → `Use Image Root Path` to tell Typora to generate `typora-root-url` property automatically.

## Загрузка изображений на облачный сервер (только для MacOS) - Upload images to cloud server (macOS only) - (H2)

### Введение в iPic - Introduction to iPic

! [IPIC] (IMG / ipic.jpg)

[iPic] [] - приложение, которое позволяет загружать локальные изображения в различные облачные сервисы, включая [Imgur] (http://imgur.com/), [Flickr] (https://www.flickr.com/) , [Amazon S3] (https://aws.amazon.com/s3/) и т. Д., И верните вам URL-адрес загруженного изображения для общего доступа. Вы можете найти подробные документы [здесь] (http://toolinbox.net/en/iPic/).

Благодаря интеграции [iPic] [] пользователи могут совместно использовать файл разметки другим, не упаковывая локальные изображения вместе с текстовым файлом. Пользователи могут перестать заботиться о том, где размещать локальные изображения или как ссылаться на локальные изображения, используя относительный путь, поскольку они могут просто загружать используемые изображения в облачный сервер.

![ipic](img/ipic.jpg)

[iPic][] is an app which allows you to upload local images into various cloud service, including  [Imgur](http://imgur.com/), [Flickr](https://www.flickr.com/),[ Amazon S3](https://aws.amazon.com/s3/), etc, and return you a web url of the uploaded image for public access. You could find detailed documents [here](http://toolinbox.net/en/iPic/).

With the integration of [iPic][], users could share markdown file to others without packaging local images along with the plain text file. And users can stop caring about where to put local images or how to refer local images using relative path, since they can simply upload used images into cloud server.

### Системные требования и подготовка - System requirements and preparation

1. Эта функция поддерживает только macOS ≥ 10.11.
2. Необходимо установить последнюю версию [iPic] [].
3. Настройте веб-сервер в [iPic] [].

4. This feature only supports macOS ≥ 10.11.
5. Must install latest version of [iPic][].
6. Configure web server in [iPic][].

### Загружать все локальные изображения в облачный сервер - Upload all local images to cloud server

Typora предоставляет функцию загрузки всех локальных изображений на облачный сервер через [iPic] []. Чтобы использовать его, просто выберите «Редактировать» → «Инструменты изображения» → «Загрузить локальные изображения через iPic» из меню и дождитесь завершения процесса загрузки.

Typora provides a function to upload all local images to cloud server via [iPic][]. To use it, simply, check `Edit` → `Image Tools` → `Upload Local Images via iPic` from menubar and wait for the uploading process to be finished.

### Загрузка при вставке изображений - Upload when inserting images

How-tos for this part can be found in section [When insert local image…](#when-insert-local-image…) → Upload image file to web server. (macOS only).

## Выравнивание изображений - Align images - (H2)

В настоящее время Typora не поддерживает выравнивание изображения. Но вы можете использовать HTML-код, например `<center>! [Img] (src) </ center>` для выравнивания изображений на экспортированных HTML или PDF.

Кроме того, по умолчанию, если один абзац содержит только одно изображение, он будет выровнен по центру. Он управляется CSS и может быть возвращен [добавить пользовательский CSS] (http://support.typora.io/Add-Custom-CSS/):

`` `CSS
p .md-image: only-child {
     ширина: авто;
     text-align: inherit;
}
`` `

Currently Typora does not support image alignment. But you could use HTML code like `<center>![img](src)</center>` to align images on exported HTML or PDF.

Also, by default, if one paragraph only contains one image, it will be center aligned. It is controlled by CSS, and can be reverted by [add custom CSS](http://support.typora.io/Add-Custom-CSS/):

```css
p .md-image:only-child{
    width: auto;
    text-align: inherit;
}
```

## Изменение размера изображений Resize images - (H2) 

Please check [this link](http://support.typora.io/Resize-Image/).



[YAML Front Matter]: http://yaml.org/
[iPic]: https://itunes.apple.com/app/id1101244278?ls=1&amp;amp;amp;amp;amp;mt=12