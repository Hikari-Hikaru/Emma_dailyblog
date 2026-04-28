<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <title>thanks</title>

  <style>
    body {
      background-color: #000;
      color: #fff;
      font-family: "Courier New", monospace;
      padding: 40px;
      line-height: 1.8;
      opacity: 1;
    }

    h1 {
      color: #1e90ff;
      border-bottom: 1px solid #444;
      padding-bottom: 10px;
    }

    .main-text {
      font-size: 1.3em;
      margin-top: 20px;
      font-weight: bold;
    }

    .sub-text {
      margin-top: 30px;
      color: #ccc;
    }

    .fade-warning {
      margin-top: 30px;
      color: #777;
      font-size: 0.9em;
    }
  </style>
</head>

<body>

<h1>thanks</h1>

<p class="main-text">……ここまで読んでくれてありがとう。</p>

<p class="sub-text">
でも、もう遅いよね。<br>
あのとき、わたしは気づいてた。<br>
誰が、わたしを……。<br><br>

お願い。もしこれを見つけてくれたなら、<br>
わたしがなぜ、こんな最後を迎えたのかを知ってほしい。<br>
そして、〇〇〇を…。
</p>

<p class="fade-warning">（このページはすぐに閉じるかもしれない）</p>

<script>
  // 58秒後にフェードアウト開始
  setTimeout(() => {
    document.body.style.transition = "opacity 2s";
    document.body.style.opacity = "0";

    // フェード後に元のブログへ戻る
    setTimeout(() => {
      window.location.href = "https://hikari-hikaru.github.io/Emma_dailyblog/";
    }, 2000);
  }, 58000);
</script>

</body>
</html>
