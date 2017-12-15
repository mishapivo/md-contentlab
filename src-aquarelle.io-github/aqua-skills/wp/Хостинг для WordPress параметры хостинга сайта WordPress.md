# Хостинг для WordPress: параметры хостинга сайта WordPress

[Главная](https://www.wordpress-abc.ru/) » [Уроки WordPress](https://www.wordpress-abc.ru/uroki-wordpress) » Хостинг для WordPress: параметры хостинга сайта WordPress

![img](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/Hosting-dlya-wordpress.jpg)

Содержание

- [Тема урока](https://www.wordpress-abc.ru/uroki-wordpress/hosting-dlya-wordpress.html#i)
- [Несколько слов о хостинге](https://www.wordpress-abc.ru/uroki-wordpress/hosting-dlya-wordpress.html#i-2)
- [Удаленные сервера](https://www.wordpress-abc.ru/uroki-wordpress/hosting-dlya-wordpress.html#i-3)
- Хостинг
  - [Программное обеспечение хостинга](https://www.wordpress-abc.ru/uroki-wordpress/hosting-dlya-wordpress.html#i-5)
- Параметры хостинга для сайта WordPress
  - [Оперативная память](https://www.wordpress-abc.ru/uroki-wordpress/hosting-dlya-wordpress.html#i-6)
  - [Трафик](https://www.wordpress-abc.ru/uroki-wordpress/hosting-dlya-wordpress.html#i-7)
  - [Цена](https://www.wordpress-abc.ru/uroki-wordpress/hosting-dlya-wordpress.html#i-8)
- [Хостинг для wordpress: выбор хостинга и покупка домена](https://www.wordpress-abc.ru/uroki-wordpress/hosting-dlya-wordpress.html#_wordpress)
- Хостинг и DNS сервера
  - [Итоги урока](https://www.wordpress-abc.ru/uroki-wordpress/hosting-dlya-wordpress.html#i-9)
  - [Полезные ссылки](https://www.wordpress-abc.ru/uroki-wordpress/hosting-dlya-wordpress.html#i-10)
  - [Другие Уроки WordPress](https://www.wordpress-abc.ru/uroki-wordpress/hosting-dlya-wordpress.html#_WordPress)

## Тема урока

В этом уроке я объясню, что такое хостинг и научу вас, выбрать «правильный» хостинг для блога на WopdPress.

## Несколько слов о хостинге

Любой Интернет ресурс, в том числе и блог WordPress, должен, где-то располагаться. То есть, папки и файлы, которые составляют блог WordPress, должны «лежать» на реальном дисковом пространстве.

На время наполнения блога вы можете разместить его у себя на компьютере, установив один из локальных серверов ([Денвер](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/ustanovka-wordpress-na-denver.html), Open Server, [Xmapp](https://www.wordpress-abc.ru/hosting/lokalnyiy-server/kak-ustanovit-wordpress-na-xampp.html),  AMPPS и т.п.) Многие так и делают, а потом переносят сайт на сервер хостинг провайдера.

Можно сразу разметить блог на стороннем (удаленном) сервере и наполнять блог сразу по месту. Это избавит вас от проблем с переносом блога с локального сервера, а при желании позволит сразу выставить блог в сети и постепенно наполнять его содержанием.

## Удаленные сервера

Удаленные сервера это реальные мощные компьютеры, принадлежащие или взятые в аренду компаниями провайдерами. Называются они дата центрами.

[![Хостинг для WordPress](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/datacenter-448x252.jpg)](https://www.wordpress-abc.ru/wp-content/uploads/2015/01/datacenter-448x252.jpg)

## Хостинг

- Место, выделяемое пользователю для размещения своих сайтов, **под общим IP адресом**, называют хостингом.
- Место, выделяемое вам провайдером для ваших сайтов, **под уникальным IP**, называют VPS/VDS сервером.

Хостинг, более подходит для начинающих пользователей. Арендуя хостинг, вам не нужно задумываться об установке программного обеспечения на сервер, за вас все делает Support хостинг-провайдера. Вам остается только правильно выбрать предлагаемые услуги.

### Программное обеспечение хостинга

Повторюсь, хостинг это место на диске сервера хостинг-провайдера. По сути это тот же компьютер. Как вы понимаете, любой компьютер требует установки программного обеспечения.

[Читайте так же:  Как выбрать хостинг компанию: важные параметры хостинга](https://www.wordpress-abc.ru/hosting/kak-vyibrat-hosting-kompaniyu.html)

Программное обеспечение, устанавливается хостинг провайдером и по умолчанию предлагается клиентам хостинга, в разделе «Тарифы».

Для установки и работы WordPress 4.7.4 (последняя версия на 07-05-2017) , нужно выбрать хостинг со следующим программным обеспечением:

- PHP версии 7+
- MySQL версии 5.6+ или MariaDB версии 10.0+
- Протокол HTTPS
- Операционная система, подойдет и Linux и Windows;
- Сервер должен работать с  HTTP-сервером Apache (с включенным модулем mod_rewrite Apache) или с сервисом Nginx;
- Сервер должен быть доступен по протоколу FTP, через программу FTP клиент, установленную на вашем компьютере.

Сайт будет работать и на более старых, не поддерживаемых  версиях:

- Версия PHP 5.2.4;
- База данных MySQL старше версии 5.0;

, но в этом случае есть угроза безопасности сайта.

Вообще говоря, веб-приложение WordPress не прихотлива к программному обеспечению сервера. Без преувеличения можно сказать, что любой уважающий себя сервер, подойдет по программному обеспечению для установки WordPress.

## Параметры хостинга для сайта WordPress

### Оперативная память

Особое внимание, нужно уделить выбору, такого параметра сервера, как оперативная память. Она нужна для запуска скрипта по его вызову. Система WordPress, по-умолчанию, устроена так, что очень часто обращается к серверу при посещении пользователями. Чем больше будет посещение вашего блога, тем таких обращений будет больше. Поэтому, не выбирайте хостинг с низкой оперативной памятью 64 Mb. При среднем посещении WordPress на таких серверах «виснет» или «отрубается». Для WordPress ищите хостинг с заявленной оперативной памятью от 124 Mb, а лучше 256 Mb. Такие сервера сейчас не редкость и найти их просто.

### Трафик

Еще обратите внимание, на предлагаемый трафик хостинга. Выбирайте трафик ∞ (без ограничений).

### Цена

Про цену хостинга говорить не буду, выбор за вами, но замечу, что разумный хостинг для WordPress стоит от 160 рублей до 6 $ в месяц.

[Читайте так же:  Домен для WordPress сайта](https://www.wordpress-abc.ru/uroki-wordpress/domen-dlya-wordpress-3.html)

## Хостинг для wordpress: выбор хостинга и покупка домена

Большинство хостинг провайдеров предлагают зарегистрировать домен, с их помощью. Не рекомендую этого делать и поясню почему.

Покупая домен у провайдера, вы лишний раз привязываете себя к хостингу. А это не правильно. Не все хостинги, так хороши, как они себя рекламируют. Вы легко можете сменить сервер и перенести свой блог на другой хостинг, а вот если привязать свой домен к хостингу,  забрать с собой домен будет проблема. Её, конечно, тоже можно решить, только не понимаю, зачем создавать проблемы на ровном месте.

Лучше регистрацию домена, доверить специальной фирме, которая так и называется, регистратор доменных имен. Они аккредитованы в специальном центре и обычно без следа не исчезают. Если все-таки, регистратор закрывается, то он должен самостоятельно перенести ваши домены к генеральному регистратору доменных имен.

> Итак, хостинг для wordpress вы арендуете у понравившегося вам хостинг провайдера, а домен, у аккредитованного [регистратора доменных имен](https://www.wordpress-abc.ru/uroki-wordpress/domen-dlya-wordpress.html).

## Хостинг и DNS сервера

Домен должен быть обязательно привязан к [DNS серверам](https://www.wordpress-abc.ru/hosting/dns-hosting/kak-rabotaet-sistema-dns.html). Для своего домена можно использовать DNS сервера хостинга или сторонние DNS или DNS сервера регистратора имен. Принципиально разницы в выборе нет.

Чтобы привязать домен к DNS серверам хостинга, после покупки хостинга, узнайте адреса его DNS-серверов и зарегистрируйте их у регистратора имен. Для регистрации DNS серверов в панели регистратора ищите вкладку, управление DNS серверами и в поля NS сервера впишите адреса DNS серверов хостинга.

> Смена и регистрация DNS серверов происходит в течении 12-20 часов.

Если вы при покупке домена решили использовать сторонние DNS сервера, то сторонние DNS сервера нужно зарегистрировать (поменять) в административной панели сервера вашего хостинга.

[Читайте так же:  Чужой код в теме WordPress](https://www.wordpress-abc.ru/bezopasnost-wp/chuzhoy-kod-v-teme-wordpress.html)

### Итоги урока

Урок, Хостинг для WordPress – завершен. Теперь вы можете выбрать хостинг для своего блога WordPress, купить его и привязать домен к DNS-серверам.

### Полезные ссылки

- Apache http://httpd.apache.org/
- Nginx http://nginx.org/ru/
- https://ru.wordpress.org/about/requirements/ (требования к хостингу для WordPress).

©www.wordpress-abc.ru

### Другие Уроки WordPress

- [Первые настройки WordPress](https://www.wordpress-abc.ru/uroki-wordpress/pervyie-nastroyki-wordpress.html)
- [Как объединить два сайта WordPress](https://www.wordpress-abc.ru/uroki-wordpress/kak-obedinit-dva-sayta-wordpress.html)
- [Публикация статей в WordPress](https://www.wordpress-abc.ru/uroki-wordpress/publikatsiya-statey-v-wordpress.html)
- [Сайдбар и виджеты WordPress](https://www.wordpress-abc.ru/uroki-wordpress/saydbar-vidzhetyi-wordpress.html)
- [Установка и удаление плагина на WordPress](https://www.wordpress-abc.ru/uroki-wordpress/ustanovka-udalenie-plagina-na-wordpress.html)
- [Создаем меню WordPress: как создать меню WordPress](https://www.wordpress-abc.ru/uroki-wordpress/sozdaem-menyu-wordpress.html)
- [Настройки постоянных ссылок WordPress](https://www.wordpress-abc.ru/uroki-wordpress/nastroyki-postoyannyih-ssyilok-wordpress.html)
- [Домен для WordPress сайта](https://www.wordpress-abc.ru/uroki-wordpress/domen-dlya-wordpress-3.html)
- [Что такое тема WordPress](https://www.wordpress-abc.ru/uroki-wordpress/chto-takoe-tema-wordpress.html)
- [Создание базы данных для WordPress](https://www.wordpress-abc.ru/uroki-wordpress/sozdanie-bazyi-dannyih-dlya-wordpress.html)