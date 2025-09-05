<!DOCTYPE html>
<html lang="zh-TW">
<head>
<meta charset="UTF-8">
<title>線上抽獎轉盤</title>
<style>
  body { font-family: Arial, sans-serif; text-align: center; padding: 50px; background: #f0f8ff; }
  #nameInput { padding: 10px; font-size: 16px; }
  #spinButton { padding: 10px 20px; font-size: 16px; margin-left: 10px; cursor: pointer; }
  #wheelContainer { margin: 50px auto; width: 300px; height: 300px; position: relative; }
  #wheel { width: 100%; height: 100%; border-radius: 50%; border: 10px solid #333; position: relative; transition: transform 5s cubic-bezier(0.33, 1, 0.68, 1); }
  .slice { position: absolute; width: 50%; height: 50%; top: 50%; left: 50%; transform-origin: 0% 0%; background: #f1c40f; border: 1px solid #fff; line-height: 2; font-weight: bold; text-align: right; padding-right: 10px; box-sizing: border-box; }
  #pointer { width: 0; height: 0; border-left: 15px solid transparent; border-right: 15px solid transparent; border-bottom: 30px solid red; margin: -30px auto 0; }
  #result { font-size: 24px; font-weight: bold; margin-top: 20px; color: green; }
  #history { margin-top: 20px; text-align: left; max-width: 400px; margin-left: auto; margin-right: auto; }
</style>
</head>
<body>

<h1>🎉 線上抽獎轉盤 🎉</h1>
<input type="text" id="nameInput" placeholder="輸入你的姓名" />
<button id="spinButton">開始抽獎</button>

<div id="wheelContainer">
  <div id="wheel"></div>
  <div id="pointer"></div>
</div>

<div id="result"></div>
<div id="history"><strong>已抽過名單：</strong><ul id="historyList"></ul></div>

<script>
  const prizes = ["大獎", "二獎", "三獎", "四獎", "五獎", "安慰獎"];
  const wheel = document.getElementById('wheel');
  const resultDiv = document.getElementById('result');
  const historyList = document.getElementById('historyList');
  let participants = {}; // 用於記錄已抽過的人

  // 建立轉盤
  prizes.forEach((prize, i) => {
    const slice = document.createElement('div');
    slice.className = 'slice';
    slice.style.transform = `rotate(${i * (360 / prizes.length)}deg) skewY(-60deg)`;
    slice.style.background = `hsl(${i * (360 / prizes.length)}, 70%, 60%)`;
    slice.innerText = prize;
    wheel.appendChild(slice);
  });

  document.getElementById('spinButton').addEventListener('click', () => {
    const name = document.getElementById('nameInput').value.trim();
    if (!name) {
      alert("請輸入姓名！");
      return;
    }
    if (participants[name]) {
      alert(`${name} 已經抽過獎了！`);
      return;
    }

    // 隨機選擇獎項
    const prizeIndex = Math.floor(Math.random() * prizes.length);
    const spinDegrees = 360 * 5 + (prizeIndex * (360 / prizes.length)) + (360 / prizes.length / 2);
    wheel.style.transition = "transform 5s cubic-bezier(0.33, 1, 0.68, 1)";
    wheel.style.transform = `rotate(${spinDegrees}deg)`;

    // 顯示結果並更新已抽過名單
    setTimeout(() => {
      const prize = prizes[prizeIndex];
      resultDiv.innerText = `${name} 抽中了 ${prize} 🎉`;
      participants[name] = prize;

      // 更新已抽過名單
      const li = document.createElement('li');
      li.innerText = `${name} → ${prize}`;
      historyList.appendChild(li);
    }, 5000);
  });
</script>

</body>
</html># Lottery
