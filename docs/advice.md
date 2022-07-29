# Советы

## Общие советы
**Будьте внимательны — и не придется переделывать.**

Проверяйте, что текст без грамм. ошибок, что все в порядки с пунктуаци-
ей; перед монтажем проверьте в измененных фрагментах, что все аккуратно;
после монтажа также проверьте эти места.

Измененных мест, обычно, не более 5, и это занимает 2-3 минуты, но может
сэкономить как ваше время на перерендеринг, так и время проверяющего.

**Особое внимание**: проверьте, что не забыли замьютить англ. аудио дорожку.

## Основные методы перевода текста.

- *Наложить текст с непрозрачным бекграундом.*  
   Подходит для ситуации, когда фон в месте, где размещен текст одноцветен,
   но обычно это не так, и лучше использовать другие методы.
- *Наложить gaussian blur на место где находится текст, и добавить
свой поверх.*  
    - Универсальный способ, подходит для динамического бекграунда, и,
обычно, смотрится неплохо.
    - Ниже пример, где лучше было использовать `blur`.
    <figure markdown>
     ![image title](https://github.com/AlexFreik/isha-montage/blob/master/docs/img/title_blur_bad.jpg?raw=true){ width="300" }
     <figcaption>Not nice...</figcaption>
    </figure>
    <figure markdown>
     ![image title](https://github.com/AlexFreik/isha-montage/blob/master/docs/img/title_blur.jpg?raw=true){ width="300" }
     <figcaption>Nice!</figcaption>
    </figure>
    - Если фон сливается с переведенным текстом, или `blurred` английскй
       текст добавляет слишком много белого / черного на фон, то можно
       добавить полупрозрачный бекграунд на переведенный текст.

- *Зафиксировать кадр, когда английский текст еще не появился.*
    - Подходит в случае статической картинки на бэкграунде. Если на
       заднике красивая анимация — `blur` предпочтительнее.
    - Если в оригинале естть zoom (динамическое увеличение 
       статической картинки) для добавления динамики, то нужно 
       добавить `zoom` и при переводе.  
   P.S. В обучающих материалах есть видео-пример этого способа.
- *Перевод сбоку.*  
   Иногда, когда анимация особенно сложная, или не хватает времени на блюр,   или так просто будет лучше смотреться, можно поставить перевод рядом.  
   **Note**: мы редко используем этот способ.
    <figure markdown>
     ![image title](https://github.com/AlexFreik/isha-montage/blob/master/docs/img/text_below_example.jpg?raw=true){ width="300" }
    </figure>
- *Если есть stem (видео без английского текста).*  
   В данном случае действуем так: скачиваем и оригинал с текстом, и стем.
   Добавляем их один поверх другого, и монтируем. В конце можно просто
   отключить (сделать невидимым) трек с английским текстом.  
   Для заголовков, субтитров и т.д. стараемся, по возможности, выбирать
   красивые эффекты вместо просто эффекта `Text`.

## Видео с кучей (> 20) субтитров
В таком случае — выбирайте тщательность монтажа, основываясь на 
доступном времени. Монтаж, вероятно, займет не менее 3-х часов.

Совет — надписи, вроде «ISHA VIDHYA» или «GREEN HANDS PROJECT»,
допустимо оставить как есть, поскольку переводы «ИША ВИДХЬЯ» или
«ПРОЕКТ ГРИНХЕНДС» не представляют особой важности.

Так же, возможно, будет проще использовать блюр пореже, поскольку это 
отнимает больше времени, чем текст с непрозрачным бекграундом
или перевод сбоку.

## Как скачать видео
Чтобы скачать видео с YouTube можно воспользоваться сайтом https://www.y2mate.com/,
скопировав и вставив ссылку на видео.
Также, если видео уже открыто в браузере можно просто вставить "pp" после
слова youtube в ссылке, и y2mate откроется автоматически.

Например, `https://www.youtube.com/watch?v=Oi7eLmaL1DU` нужно 
преобразовать в `https://www.youtubepp.com/watch?v=Oi7eLmaL1DU`

**Note**: если с этим сайтом не получается, есть множество других:

- [https://loader.to/en102/1080p-video-downloader.html](https://loader.to/en102/1080p-video-downloader.html)
- [https://en.savefrom.net/1-youtube-video-downloader-200/](https://en.savefrom.net/1-youtube-video-downloader-200/)

Единственно, некоторые сайты иногда не предлагают опцию `1080`
(а только `720`), не смотря на то, что `1080` доступно на YouTube
для этого видео. Поэтому нужна внимательность.

## Где монтировать
В Isha Foundation в основном используются Final Cut и Adobe Premiere Pro,
однако вы можете, использовать любой удобный для вас редактор.

Например, DaVinci Resolve — профессиональный видеоредактор с бесплатной
версией, которой нам более чем хватает.

Для пользователей MacOS самый простой вариант монтирующей системы —
iMovie, но у нее есть пара серьезных недостатков.

- Нет возможности удобно добавить текст поверх видео. То есть, придется
   делать картинку с перевдодм в отдельном приложении и наклеивать
   поверх. Это нарушает поток, и нужно будет повозиться, если придется
   исправлять текст.
- Можно использовать только два видео трека. Это ограничивает более
   сложный монтаж, хотя обычно двух хватает.

Поэтому совет — скачать более профессиональное приложение, тем более что
DaVinci бесплатный =).