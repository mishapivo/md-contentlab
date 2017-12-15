# Точная настройка показателя отказов Google Analytics

[Главная](https://www.wordpress-abc.ru/) » [SEO оптимизация Wordpress](https://www.wordpress-abc.ru/seo-wordpress) » Точная настройка показателя отказов Google Analytics

![настройка показателя отказов Google Analytics](https://www.wordpress-abc.ru/wp-content/uploads/2017/05/obzor-auditorii---Google-Analytics-pokazatel-otkazov.png)

Содержание

- [Вступление](https://www.wordpress-abc.ru/seo-wordpress/tochnaya-nastroyka-pokazatelya-otkazov-google-analytics.html#i)
- [Google Analytics и показатель отказов](https://www.wordpress-abc.ru/seo-wordpress/tochnaya-nastroyka-pokazatelya-otkazov-google-analytics.html#Google_Analytics)
- [Нормальный показатель отказов](https://www.wordpress-abc.ru/seo-wordpress/tochnaya-nastroyka-pokazatelya-otkazov-google-analytics.html#i-2)
- [Эксперимент](https://www.wordpress-abc.ru/seo-wordpress/tochnaya-nastroyka-pokazatelya-otkazov-google-analytics.html#i-3)
- Причина высокого показателя отказов
  - [Еще статьи](https://www.wordpress-abc.ru/seo-wordpress/tochnaya-nastroyka-pokazatelya-otkazov-google-analytics.html#i-5)

## Вступление

Не знаю, как вас, а меня раздражает показатель отказов Google Analytics. По определению, показатель отказов Google Analytic считает отказом такое посещение сайта, при котором посетитель остается на странице входа (не взаимодействует со страницей).

## Google Analytics и показатель отказов

Google Analytics не учитывает пассивные действия пользователя на странице. То есть не считывает движения мыши, которые могут означать, что страница читается. Так же GA не учитывает время пребывания на странице. Если перехода со страницы не было, это отказ, а время пребывания считается равным нулю.

> Система вычисляет показатель отказов как долю отказов от общего числа сеансов путем деления кол-ва сеансов с просмотром одной страницы на общее число сеансов.

Утверждать, что высокий показатель отказов, свидетельствует о плохом качестве сайта, неправильно. Вполне вероятно, что большая часть «отказников», зашли на сайт, нашли нужную информацию и довольные ушли с сайта.

Другое дело, что наблюдается высокий показатель отказов на специально созданной навигационной странице сайта. Например, вы создали главную страницу с описанием сайта и большим количеством ссылок, предполагая, что посетитель будет переходить по ним. Высокий показатель отказов на таких страницах это, безусловно, плохо.

## Нормальный показатель отказов

Есть мнения, и они вполне разумны, что нормальный показатель отказов должен быть разным для сайтов разной тематики:

- Для интернет магазина: 20-40%;
- Сайт услуг: 10-30%;
- Лейдинг-пейдж: 70-90%;
- Информационный сайт, блог: 80-90%.

Я считаю, что эти цифры не имеют никакого отношения к реальному положению дел. Поясню. Что значит, по Google Analytics, показатель отказа 80%. Это значит, что 8 человек из 10, зайдя на ваш блог (сайт) не воспользовались навигацией по сайту, а удовлетворились открытой страницей. Плохо это? Очевидно, такое поведение не плохо, если пользователь просидел на сайте протяженное время. И также очевидно, это плохо, если средний показатель «время на сайте» ничтожно мала (близок к нескольким секундам).

> Яндекс метрика считает показатель отказа по другому и именно поэтому, видим заметную разницу в показателях отказа Google Analytics и Яндекс.Метрика.

## Эксперимент

Для проверки выше изложенного, проведу эксперимент. Начало 24-03-2107. Меняю стандартный код отслеживания Google Analytics на сайте. На начало эксперимента, показатель отказа 84%.

[Читайте так же:  Как снять фильтр АГС: сайт под фильтром Яндекс](https://www.wordpress-abc.ru/seo-wordpress/kak-snyat-filtr-ags.html)

Дополняю стандартный скрипт счетчика дополнительным условием.

```
&lt;script&gt;

(function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){

(i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),

m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)

})(window,document,'script','https://www.google-analytics.com/analytics.js','ga');

ga('create', 'UA-xxxxxxxx-x', 'auto');

ga('send', 'pageview');

<strong>/* Точный показатель отказов по времени */</strong>

if (!document.referrer ||

document.referrer.split('/')[2].indexOf(location.hostname) != 0)

setTimeout(function(){

ga('send', 'event', 'Новый посетитель', location.pathname);

}, 15000);

&lt;/script&gt;
```

[![редакция кода счетчика Google Analytics](https://www.wordpress-abc.ru/wp-content/uploads/2017/05/pokazatel-otkazov-google-analytics-screen2.png)](https://www.wordpress-abc.ru/wp-content/uploads/2017/05/pokazatel-otkazov-google-analytics-screen2.png)Точная настройка показателя отказов Google Analytics

Вижу, что показатель отказа снизился на следующий день до 23% и держится в пределах 10-12%.

[![результаты точной настройки Google Analytics](https://www.wordpress-abc.ru/wp-content/uploads/2017/05/pokazatel-otkazov-google-analytics-screen1.png)](https://www.wordpress-abc.ru/wp-content/uploads/2017/05/pokazatel-otkazov-google-analytics-screen1.png)результаты настройка показателя отказов Google Analytics

> Настройка показателя отказов Google Analytics не всегда помогает и вполне возможно, что дело не в счетчике и на самом деле, пользователи «бегут с вашего сайта» по объективным причинам. Что делать и в чём причина?

## Причина высокого показателя отказов

Неадекватно высокий показатель отказов говорит, что на сайте есть серьезные проблемы. Здесь самые известные из них:

- Дизайн сайт переполнен яркими красками, много мигающих блоков, плохих картинок и т.д.;
- Много навязчивой всплывающей рекламы;
- Навигация по сайту запутана и не понятна;
- Открытая страница не соответствует запросу пользователя;
- Страница сайта долго загружается.

В этом случае работа предстоит более серьезная.

©www.wordpress-abc.ru

### Еще статьи

- [Как ускорить загрузку JS скриптов, CSS и HTML сайта WordPress: плагин Autoptimize](https://www.wordpress-abc.ru/plaginy/kak-uskorit-zagruzku-js-skriptov-css-i-html-sayta-wordpress-plagin-autoptimize.html)
- [Оптимизация изображений WordPress](https://www.wordpress-abc.ru/seo-wordpress/optimizatsiya-izobrazheniy-wordpress.html)
- [Как снять фильтр АГС: сайт под фильтром Яндекс](https://www.wordpress-abc.ru/seo-wordpress/kak-snyat-filtr-ags.html)
- [Группировка материалов по меткам WordPress: дополнительная навигация по сайту, как вывести метки списком](https://www.wordpress-abc.ru/seo-wordpress/gruppirovka-materialov-po-metkam-wordpress.html)
- [Как разделить анонс и цитату  в шаблоне WordPress](https://www.wordpress-abc.ru/seo-wordpress/kak-razdelit-anons-i-tsitatu-v-shablone-wordpress.html)