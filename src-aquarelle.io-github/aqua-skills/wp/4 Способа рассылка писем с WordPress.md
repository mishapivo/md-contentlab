# 4 Способа рассылка писем с WordPress

[Главная](https://www.wordpress-abc.ru/) » [Уроки WordPress](https://www.wordpress-abc.ru/uroki-wordpress) » 4 Способа рассылка писем с WordPress

![4 Способа рассылка писем с Wordpress](https://www.wordpress-abc.ru/wp-content/uploads/2015/12/rassyilka-pisem-wordpress-1.jpg)

Содержание

- [Вступление](https://www.wordpress-abc.ru/uroki-wordpress/4-sposoba-rassyilka-pisem-s-wordpress.html#i)
- [4 Способа рассылка писем с WordPress — от простого к сложному](https://www.wordpress-abc.ru/uroki-wordpress/4-sposoba-rassyilka-pisem-s-wordpress.html#4___WordPress_8212)
- [Доставка писем WordPress (wp_mail)](https://www.wordpress-abc.ru/uroki-wordpress/4-sposoba-rassyilka-pisem-s-wordpress.html#_WordPress_wp_mail)
- [Доставка писем FeedBurner](https://www.wordpress-abc.ru/uroki-wordpress/4-sposoba-rassyilka-pisem-s-wordpress.html#_FeedBurner)
- [Доставка писем плагинами почтовых рассылок WordPress](https://www.wordpress-abc.ru/uroki-wordpress/4-sposoba-rassyilka-pisem-s-wordpress.html#___WordPress)
- Рассылка писем сервисами моментальных рассылок
  - [Выводы статьи](https://www.wordpress-abc.ru/uroki-wordpress/4-sposoba-rassyilka-pisem-s-wordpress.html#i-3)
  - [Другие Уроки WordPress](https://www.wordpress-abc.ru/uroki-wordpress/4-sposoba-rassyilka-pisem-s-wordpress.html#_WordPress)

## Вступление

Было бы странным, если такая популярная система управления сайтом (CMS), как WordPress не имела расширенный функционал рассылки писем. Но вопрос не в наличие такой возможности. Для начала, вспомним, что WordPress, и без рассылки писем,  «любит» обращаться к базе данных и как следствие, создает серьезную нагрузку на сервер хостинга. Если к этому добавить рассылку писем, сотням и тем более тысячам подписчиков, то нагрузка на сервер может «зашкалить» и хостинг-провайдер может принять ее за спам рассылку. После чего, как минимум напишет вам гневное письмо, но, как правило, заблокирует ваш домен, до «устранения проблемы» или «перехода на другой тарифный план».

**Примечание:** В нагрузке на сервер важно значение имеет сборка самого сервера. Если он построен на «чистом» http Apache, то один запрос будет обрабатываться одним процессом и превышение нагрузки на сервер наиболее вероятно. Если сервер построен на Nginx или Nignx+ Apache, то будет обрабатываться тысячи запросов (соединений) одним процессом, что значительно уменьшает вероятность принять вашу рассылку за спам.

Покажу** 4 Способа рассылка писем с WordPress**. Использовать их можно последовательно по мере набора активных подписчиков. Под активными подписчиками мы понимаем получателей писем, которые реально открывают письма с вашими рассылками, а не фантомы из купленных баз.

## 4 Способа рассылка писем с WordPress — от простого к сложному

Перечислю эти четыре способа:

- Рассылка писем с доставкой WordPress;
- Рассылка писем с доставкой FeedBurner;
- Рассылка писем плагинами почтовых рассылок WordPress;
- Рассылка писем сервисами моментальных рассылок.

## Доставка писем WordPress (wp_mail)

Как я уже упоминал, функционал WordPress позволяет по умолчанию отправлять письма с анонсами новых статей, своим подписчикам и пользователям (функция wp_mal). Как проверить работу почтового сервиса WordPress можно прочитать в статье ([Рассылка новостей и писем на WordPress](https://www.wordpress-abc.ru/administrirovanie/rss-wordpress/rassyilka-novostey-i-pisem-na-wordpress.html)). Работает такая рассылка с [плагином JetPack](https://www.wordpress-abc.ru/plaginy/podpiski-plaginom-jetpack.html), в автоматическом режиме следующим образом:

Набираем подписчиков, разместив виджет с формой подписки на сайте. Список подписчиков не видим, видим только их количество.

Собираем пользователей сайта. Для этого размещаем на сайте вижджет с названием «Мета» со ссылкой «Регистрация» или в статью вставляем ссылку на страницу авторизации или регистрации, где пользователь проходит простую регистрацию (ссылка типа: *http://exemple.net/wp-login.php* или *http://exemple.net/wp-login.php?action=register*).

[![Форма авторизации wordpress](https://www.wordpress-abc.ru/wp-content/uploads/2015/12/wp-login-stranitsa-314x448.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/12/wp-login-stranitsa.jpg)Форма авторизации wordpress

[![Форма регистрации WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2015/12/stranitsa-registratsii-wordpress-302x448.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/12/stranitsa-registratsii-wordpress.jpg)Форма регистрации WordPress

Внешний вид виджета можно изменить, а также шорткодом добавить форму подписки в статьи. Подробнее в новой статье: [Подписки плагином JetPack: размещение и редакция формы подписки JetPack](https://www.wordpress-abc.ru/plaginy/podpiski-plaginom-jetpack.html)

При этом в общих настройках сайта (*Настройки→Общие*) присваиваем [Пользователю](https://www.wordpress-abc.ru/administrirovanie/polzovateli-wordpress.html) права, как минимум, подписчик, что бы он получал рассылки с [доставкой почтовой службой WordPress.com](https://www.wordpress-abc.ru/administrirovanie/nastrojki-wordpress/pochtovaya-sluzhba-wordpress-com.html). Кстати, на последних версиях WordPress, внешний вид писем, стал, вполне, респектабельным, со ссылками на три последние статьи и другими, цепляющими фишками.

[Читайте так же:  Что такое тема WordPress](https://www.wordpress-abc.ru/uroki-wordpress/chto-takoe-tema-wordpress.html)

[![письмо подтверждение wordpress подписка-3](https://www.wordpress-abc.ru/wp-content/uploads/2015/12/pismo-podtverzhdenie-wordpress-podpiska-3-324x350.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/12/pismo-podtverzhdenie-wordpress-podpiska-3.jpg)внешний вид писем с доставкой WordPress.com

Еще один способ сбора, не явных (вы о них можете вообще не знать) подписчиков, вывесить виджет «Ссылки RSS» своего сайта. Это для любителей получать письма обновления сайта по каналам RSS рассылок.

## Доставка писем FeedBurner

Для начала замечу, несмотря на довольно устаревший функционал и убогий внешний вид рассылок, сервис FeedBurner остается самым стабильным и «непотопляемым» сервисом RSS рассылок новостей.

Доставка писем через сервис FeedBurner был распространен, и даже рекомендуем, многими веб мастерами. Но после закрытия Reader, сервис остановился в своем развитии и как следствие, становится не интересным. Хотя многие и я в том числе, продолжаю размещать подписку с доставкой FeedBurner.

[![FeedBurner подписка WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2015/12/feedBurner-podpiska-448x259.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/12/feedBurner-podpiska.jpg)Виджет FeedBurner

[![feedBurner-подписка-5](https://www.wordpress-abc.ru/wp-content/uploads/2015/12/feedBurner-podpiska-5-448x225.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/12/feedBurner-podpiska-5.jpg)Подтверждение feedBurner подписки

[Читайте так же:  Установка и удаление плагина на WordPress](https://www.wordpress-abc.ru/uroki-wordpress/ustanovka-udalenie-plagina-na-wordpress.html)

## Доставка писем плагинами почтовых рассылок WordPress

Сразу замечу, при большом количестве подписчиков, все плагины почтовых рассылок могут перегружать сервис хостинга и восприниматься, как спам рассылка. Стремитесь найти плагин с настройками периодичности отправки писем, где-то 20-25 писем в час.

Я рассказывал о некоторых плагинах почтовых рассылок, здесь перечислю наиболее популярные:

- [MailPress](https://www.wordpress-abc.ru/plaginy/plagin-mailpress-dlya-pochtovoj-rassylki-wordpress.html);
- [Mail Poet Newsletter](https://www.wordpress-abc.ru/plaginy/plagin-rassyilki-mailpoet-newsletters.html);
- Subscribe 2;
- MailChimp;
- BuddyPress (социальные сети).

## Рассылка писем сервисами моментальных рассылок

Лучший вариант, для рассылки большого количества писем своим подписчикам или «купленным» подписчикам, это использовать специальные сервера почтовых рассылок. Преимуществ в таких сервисах несколько:

- Минимальная нагрузка на сервер;
- Отправка писем тысячам подписчикам;
- Управление внешним видом писем;
- Красивая, «цепляющая» страница с формой подписки.

~~И, конечно же, лучший вариант такого сервиса в Рунете~~, сервис «[Smartresponder](https://www.wordpress-abc.ru/administrirovanie/rss-wordpress/rassyilka-pisem-na-servise-smartresponder.html)».

Лучший, потому что можно в него можно импортировать своих подписчиков из «умирающего» FeedBurner и не только из него, и потому-то, есть специальный плагин, который без проблем свяжет ваш сайт WordPress с сервисом Smartresponder.

**Примечание:** Плагина Smartresponder нет в списке плагинов WordPress.org. Скачать его нужно на сайте сервиса Smartresponder, после регистрации (тут: https://smartresponder.ru/l_ru/integration/wordpress.html). Установить старым добрым способом, через страницу *Плагины→ Добавить новый→Загрузить плагин*. Затем активировать и начать использовать. Подробная инструкция на той же странице: smartresponder.

[Читайте так же:  Домен для WordPress сайта](https://www.wordpress-abc.ru/uroki-wordpress/domen-dlya-wordpress-3.html)

[![Smartresponder](https://www.wordpress-abc.ru/wp-content/uploads/2015/12/Smartresponder-448x193.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/12/Smartresponder.jpg)Плагин Smartresponder

**Примечание:** Западный аналог Smartresponder, сервис рассылок Mandril. (http://www.mandrill.com/). Он синхронизируется плагином «wpMandrill» и отменят функцию wp_mail, а также используется в плагине рассылок MailChimp.

> На момент редактирования статьи, ноябрь 2016, считаю лучшим вариантом рассылок, сервис MailChimp с формой подписки MailMunch.

### Выводы статьи

Важна возможность выбора способов рассылки своих анонсов, новостей и писем. У вас есть возможность выбрать способ рассылки доступный и полезный для вас, при этом оценить нагрузку на сервер.

Игорь Серов специально для сайта «[Как сделать сайт WordPress](https://www.wordpress-abc.ru/)»

### Другие Уроки WordPress

- [Первые настройки WordPress](https://www.wordpress-abc.ru/uroki-wordpress/pervyie-nastroyki-wordpress.html)
- [Сайдбар и виджеты WordPress](https://www.wordpress-abc.ru/uroki-wordpress/saydbar-vidzhetyi-wordpress.html)
- [Что такое тема WordPress](https://www.wordpress-abc.ru/uroki-wordpress/chto-takoe-tema-wordpress.html)
- [Создаем меню WordPress: как создать меню WordPress](https://www.wordpress-abc.ru/uroki-wordpress/sozdaem-menyu-wordpress.html)
- [Установка и удаление плагина на WordPress](https://www.wordpress-abc.ru/uroki-wordpress/ustanovka-udalenie-plagina-na-wordpress.html)
- [Настройки постоянных ссылок WordPress](https://www.wordpress-abc.ru/uroki-wordpress/nastroyki-postoyannyih-ssyilok-wordpress.html)
- [Публикация статей в WordPress](https://www.wordpress-abc.ru/uroki-wordpress/publikatsiya-statey-v-wordpress.html)
- [Установка WordPress на сервер хостинга](https://www.wordpress-abc.ru/uroki-wordpress/ustanovka-wordpress-na-server-hostinga.html)
- [Как объединить два сайта WordPress](https://www.wordpress-abc.ru/uroki-wordpress/kak-obedinit-dva-sayta-wordpress.html)
- [Что такое плагины WordPress](https://www.wordpress-abc.ru/uroki-wordpress/chto-takoe-plaginyi-wordpress-2.html)