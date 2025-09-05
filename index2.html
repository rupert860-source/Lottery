<!DOCTYPE html>
<html lang="zh-Hant">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>婚禮幸運轉盤</title>
<style>
  body {
    font-family: 'Arial', sans-serif;
    text-align: center;
    padding: 50px;
    background: #fff0f5;
  }
  h1 {
    color: #d147a3;
    font-size: 36px;
  }
  #wheel-container {
    position: relative;
    width: 350px;
    height: 350px;
    margin: 20px auto;
  }
  #wheel {
    width: 100%;
    height: 100%;
    border-radius: 50%;
    border: 10px solid #d147a3;
    overflow: hidden;
    transition: transform 5s cubic-bezier(0.33, 1, 0.68, 1);
  }
  .segment {
    width: 50%;
    height: 50%;
    position: absolute;
    top: 50%;
    left: 50%;
    transform-origin: 0% 0%;
    text-align: right;
    padding-right: 10px;
    box-sizing: border-box;
    font-weight: bold;
    color: #fff;
  }
  #pointer {
    width: 0; 
    height: 0; 
    border-left: 15px solid transparent;
    border-right: 15px solid transparent;
    border-bottom: 30px solid #d147a3;
    position: absolute;
    top: -30px;
    left: 50%;
    transform: translateX(-50%);
  }
  #spinBtn, #joinBtn {
    padding: 12px 25px;
    font-size: 18px;
    background: #d147a3;
    color: white;
    border: none;
    cursor: pointer;
    border-radius: 8px;
    margin-top: 10px;
  }
  #winner {
    margin-top: 20px;
    font-size: 22px;
    color: #d147a3;
    font-weight: bold;
  }
  input {
    padding: 5px;
    font-size: 16px;
    margin-bottom: 10px;
  }
  #confetti-canvas {
    position: fixed;
    pointer-events: none;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 9999;
  }
</style>
</head>
<body>

<h1>婚禮幸運轉盤</h1>
<p>請輸入你的名字參加抽獎：</p>
<input type="text" id="playerName" placeholder="名字">
<button id="joinBtn">加入抽獎名單</button>

<div id="wheel-container">
  <div id="pointer"></div>
  <div id="wheel"></div>
</div>
<button id="spinBtn">轉動轉盤抽獎</button>

<div id="winner"></div>
<canvas id="confetti-canvas"></canvas>

<script>
  const wheel = document.getElementById('wheel');
  const spinBtn = document.getElementById('spinBtn');
  const joinBtn = document.getElementById('joinBtn');
  const playerNameInput = document.getElementById('playerName');
  const winnerDiv = document.getElementById('winner');
  const confettiCanvas = document.getElementById('confetti-canvas');
  const confettiCtx = confettiCanvas.getContext('2d');

  let players = [];
  let prizes = ["紅包", "婚禮小禮物", "紀念品", "甜點", "香水", "巧克力"];
  let segments = prizes.length;
  let colors = ["#FF6B6B", "#FFD93D", "#6BCB77", "#4D96FF", "#FF6FF0", "#FF9F1C"];

  // 調整 canvas 大小
  confettiCanvas.width = window.innerWidth;
  confettiCanvas.height = window.innerHeight;

  // 建立轉盤
  function createWheel() {
    wheel.innerHTML = '';
    for (let i = 0; i < segments; i++) {
      const segment = document.createElement('div');
      segment.className = 'segment';
      segment.style.transform = `rotate(${i * (360/segments)}deg) skewY(-60deg)`;
      segment.style.backgroundColor = colors[i % colors.length];
      segment.innerHTML = `<span style="position:absolute;top:50%;left:110%;transform:rotate(60deg);font-weight:bold;">${prizes[i]}</span>`;
      wheel.appendChild(segment);
    }
  }

  createWheel();

  // 加入抽獎名單
  joinBtn.addEventListener('click', () => {
    const name = playerNameInput.value.trim();
    if(name) {
      players.push(name);
      alert(`${name} 已加入抽獎名單！`);
      playerNameInput.value = '';
    } else {
      alert('請輸入名字！');
    }
  });

  // 音效
  const spinSound = new Audio('https://actions.google.com/sounds/v1/cartoon/wood_plank_flicks.ogg');
  const winSound = new Audio('https://actions.google.com/sounds/v1/cartoon/clang_and_wobble.ogg');

  // 轉盤抽獎
  spinBtn.addEventListener('click', () => {
    if(players.length === 0){
      alert('請先加入至少一位玩家！');
      return;
    }
    spinBtn.disabled = true;
    spinSound.play();
    
    const winnerIndex = Math.floor(Math.random() * segments);
    const winnerPlayer = players[Math.floor(Math.random() * players.length)];
    const degrees = 360 * 5 + winnerIndex * (360/segments);
    
    wheel.style.transform = `rotate(${degrees}deg)`;

    setTimeout(() => {
      winnerDiv.textContent = `恭喜 ${winnerPlayer} 獲得 ${prizes[winnerIndex]} 🎉`;
      winSound.play();
      launchConfetti();
      spinBtn.disabled = false;
    }, 5000);
  });

  // 簡單彩帶效果
  function launchConfetti() {
    let confetti = [];
    for (let i = 0; i < 150; i++) {
      confetti.push({
        x: Math.random() * confettiCanvas.width,
        y: Math.random() * confettiCanvas.height - confettiCanvas.height,
        r: Math.random() * 6 + 4,
        d: Math.random() * 20,
        color: colors[Math.floor(Math.random() * colors.length)],
        tilt: Math.random() * 10 - 10,
        tiltAngleIncremental: Math.random() * 0.07 + 0.05,
        tiltAngle: 0
      });
    }

    function draw() {
      confettiCtx.clearRect(0, 0, confettiCanvas.width, confettiCanvas.height);
      confetti.forEach((c) => {
        confettiCtx.beginPath();
        confettiCtx.lineWidth = c.r / 2;
        confettiCtx.strokeStyle = c.color;
        confettiCtx.moveTo(c.x + c.tilt + c.r / 4, c.y);
        confettiCtx.lineTo(c.x + c.tilt, c.y + c.tilt + c.r / 4);
        confettiCtx.stroke();
      });
      update();
    }

    function update() {
      confetti.forEach((c) => {
        c.tiltAngle += c.tiltAngleIncremental;
        c.y += (Math.cos(c.d) + 3 + c.r/2)/2;
        c.tilt = Math.sin(c.tiltAngle) * 15;

        if (c.y > confettiCanvas.height) {
          c.y = -10;
          c.x = Math.random() * confettiCanvas.width;
        }
      });
    }

    let animation = setInterval(draw, 20);
    setTimeout(() => clearInterval(animation), 5000);
  }
</script>

</body>
</html>
