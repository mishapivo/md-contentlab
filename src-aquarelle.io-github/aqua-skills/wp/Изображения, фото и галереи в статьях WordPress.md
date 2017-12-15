# Изображения, фото и галереи в статьях WordPress

[Главная](https://www.wordpress-abc.ru/) » [Администрирование](https://www.wordpress-abc.ru/administrirovanie) » Изображения, фото и галереи в статьях WordPress

![Изображения, фото и галереи в статьях Wordpress](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/wordpress-galereya.jpg)

Изображения, фото и галереи в статьях WordPress это обязательный атрибут современного медийного ресурса. В WordPress встраивать изображения в посты сайта можно различными способами. В этой статье я расскажу, как управлять  медиафайлами (фотографиями, картинками) на сайте WordPress без установки дополнительных плагинов.

Скриншоты поста сняты c версии ранее WordPress 3.8.

Для WP есть масса плагинов для работы с  изображениями. Но в этой статье рассмотрим  внутренний инструмент WordPress для вставки изображений в пост. C его помощью можно вставлять как, отдельные фото, так и целые  галереи. Причем как изображения, так и галереи пожеланию можно настраивать.

Содержание

- Общие настройки изображения, фото и галереи в статьях WordPress
  - [Миниатюра статьи](https://www.wordpress-abc.ru/administrirovanie/izobrazheniya-foto-i-galerei-v-statyax-wordpress.html#i)
- Загрузка файлов
  - [Привязанные и не привязанные фото](https://www.wordpress-abc.ru/administrirovanie/izobrazheniya-foto-i-galerei-v-statyax-wordpress.html#i-3)
- [Как вставить в статью WP изображение](https://www.wordpress-abc.ru/administrirovanie/izobrazheniya-foto-i-galerei-v-statyax-wordpress.html#__WP)
- [Редактирование, дороботка фото в статье](https://www.wordpress-abc.ru/administrirovanie/izobrazheniya-foto-i-galerei-v-statyax-wordpress.html#i-4)
- [Как вставить галерею в статью WordPress](https://www.wordpress-abc.ru/administrirovanie/izobrazheniya-foto-i-galerei-v-statyax-wordpress.html#___WordPress)
- Добавление галерей при помощи кодов
  - [Добавить галерею с прикрепленными к статье фото](https://www.wordpress-abc.ru/administrirovanie/izobrazheniya-foto-i-galerei-v-statyax-wordpress.html#i-6)

## Общие настройки изображения, фото и галереи в статьях WordPress

В [настройках](https://www.wordpress-abc.ru/administrirovanie/nastrojki-parametrov-wordpress-obshhie-nastrojki-nastrojki-napisaniya-i-chteniya-statej-bloga-wpspisok-ping-sajtov.html) сайта можно выставить размеры показываемых изображений. Для этого авторизуйтесь в [admin панели](https://www.wordpress-abc.ru/administrirovanie/konsol-sajta-wordpress.html) своего сайта WP. В меню консоли нужен пункт Параметры→Медиафайлы.

[![Konsol-wordpress-10](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Konsol-wordpress-10-256x300.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Konsol-wordpress-10.png)

Откроется страница настроек изображений для вставки в статьи, по-умолчанию. Здесь видим три параметра размеров изображений: размер миниатюры, средний размер, крупный размер.

[![Изображения, фото и галереи в статьях WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Obshhie-nastroyki-WP-091-400x219.png)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Obshhie-nastroyki-WP-091.png)настройки медиафайлов wordpress

[Читайте так же:  Новый Wordpress3.9](https://www.wordpress-abc.ru/administrirovanie/novyiy-wordpress3-9.html)

Объясню, зачем нужны три размера фотографий. При вставки изображения в статью, в редакторе в форме «Добавить медиафайл»,  Wordpress предлагает на выбор три размера для изображений. Именно параметры, которые вы выставите в этих настройках, будут предлагаться для вставки в статьи.

[![Media](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media.jpg)

### Миниатюра статьи

Кроме этого, при публикации статьи, вам будет предложено создать миниатюру для статьи. Эта миниатюра будет прикреплена к статье и отражаться в различных виджетах и являться, визитной карточкой статьи.

*Для правильного отражения миниатюры в Facebook размер миниатюры должен быть минимум 200×200.*

Размер миниатюры задается в шаблоне при его верстке. Чтобы большие изображения для миниатюр пропорционально обрезались под размер миниатюры, отметьте специальный чекбокс.

[![Media1](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media1-400x166.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media1.jpg)

[Читайте так же:  История развития алгоритмов Google](https://www.wordpress-abc.ru/seo-nachinayushhim/istoriya-razvitiya-algoritmov-google.html)

Крупный размер выставите на максимальное значения 1024×1024. Но если вы хотите, чтобы изображения на всем сайте были ограничены определенными размерами, выставите эти размеры в этом пункте настроек.

## Загрузка файлов

Следующий пункт меню заслуживает внимания, это загрузка файлов.

Все фото сайта загружаются в так называемую «Библиотеку медиафайлов» вашего сайта. *Изображения загружаются сразу в трех размерах указанных в настройках выше.*

Если в настройках медиафайлов в пункте «Помещать загруженные мной файлы в папки по месяцу и году»  поставить галочку

[![Media1a](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media1a-400x166.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media1a.jpg)

,то изображения будут загружаться в следующий каталог:

, где Год/Месяц автоматически создаются по году и месяцу загрузки фото в библиотеку.

Если галочку в пункте не ставить, то все фото будут загружаться в папку:

**Обратите внимание: (1) **Если вы загружаете фото при написании статьи, то фото привязывается к этой статье. **(2)** Если вы по каким либо причинам, при редактировании статьи редактируете фото, то в библиотеке остаются все редакции фото, автоматом они не удаляются. **(3)** Если вы загружаете фото сразу в «Медиафайлы», то фото считается не привязанным.

### Привязанные и не привязанные фото

Объясню, что значит и чем отличаются привязанные и не привязанные фото. Все привязанные к статье фотографии, можно показать в статье в виде простой галереи WordPress, по умолчанию. Для создания простой галереи не нужно ставить дополнительных палгинов, достаточно  в визуальном редакторе в любом месте статьи разместить короткий код для галереи, [gаllery]. Галерея WordPress по умолчанию можно настроить, короткие коды различных видов галереи ниже.

Остановлюсь подробнее как вставлять в статьи отдельные изображения и фото галереи.

## Как вставить в статью WP изображение

Редактор WordPress позволяет полноценно вставлять изображения, фото и галереи в статьях WordPress. Делается это достаточно просто. Проиллюстрирую это примером в скриншотах.

- Открываете **Консоль→Записи→Добавить новую**.
- Для вставления фото в статью нажимаем «Добавить медиафайл».

[![Media-fajly-WP-01](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-01-400x271.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-01.jpg)

Далее по пунктам:

- Выбираем фото либо с компьютера, либо из интернет по URL, либо из библиотеки ранее загруженных фотографий, сайта.

[![Media-fajly-WP-03](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-03-400x166.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-03.jpg)

[![Media-fajly-WP-05](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-05-400x169.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-05.jpg)

[![Media-fajly-WP-04](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-04-400x300.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-04.jpg)

Перед добавлением фото в статью (справа) выбираем размер фото для установки в статью, прописываем теги alt, название фото, при желании описание фото.

[![Media-fajly-WP-09](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-09.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-09.jpg)

- ** **В графе «Ссылка» выставите как, на скриншоте «Медиафайл». Если не установлены плагины, открывающие фото в модальных окнах, типа lightbox, то фото будет открываться в отдельном окне. Если выставить не медиафайл, а «Страница вложения», то фото будет открываться сначала как страница сайта с фото, а только потом в отдельном окне, как фотография. Исправить показ фото можно при редактировании фото. Читать ниже  «Вставляем фото» в статью или страницу.

## Редактирование, дороботка фото в статье

В редакторе можно дополнительно настроить отображение фото. Для этого кликните по фото в редакторе и выберите иконку редактировать. Вторая иконка удаляет фото из статьи.

[![Media-fajly-WP-10](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-10-297x400.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-10.jpg)

В новых версиях WordPress, например 4.4., кнопки редактирования фото несколько изменились:

[![фото-редактор](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/foto-redaktor-448x400.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/foto-redaktor.jpg)

В настройках можно изменить:

- Изменить размер (пропорционально);
- Выбрать ссылку которая будет открываться при клике на фото (Нет, Текущая страница, Ссылка на изображение);

Если вы выставите «Ссылка на это изображение», то фото будет открываться в отдельном окне, под своим URL в библиотеке медиафайлов или в всплывающих окнах, если вы используете плагины для показа фото во всплывающих окнах (типа[Lightbox](https://www.wordpress-abc.ru/plaginy/14-plaginy-dlya-effekta-lightbox-na-sajte-wordpress.html)).

- Изменить положение фото в статье (нет, центр, справа, слева).
- Добавить стиль рамки, отступы по горизонтали и вертикали.

[![Media-fajly-WP-11](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-11-400x344.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-11.jpg)

[![Media-fajly-WP-13](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-13-400x341.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-13.jpg)

Пример Стиля рамки: border: 5px solid red;

[![Media-fajly-WP-14](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-14.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-14.jpg)

## Как вставить галерею в статью WordPress

- Выбрать «Вставить галерею»;
- Выбрать «Загрузить фото»;
- Выбрать на компьютере нужные для галереи фото;
- Настроить показ галереи: количество колонок и порядок показа фото;
- Нажмите «Вставить галерею».

[![Media-fajly-WP-06](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-06-400x186.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-06.jpg)

[![Media-fajly-WP-07](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-07-400x186.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-07.jpg)

[![Media-fajly-WP-08](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-08-400x344.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media-fajly-WP-08.jpg)

Размер миниатюр в галерее будет соответствовать  установленным размерам миниатюр во вкладке (Параметры→Медиафайлы).

## Добавление галерей при помощи кодов

Галереи можно создавать при помощи коротких кодов WordPress в текстовом редакторе (HTML) на странице «Изменить». Для этого переключитесь в текстовой редактор(кнопка «Текст» справа вверху редактора) и вставьте нужный код на выбор из показанных ниже.

**Все коды заключите в квадратные скобки, [код]**

### Добавить галерею с прикрепленными к статье фото

Все фото, которые вы загружаете из редактора при написании статьи привязаны к этой статье. Также можно привязать к статье фотографии из библиотеки медиафайлов.

[![Media3](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media3-400x217.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media3.jpg)

[![Media3a](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media3a-400x274.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/01/Media3a.jpg)

**Интересно:**

Все прикрепленные к статье фото, можно вывести в любом месте статьи, вставив простой код: [gаllery]. После этого все прикрепленные фото к этой статье, появятся в статье в виде галереи.

- **Поясню.** Чтобы создать простую галерею на сайте,** можно не вставлять фото в статьи в редакторе**.
- Создаете статью, в нужном месте текста вставляете короткий код из списка выше.
- Статью сохраняете, публиковать не обязательно.
- Далее идем в Библиотеку медиафайлов, загружаем нужное количество фотографий для галереи и все их прикрепляем к нашей записи.
- Также, можно дополнить любую статью галереей из Менеджера медиафайлов или дополнить галерею не входя в редактор статьи.

 

Игорь Серов специально для сайта «[Как сделать сайт WordPress](https://www.wordpress-abc.ru/)»

### Другие статьи раздела: Администрирование WordPress

- Записи не найдены