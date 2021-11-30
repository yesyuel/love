<!DOCTYPE html>
<html lang="zh-CN">

<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
    <meta name="renderer" content="webkit">
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no" />
    <title>张逸赫♡</title>
    <style>
        body {
            -webkit-font-smoothing: antialiased;
            font-family: Helvetica Neue, Helvetica, Hiragino Sans GB, Microsoft YaHei, Arial, sans-serif;
            
            font-size: 85%;
            margin: 0;
        }
        
        h2 {
            font-size: 220%;
            font-weight: 400;
        }
        
        .content {
            position: absolute;
            width: 100%;
            top: 40%;
            transform: translate(0, -50%);
            text-align: center;
        }
        
        .timer {
            font-size: 180%;
            line-height: 1.5;
            margin: 1em 0;
        }
        
        .timer b {
            color: rgb(253, 99, 125);
        }
    </style>
</head>

<body background="C:\oc\ba.jpg" style=" background-repeat:no-repeat ;background-size:100% 100%;
background-attachment: fixed;">
    <div class="content">
        <h2 style="color: lightseagreen;">张逸赫</h2>
		<h2 style="color: rgb(24, 5, 92);">&</h2>
		<h2 >***</h2>
		<h2 style="color: rgb(182, 69, 98);">已经热恋了</h2>
        <div class="timer">
            <b id="d"></b> <b style="color: rgb(191, 207, 44);">天 </b><b id="h"></b> <b style="color: rgb(191, 207, 44);">时 </b> <b id="m"></b> <b style="color: rgb(191, 207, 44);">分 </b> <b id="s"></b> <b style="color: rgb(191, 207, 44);">秒 </b>
        </div>
    </div>

    <script>
        function timer() {
            var start = new Date(2021, 10, 30); // 2015.7.2
            var t = new Date() - start;
            var h = ~~(t / 1000 / 60 / 60 % 24);
            if (h < 10) {
                h = "0" + h;
            }
            var m = ~~(t / 1000 / 60 % 60);
            if (m < 10) {
                m = "0" + m;
            }

            var s = ~~(t / 1000 % 60);
            if (s < 10) {
                s = "0" + s;
            }
            document.getElementById('d').innerHTML = ~~(t / 1000 / 60 / 60 / 24);
            document.getElementById('h').innerHTML = h;
            document.getElementById('m').innerHTML = m;
            document.getElementById('s').innerHTML = s;
        }
        timer();
        setInterval(timer, 1000);
    </script>
</body>

</html>
