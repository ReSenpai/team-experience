
FSD step 1 - 2 team experience

https://resenpai.github.io/team-experience/  - github pages

Давайте сразу определимся, каждый работает в своей ветке и называет ее именем модуля, над которым работает + имя или никнейм.
Не бойтесь делать частые коммиты.
После того, как вы сделаете часть модуля, заливайте его в develop ветку с пометкой версии модуля.

Так же старайтесь писать классы по БЭМ. ( https://ru.bem.info/methodology/quick-start/ )
Если пишите CSS или HTML препроцессорами, то заливайте и препроцессорный вариант тоже, очень интересно.

Будем разрабатывать Landing page , например посмотрите как зверстан этот сайт https://one-page-site.ru/#portfolio или https://slumber.fm/
Все стили подключаем импортом в индекс (можете отдельно писать свои файлики стилей если так удобнее).
Шрифты, иконки и прочие метаданные - в метаданные. Так же все по папкам раскидывайте, что бы было понятно. 
Картинки в картинки, шрифты в шрифты и тд. Если нужной папки нет - создайте). Но шрифты лучше искать в гугл фонтс и подключать удаленно.

Так же на этот макет заведен github pages
по адресу ( https://resenpai.github.io/team-experience/ ).
Он подцепляет версию сайта с ветки мастер.


Эмулируем такую ситуацию, когда заказчик сам не знает, чего хочет, у него нет макета, но есть куча хотелок.
Я так же напишу пресеты цветов, шрифтов и прочего в отдельный файлик css(или уже написал).

            -------------------Тех задание------------------
            
            
            
 Заказчик хочет сайт one page site он же Landing page с рекламной его продукта, описанием компании и прочее. 
 У заказчика довольно необычная компания по продаже дизайнерских игральных карт для фокусов и покера.
 
 Общая концепция: Придерживайтесь тонов и шрифтов в пресетах. Можете свои переменные стилей назначать,
 только пожалуйста раскоментите там свой отдел, что бы было понятно, куда идут эти переменные.
 Вы всегда можете посмотреть текущее состоянии полной страницы в develop/master или на github pages .

                       -----------Моуди-------

Описание модулей фривольное и содержит множество неточностей, прошу меня простить заранее.
Но зато дает какой то общий концепт работы. Далее по ходу верстки это все скорее всего
будет правиться и расширяться, уточнятся. Если хотите внести какие то изменения в модули,
добавить новые, изменить и уточнить имеющиеся, то заходите в request, меняйте содержимое тех задания и создавайте коммит об этом, затем обратно идите на свою ветку. Таким образом у нас будет отдельная ветка со всеми версиями ТЗ.
                       
                       
                        1. Шапка сайта. 

В шапке будут ссылки на каждый модуль в сайте. При нажатии на них страничка должна скроллится до нужного участка. 
Шапка должна быть фикисрованной и хорошо смотрется при скролле. Так же нужно разработать лого и поместить его в шпаку так,
что бы это смотрелось уместно. Можете использовать лого креаторы по типу (https://www.namecheap.com/logo-maker/app/new). 
Название фирмы заказчик "Face card". Работа творческая, лучше сразу сделайте несколько логотипов и примеряйте к готовому дизайну.

  
 
                        2. Модуль с описанием компании.
                        
Сюда нужно поместить блок с описанием компании. Заказчик хочет, что бы на фоне играла гифка или видео(без звука) на весь экран или в большом блоке, скажем 90vh на 75-90vw. Желательно все спрятать за 
полупрозрачный цветной фильтр. При скролле гифка или видео должна быть фикисрованна относительно
видимой части экрана, а все остальные элементы должны двигатся по ней. Таким образом следующий
модуль просто перекроет собой это видео или гифку. Если не сможете вставить видео\ гифку, то сделайте
то же самое с картинкой. Так же в отделе должнен быть текст с названием компании, описанием приемуществ
работы с данной компанией и прочие кричащие фразочки, но не перебарщивайте.
 
                        3. Модуль с описанием товаров.

Тут у нас будет некий небольшой каталог игральных карт. Можете сделать по отделам или что бы каталог
динамический менялся. Главное сделать какие нибудь красивые ховер эффекты при наведение на фото товара
и что бы все это сочиталось с текстом товара, в котором будет название, краткое описание и цена и прочее, что сочтете нужным, но не советую много текста там писать. Только самое важное. Далее, если вы 
сможете, тот тут можно сделать отдельную выезжающую панельку с товаром при нажатии на фотографию, где вы
уже сможете на полную развернутся в его описании и рекламе, добавить больше фоток и тд. Это все делается
через js, можно создать под это дело отдельный объект с каталогом товаров и динамически подгружать по 
id товаров, на который в данным момен нажал пользователь.
 
                        4. Модуль с отзывами

Далее модуль с отзывами о товаре. Тут хотелось бы увидеть реализацию такой схемы: Динамические отзывы, которые менятся каждые 5 секунд, как будто лента сообщений подгружается. При этом верхнее сообщение уходит, а нижнее новое двигает все отслаьные на верх. Если сможете такое реализовать - круто. Если нет, 
то просто сделайте классические примеры с отзывами как на любых других сайтах по вашему усмотрению. В 
качестве фото, имен и текста отзывов - можете использовать что хотите - все равно этот проект для обучения).
 
                        5. Модуль с контактами

В модуле с контактами нужно реализовать адреса какого нибудь физического магазина данной компании.
Если сможете прикрутить виджет яндекс карты - то будет супер. Так же поместите сюда кликабельные иконки
на соцсети (чем больше, тем лучше). И прочие контактные данные, почту, телефоны и тд. Только ненадо
реальные контаткные данные тут выкладывать)) Иконки под соцсети можно найти в интернет, например на:
https://fontawesome.com/

                        6. Подвал.

Так как у нас фиксированная шапка, тут не нужно дублировать ссылки. Достаточно просто выставить копирайт
по названию компании. Добавить несколько ссылок на скачку документов, типо реквизитов или прайсов.
Просто копируйте первые попавшиеся шаблоны в интернете. Понимаю, что этот модуль скудный, относительно
других, поэтому можно прикрутить сюда еще вызжающие блоки с анкетами. Например сделать пару анкет:
1) Оставить отзыв на товар, с разными вопросами и вариантами ответа, используйе по максимум возможности input .
2) Анкета с вакансиями в эту фирму, так же с выбором профессии и прочие нужные штуки для
быстрого составления резюме. Можете делать обе анкеты, можете взять одну на выбор, ваше право)
