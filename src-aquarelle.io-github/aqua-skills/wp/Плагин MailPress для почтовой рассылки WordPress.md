# Плагин MailPress для почтовой рассылки WordPress

[Главная](https://www.wordpress-abc.ru/) » [Плагины](https://www.wordpress-abc.ru/plaginy) » Плагин MailPress для почтовой рассылки WordPress

![Плагин MailPress для почтовой рассылки WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/MailPress-wordpress.jpg)

Если Вы хотите организовать почтовую рассылку непосредственно со своего  WordPress, можете попробовать мощный плагин  MailPress. При помощи плагина MailPress можно организовать  настраиваемую,  независимую от RSS, многофункциональную почтовую рассылку, как новостей сайта, так и сторонних писем. Причем вы можете выбрать внешний вид (шаблон) отправляемых писем.

Содержание

- [Где скачать плагин MailPress](https://www.wordpress-abc.ru/plaginy/plagin-mailpress-dlya-pochtovoj-rassylki-wordpress.html#__MailPress)
- [Установка плагина почтовой рассылки MailPress](https://www.wordpress-abc.ru/plaginy/plagin-mailpress-dlya-pochtovoj-rassylki-wordpress.html#__MailPress-2)
- [Активация плагина MailPress](https://www.wordpress-abc.ru/plaginy/plagin-mailpress-dlya-pochtovoj-rassylki-wordpress.html#_MailPress)
- Настройка плагина  MailPress
  - [Настройка внешнего вида рассылки плагина MailPress](https://www.wordpress-abc.ru/plaginy/plagin-mailpress-dlya-pochtovoj-rassylki-wordpress.html#___MailPress)
  - [Управление подписчиками](https://www.wordpress-abc.ru/plaginy/plagin-mailpress-dlya-pochtovoj-rassylki-wordpress.html#i)
  - [Экспорт и импорт подписчиков](https://www.wordpress-abc.ru/plaginy/plagin-mailpress-dlya-pochtovoj-rassylki-wordpress.html#i-2)
  - [Настройка автоответчика](https://www.wordpress-abc.ru/plaginy/plagin-mailpress-dlya-pochtovoj-rassylki-wordpress.html#i-3)
  - [Написание писем](https://www.wordpress-abc.ru/plaginy/plagin-mailpress-dlya-pochtovoj-rassylki-wordpress.html#i-4)
  - Виджет подписки
    - [Примечание](https://www.wordpress-abc.ru/plaginy/plagin-mailpress-dlya-pochtovoj-rassylki-wordpress.html#i-6)

## Где скачать плагин MailPress

Прежде всего, скачайте плагин со страницы плагина на WordPress.org (ссылка[ ТУТ](http://wordpress.org/plugins/mailpress/)). Последняя версия 5.4 требует установленной версии WordPress 3.6. Распакуйте скачанный архив (mailpress.zip). Проверьте наличие в архиве папки [tmp] для запуска.

Сразу отмечу, что плагин постоянно обновляется, но его обновление несколько усложнено, по сравнению с другими плагинами WP.

Важно, если у вас установлен и работает плагин MailPress, то нельзя обновлять его автоматически. Автоматическое обновление плагина  удалит все ваши предыдущие настройки.

## Установка плагина почтовой рассылки MailPress

- Для установки плагина MailPress у вас должен быть доступ в административную панель сайта.
- По FTP загрузите папку mailpress, распакованного архива, в каталог сайта в директорию [wp-content/plugins];
- Далее войдите в административную панель сайта, во вкладку «Плагины установленные»;
- Найдите в списке своих плагинов плагин MailPress и активируйте его. После активации меню плагина появится консоли WP.

## Активация плагина MailPress

Плагин MailPress очень объемный и включает большое количество дополнительных, нужных и «не нужных», расширений. Для начала нужно активировать основные расширения. Для этого откройте вкладку «Add-on» в меню плагина. Вкладка находится  под названием плагина в списке плагинов или в  консоли, в пункте меню Плагины→ MailPress Add-ons.

[![Mailpress_plagin_wp_13](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_13.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_13.jpg)

Список расширений «MailPress Add-ons» достаточно большой. Не нужно активировать все подряд. Для информации о каждом расширении пользуйтесь кнопкой «Visit add-on page».

[![Mailpress_plagin_wp_03](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_03.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_03.jpg)

Для начала работы с плагином активируйте Connection_php_mail. Это  подключение встроенной функции почты mail php.

## Настройка плагина  MailPress

Все настройки плагина находятся по пути: Параметры → MailPress (2). Обращу ваше внимание, что управление плагином находится в отдельном меню консоли «Mails»(3), а включение плагинов Mailpress во вкладке Плагины →  MailPress Add-ons(1).

[Читайте так же:  Media File Cleaner плагин WordPress для чистки Media Library](https://www.wordpress-abc.ru/plaginy/media-file-cleaner-plagin-wordpress-dlya-chistki-media-library.html)

[![Mailpress_plagin_wp_16](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_16.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_16.jpg)

Заходим в Параметры → MailPress. Это страница MailPress Settings (настройки MailPress). В настройках плагина четыре вкладки (фото ниже): General, PHP_Mail, Test, Logs.

Основная настройка General. Основные настройки разделены три части. Первая часть это email обратного адреса и название вашей рассылки. Вторая часть это вид рассылки на сайте и вид формы подписки. Третья часть это, что выводиться в административной панели сайта.

[![Mailpress_plagin_wp_04](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_04.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_04.jpg)

PHP_Mail –необязательная настройка. Можете указать пятый параметр в стандартной php функции (php mail). Это пример функции php mail.

```
bool mail (string $to , string $subject , string $message [, string $additional_headers [, string $additional_parameters]] )
```

[![Mailpress_plagin_wp_05](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_05.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_05.jpg)

**Test.** Это вкладка для тестовой рассылки «самому себе». В настройке тестового письма укажите свой адрес, куда отправить тестовое письмо и выберите произвольную Тему(Theme) и Шаблон (Template) тестового письма. Вы, конечно, сразу можете повозиться с темами и выбрать тему для всех ваших будущих рассылок, но задача на этом этапе просто протестировать работоспособность плагина, и неважно в каком виде вы получите тестовое письмо. О внешнем виде вашей рассылки можете позаботиться позже.

[![Mailpress_plagin_wp_08](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_08.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_08.jpg)

[![Mailpress_plagin_wp_14](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_14.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_14.jpg)

**Logs **–эта вкладка настройка журнала ошибок рассылки. Вы можете настроить вывод  ошибок в три журнала ошибок и включить в них  вывод различных ошибок. Список , какие ошибки выводить в лог, внушительный. Нужно выбрать тип вывода ошибок из выпадающего списка. Самые общие ошибки это вывод типа E_ALL. На скриншоте этот тип вывода ошибок последний.

[![Mailpress_plagin_wp_07](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_07.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_07.jpg)

После выставления всех настроек, а особенно тестовой настройки, сохраните настройки. После сохранения настроек проверьте получение тестового письма по указанному в настройке test адресу. Если письмо прошло, можно детально настраивать плагин MailPress.

### Настройка внешнего вида рассылки плагина MailPress

Все настройки и управление плагина MailPress осуществляются через меню плагина.

[![Mailpress_plagin_wp_15](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_15.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_15.jpg)

Сейчас настроим внешний вид вашей будущей рассылки. Здесь все просто. Открываете в меню Mails → Themes. Видите страницу с шаблонами рассылки аналогичной странице с шаблонами сайта. Выбираете шаблон, можете его посмотреть и потом активировать. Лежат все темы рассылки  MailPress в папке: wp-content/plugins/mailpress/mp-content/themes/. Внешний вид рассылки настроен.

[![Mailpress_plagin_wp_12](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_12.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_12.jpg)

### Управление подписчиками

Войдите в Плагины → MailPress Add-ons. В списке  внутреyних плагинов MailPress, активируйте плагин Sync_wordpress_user (Синхронизация с пользователей  WordPress). Тем самым все пользователи сайта станут и будут становиться в дальнейшем, подписчиками MailPress.

[Читайте так же:  Вставляем произвольный код в посты и страницы WordPress](https://www.wordpress-abc.ru/plaginy/vstavlyaem-proizvolnyiy-kod-v-postyi-i-stranitsyi-wordpress.html)

[![Mailpress_plagin_wp_17](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_17.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_17.jpg)

Кроме пользователей WordPress, подписчики  на рассылку MailPress будут добавляться в пользователи плагина по мере подписки, форму которой вы разместите на сайте (читать ниже). Но кроме этих подписчиков вы можете импортировать подписчиков из других сервисов почтовой рассылки.

Если не активировать плагин Sync_wordpress_user (Синхронизация с пользователей  WordPress), то пользователи сайта WordPress  и подписчики MailPress будут разделены. Это  позволит сделать тематическую рассылку, отличную от новостей сайта. Например, подписчики на новости вашего сайта ( пользователи), будут получать информацию о выходе новых статей, а  подписчики  MailPress, будут получать тематические письма. В вопросе организации рассылок, плагин MailPress, позволяет организовать самые разнообразные схемы. Выбор за вами.

### Экспорт и импорт подписчиков

Плагин MailPress, позволяет импортировать своих подписчиков и экспортировать подписчиков с других почтовых сервисов. Для импорта подписчиков, войдите в Плагины → MailPress Add-ons. В списке плагинов активируйте плагин Import.

[![Mailpress_plagin_wp_06](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_06.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_06.jpg)

Если у вас есть электронная рассылка почты в других системах электронной рассылки, MailPress может импортировать и экспортировать пользователей (подписчиков), а также импортировать данные из аналогичного плагина для WordPress Subscribe2.

[![Mailpress_plagin_wp_10](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_10.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_10.jpg)

Обращу внимание на импорт подписчиков. Вы можете импортировать своих подписчиков с других сервисов рассылок. Импорт подписчиков осуществляется в формате csv. Причем, не обязательно чтобы сервис экспортер был на WordPress. Я, например, импортировал подписчиков с сайта на Joomla из рассылки AcyMail.

Механизм экспорта-импорта очень прост. На сервере экспортере делаете файл в формате csv с данными нужных подписчиков, а на WordPress (вкладка Mails→Import/Export) импортируете этот список. Ограничений, в количестве импортируемых подписчиков, я не знаю. Я максимально импортировал 600 подписчиков. При импорте плагин MailPress отлично фильтрует дубли подписчиков.

### Настройка автоответчика

Как и ранее, войдите в Плагины → MailPress Add-ons и включите плагин Autoresponder (автоответчик). В настройки автоответчика можно перейти отсюда (параметры) или во вкладке Mails → Autoresponders из меню консоли.

[![Mailpress_plagin_wp_19](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_19.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_19.jpg)

Важный пункт настройки автоответчика это Slug (уникальный идентификатор для автоответчика). Он должен быть вписан латинскими буквами в нижнем регистре. Не забудьте заполнить Name (Имя) и Description (Описание).

[Читайте так же:  Управление виджетами Wordpress](https://www.wordpress-abc.ru/plaginy/upravlenie-vidzhetami-wordpress.html)

[![Mailpress_plagin_wp_09](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_09.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_09.jpg)

### Написание писем

Письма рассылки пишутся во вкладке Mails → Add New. Здесь тоже все несложно.

Письмо пишется, как и статья сайта в аналогичном основном поле визуального редактора. Поле Plaintext это текст письма в Html, он нужен для старых почтовых серверов. Этот текст самому заполнять не нужно. Достаточно воспользоваться кнопкой синхронизации (слева вверху), после написания письма в основном окне визуального редактора.

[![Mailpress_plagin_wp_11](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_11.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_11.jpg)

Пользовательские поля могут быть использованы для добавления дополнительных метаданных для почты. Эта функция новая на версии WP 3.6.

Внизу страницы вы можете включить написанное письмо в автоответчик. Автоответчик это письмо, которое можно отправлять автоматически с установленной периодичностью. Например, напоминание об активации подписки и постоянные письма с продажей чего либо или продажа инфо-продукта и т.д.

[![Mailpress_plagin_wp_20](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_20.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_20.jpg)

### Виджет подписки

Вы можете разместить форму подписки на свою рассылку в виджетах сайта.  Активируется виджет подписки после активации плагина.

В настройках виджета можете указать наименование, надпись на кнопке подписки и поставить ссылку (link) куда перенаправить подписчика во время подписки, например, на страницу, рассказывающую, о чем подписка.

[![Mailpress_plagin_wp_21](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_21.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_21.jpg)

[![Mailpress_plagin_wp_22](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_22.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2013/10/Mailpress_plagin_wp_22.jpg)

#### Примечание

- Вы уже, наверное, поняли, что любые новые настройки плагин MailPress включает после включения соответствующего плагина во вкладке MailPress Add-ons.
- Плагин MailPress при автоматическом обновлении теряет все свои настройки. Про обновление плагина почитайте страницу плагина на Plugin Directory WordPress.org или на сайте MailPress.

На этом про Плагин MailPress для почтовой рассылки WordPress все.

Игорь Серов специально для сайта «[Как сделать сайт WordPress](https://www.wordpress-abc.ru/)»

### Другие статьи раздела: Плагины

- Записи не найдены