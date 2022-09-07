# Обучающие материалы

Монтировать совсем не сложно! В начале будет немножко трудно, но основы
можно освоить за пару часов. Главное — не бояться, и спрашивать, если что-то
не понятно.
Так же, Google — ценный помошник, особенно, если гуглить на английском.

Например, запросы, вроде "DaVinci how to add frame hold" 
("DaVinci как зафиксировать фрейм видео") должны помочь.

Ниже real-life примеров монтажа, можете ознакомится с ними!

- Подробное видео-пример монтажа видео в DaVinci. (Пример для ролика 
   с YouTube, но, в Instagram примерно те-же задачи)  
   DaVinci exmple: — [https://youtu.be/SAceoBqdAvw](https://youtu.be/SAceoBqdAvw)
- Короткое видео о том, как фиксировать фрейм и добавить zoom.  
   DaVinci Frame Freez example: — [https://youtu.be/caPaZ5syTC8](https://youtu.be/caPaZ5syTC8)
- Короткий туториал о том что делать со старыми "квадратными"видео.  
   DaVinci Narrow Video Tutorial: — [https://youtu.be/FGdErSdSOAI](https://youtu.be/FGdErSdSOAI)
- Три двух-минутных ролика монтажа для Instagram в Premiere Pro.  
   Premiere short examples:  
    - [https://youtu.be/AWOsM9fX9RQ](https://youtu.be/AWOsM9fX9RQ)
    - [https://youtu.be/lvRnpvTXHis](https://youtu.be/lvRnpvTXHis)
    - [https://youtu.be/Ontq3mMD9AM](https://youtu.be/Ontq3mMD9AM)

- Подробное обучающее видео-пример монтожа квадрата в DaVinci для соцсетей.  
   DaVinci Square Example: - [https://youtu.be/WGUWebrpf2o](https://youtu.be/WGUWebrpf2o)

<!-- <iframe -->
<!--     id="ytplayer" -->
<!--     type="text/html" -->
<!--     width="640" -->
<!--     height="360" -->
<!--     src="https://www.youtube-nocookie.com/embed/N4Keb583jf0" -->
<!--      frameborder="0"></iframe> -->

<div id="ytplayer"></div>

<script>
  // Load the IFrame Player API code asynchronously.
  var tag = document.createElement('script');
  tag.src = "https://www.youtube.com/player_api";
  var firstScriptTag = document.getElementsByTagName('script')[0];
  firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);

  // Replace the 'ytplayer' element with an <iframe> and
  // YouTube player after the API code downloads.
  var player;
  function onYouTubePlayerAPIReady() {
    player = new YT.Player('ytplayer', {
      height: '360',
      width: '640',
      videoId: 'WGUWebrpf2o'
    });
  }
</script>
