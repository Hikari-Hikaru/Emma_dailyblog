<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <title>2025年4月5日 - </title>
  <link rel="stylesheet" href="../style.css">

  <style>
    body {
      background-color: #ffe4e1;
      font-family: "Helvetica Neue", sans-serif;
      color: #333;
    }

    header {
      text-align: center;
      margin-top: 40px;
    }

    header h1 {
      font-family: 'Courier New', Courier, monospace;
      font-size: 2.5em;
      color: #ff69b4;
      letter-spacing: 0.1em;
      text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
    }

    header h2 {
      font-size: 0.9em;
      color: #999;
      margin-top: -10px;
    }

    .secret-link {
      color: #ffe4e1;
      text-decoration: none;
      cursor: pointer;
      animation: blink 1.2s infinite;
    }

    .secret-link:hover {
      color: red;
    }

    @keyframes blink {
      0%, 100% { color: #ffe4e1; }
      50% { color: #ff69b4; }
    }

    #emma-message {
      margin-top: 40px;
      text-align: center;
    }

    .letter {
      font-size: 1.5em;
      color: #cc0000;
      opacity: 0;
      transform: translateY(-20px) rotate(0deg);
      animation: glitchDrop 0.8s ease-in-out forwards;
      margin: 5px 0;
    }

    .letter:last-child {
      color: red;
      font-weight: bold;
      font-size: 1.8em;
    }

    @keyframes glitchDrop {
      0% {
        opacity: 0;
        transform: translateY(-20px) rotate(0deg);
      }
      50% {
        opacity: 1;
        transform: translateY(5px) rotate(10deg);
      }
      100% {
        transform: translateY(0px) rotate(-2deg);
      }
    }
  </style>
</head>

<body>
  <header>
    <h1>2025_04_05</h1>
    <h2>
      <a href="#" id="secretTrigger" class="secret-link">
        Not everything is what it seems.
      </a>
    </h2>
  </header>

  <main>
    <p style="text-align:center;">
      Today was the entrance ceremony for high school.<br>
      I was born in Japan, but since my parents grew up in U.S.A.,<br><br>
      I stood out in a strange way from the perspective of Japanese people,<br>
      and it was a bit embarrassing.
    </p>

    <!-- ダイイングメッセージ表示 -->
    <div id="emma-message"></div>
  </main>

  <!-- ▼ ブログ一覧 -->
  <h2>ブログ一覧</h2>
  <ul>
    <li><a href="https://hikari-hikaru.github.io/Emma_dailyblog_2/">（dairy2ページ）</a></li>
    <li><a href="https://hikari-hikaru.github.io/Emma-s_dailyblog_3/">（dairy3ページ）</a></li>
    <li><a href="https://hikari-hikaru.github.io/Emma-s_dailyblog_4/">（dairy4ページ）</a></li>
    <li><a href="https://hikari-hikaru.github.io/Emma-s_dailyblog_5/">（dairy5ページ）</a></li>
    <li><a href="https://hikari-hikaru.github.io/Emma-s_dailyblog_6/">（dairy6ページ）</a></li>
    <li><a href="https://hikari-hikaru.github.io/Emma-s_dailyblog_7/">（dairy7ページ）</a></li>
    <li><a href="https://hikari-hikaru.github.io/Emma-s_dailyblog_8/">（dairy8ページ）</a></li>
  </ul>

  <script>
    const trigger = document.getElementById("secretTrigger");
    const container = document.getElementById("emma-message");

    function startMessage(e) {
      e.preventDefault();

      if (container.childElementCount > 0) return;

      const messages = [
        "もしこれを読んでいるなら",
        "私はもういない",
        "これは日記じゃない",
        "お願い、最後まで読んで",
        "最初は違和感だった",
        "でも気のせいじゃなかった",
        "見られてる",
        "ずっと",
        "逃げられなかった",
        "このブログも安全じゃない",
        "お願い",
        "戻って",
        "関わらないで",
        "次は",
        "あなた"
      ];

      messages.forEach((text, index) => {
        setTimeout(() => {
          const p = document.createElement("div");
          p.className = "letter";
          p.textContent = text;
          container.appendChild(p);
        }, index * 400);
      });

      setTimeout(() => {
        window.location.href = "https://hikari-hikaru.github.io/thanks/";
      }, messages.length * 400 + 1500);
    }

    trigger.addEventListener("click", startMessage);
    trigger.addEventListener("touchstart", startMessage);
  </script>
  <script> setTimeout(() => { window.location.href = "https://hikari-hikaru.github.io/Emma_dailyblog/"; }, 60000); // 60000ms = 1分 </script>
</body>
</html>
