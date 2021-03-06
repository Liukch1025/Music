# html5-audio-player

## 1. introduce
html5 audio player(with playlist) using flexbox, svg, css animations and  js api.

forked from @k-ivan at http://codepen.io/k-ivan/pen/pJMLmJ

demo: [html5-audio-player](https://likev.github.io/html5-audio-player/ 'html5-audio-player demo')

![html5-audio-player-screenshot](html5-audio-player.png)

## 2. how to use
1. insert Google Material Icons and AudioPlayer.css before `</head>`
2. insert AudioPlayer.js before `</body>`
3. use AP.init function

code example:
```html
<!DOCTYPE html>
<html >
  <head>
    <meta charset="UTF-8">
    <title>Audio player HTML5</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
    <link rel="stylesheet" href="css/AudioPlayer.css">
    <style>

    #player{
        position: relative;
        max-width: 700px;
        height: 500px;
        border: solid 1px gray;
    }
    </style>
  </head>

  <body>
      <!-- Audio player container-->
     <div id='player'></div>

    <!-- Audio player js begin-->
    <script src="js/AudioPlayer.js"></script>

    <script>
        // test image for web notifications
        var iconImage = null;

        AP.init({
            container:'#player',//a string containing one CSS selector
            volume   : 0.7,
            autoPlay : true,
            notification: false,
            playList: [
                {'icon': iconImage, 'title': '什麼都不要-許書豪', 'file': 'mp3/什麼都不要-許書豪.mp3'},
                {'icon': iconImage, 'title': '丢了你-井胧', 'file': 'mp3/丢了你-井胧.mp3'},
                {'icon': iconImage, 'title': '再見煙火-卓義峯 Yifeng Zhuo', 'file': 'mp3/再見煙火-卓義峯 Yifeng Zhuo.mp3'},
                {'icon': iconImage, 'title': '在沒有你以後-謝和弦 Rchord張智成 ZChen', 'file': 'mp3/在沒有你以後-謝和弦 Rchord張智成 ZChen.mp3'},
                {'icon': iconImage, 'title': '如果可以-韋禮安', 'file': 'mp3/如果可以-韋禮安.mp3'},
                {'icon': iconImage, 'title': '我的事不關你的事-賴慈泓 ft 孫盛希 Shi Shi', 'file': 'mp3/我的事不關你的事-賴慈泓 ft 孫盛希 Shi Shi.mp3'},
                {'icon': iconImage, 'title': '我很好騙-動力火車', 'file': 'mp3/我很好騙-動力火車.mp3'},
                {'icon': iconImage, 'title': '那不是雪中紅-JPM', 'file': 'mp3/那不是雪中紅-JPM.mp3'},
                {'icon': iconImage, 'title': '咖啡-張學友', 'file': 'mp3/咖啡-張學友.mp3'},
                {'icon': iconImage, 'title': '忽然-韋禮安', 'file': 'mp3/忽然-韋禮安.mp3'},
                {'icon': iconImage, 'title': '林中鳥-葛林', 'file': 'mp3/林中鳥-葛林.mp3'},
                {'icon': iconImage, 'title': '勇氣-棉子', 'file': 'mp3/勇氣-棉子.mp3'},
                {'icon': iconImage, 'title': '飛鳥和蟬-任然', 'file': 'mp3/飛鳥和蟬-任然.mp3'},
                {'icon': iconImage, 'title': '嘉賓-張遠', 'file': 'mp3/嘉賓-張遠.mp3'},                
                {'icon': iconImage, 'title': '斷訊-邱鋒澤FENG ZE X SpeXial偉晉 Wayne', 'file': 'mp3/斷訊-邱鋒澤FENG ZE X SpeXial偉晉 Wayne.mp3'}
          ]
        });
    </script>
    <!-- Audio player js end-->

  </body>
</html>
```

it will work!
