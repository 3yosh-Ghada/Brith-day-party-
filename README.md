<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>عيد ميلاد غادة 3D</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="style.css">
</head>
<body>

<div id="ui">
  <h2>🎮 لعبة عيد ميلاد غادة</h2>

  <select id="carSelect">
    <option value="red">🚗 سيارة حمراء</option>
    <option value="blue">🚙 سيارة زرقاء</option>
    <option value="pink">🚕 سيارة وردية</option>
  </select>

  <select id="dressSelect">
    <option value="pink">👗 فستان وردي</option>
    <option value="purple">👗 فستان بنفسجي</option>
    <option value="blue">👗 فستان أزرق</option>
  </select>

  <button id="startGame">▶️ ابدأ اللعب</button>

  <div class="controls">
    <button id="left">⬅️</button>
    <button id="forward">⬆️</button>
    <button id="right">➡️</button>
  </div>
</div>

<audio id="music" loop autoplay>
  <source src="https://cdn.pixabay.com/audio/2022/03/15/audio_98c3c7d1d1.mp3" type="audio/mpeg">
</audio>

<script src="https://cdn.jsdelivr.net/npm/three@0.152.2/build/three.min.js"></script>
<script src="script.js"></script>
</body>
</html>
body {
  margin: 0;
  overflow: hidden;
  font-family: Arial, sans-serif;
}

#ui {
  position: absolute;
  top: 10px;
  left: 50%;
  transform: translateX(-50%);
  background: rgba(255,255,255,0.95);
  padding: 15px;
  border-radius: 15px;
  text-align: center;
  z-index: 10;
}

select {
  margin: 5px;
  padding: 6px;
  border-radius: 8px;
}

button {
  font-size: 20px;
  padding: 10px 14px;
  margin: 5px;
  border: none;
  border-radius: 10px;
  background: #ff69b4;
  color: white;
}

.controls {
  margin-top: 10px;
}

.hidden {
  display: none !important;
}scene.background
