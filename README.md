<script>
  const trigger = document.getElementById("secretTrigger");
  const container = document.getElementById("emma-message");

  let started = false; // 二重防止

  function startMessage(e) {
    e.preventDefault();
    if (started) return;
    started = true;

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
</script>
