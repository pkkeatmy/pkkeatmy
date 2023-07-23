# pkkeatmy
<!DOCTYPE html>
<html>
<head>
  <title>Han & Faith E Invitation</title>
  <style>
    body {
      overflow: hidden;
      margin: 0;
      padding: 0;
    }

    img {
      width: 100%;
      height: auto;
      animation: slideDown 35s linear infinite;
    }

    @keyframes slideDown {
      0% {
        transform: translateY(0);
      }
      100% {
        transform: translateY(-100%);
      }
    }
  </style>
</head>
<body>
  <img src="Artboard 12.jpg" alt="自动播放图片" />
  <audio id="audio" controls autoplay>
    <source src="FAITH WEDDING.mp3" type="audio/mpeg">
  
  </audio>

  <script>
    var audioElement = document.getElementById("audio");
    var isScrolling;

    // 监听滚动事件，当用户滚动页面时暂停音乐
    window.addEventListener("scroll", function() {
      audioElement.pause();
      clearTimeout(isScrolling);
      isScrolling = setTimeout(function() {
        audioElement.play();
      }, 100);
    });
  </script>
</body>
</html>
