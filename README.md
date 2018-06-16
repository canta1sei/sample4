# sample4
test2
<!doctype html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<meta http-equiv="x-ua-compatible" content="IE=edge">
<title>4-03_digit</title>
<link href="../../_common/css/style.css" rel="stylesheet" type="text/css">
</head>
<body>
<header>
<div class="header-contents">
<h1>桁数を合わせる</h1>
<h2>ファンクションの作成</h2>
</div><!-- /.header-contents -->
</header>
<div class="main-wrapper">
<section>
	<h2>BESTアルバムDisc3収録曲</h2>
    <div id = 'list'>
    </div>
</section>
</div><!-- /.main-wrapper -->
<footer>JavaScript Samples</footer>
    <script>
        var addzoro = function(num,digit){
        var numString = String(num);
            while(numString.length<digit){
                numString='0'+numString;
            }
            return numString;
      }
var songs = [
    'CONTORADICTION',
    '走れ！',
    '白い風',
    'コノウタ',
    '全力少女',
    '黒い週末',
    '仮想ディストピア',
    'Link Link',
    '桃色空',
    'DNA狂詩曲'
    ];
for(var i=0;i<songs.length;i++){
    var paragraph = document.createElement('p');
    paragraph.textContent = addzoro(i+1,2)+'. '+songs[i];
    document.getElementById('list').appendChild(paragraph);
}
        
    </script>
</body>
</html>
