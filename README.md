<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Arcade Profile</title>
  <link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Press Start 2P', cursive;
      background: radial-gradient(circle at center, #0f0c29, #302b63, #24243e);
      color: #fff;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .arcade-card {
      background: linear-gradient(145deg, #ff0844, #ffb199);
      border: 4px solid #fff;
      border-radius: 20px;
      padding: 30px;
      text-align: center;
      max-width: 420px;
      box-shadow: 0 0 25px #00f0ff, 0 0 15px #ff00cc;
      animation: pulse 3s infinite;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .arcade-card:hover {
      transform: scale(1.05);
      box-shadow: 0 0 40px #ff00cc, 0 0 25px #00f0ff;
    }

    .arcade-card img {
      width: 220px;
      height: auto;
      border: 4px dashed #00f0ff;
      border-radius: 10px;
      margin-bottom: 20px;
      box-shadow: 0 0 20px #f41cc5;
      transition: filter 0.3s;
    }

    .arcade-card img:hover {
      filter: brightness(1.2) saturate(1.3);
    }

    .arcade-card h1 {
      font-size: 18px;
      margin: 15px 0;
      color: #ffea00;
      text-shadow: 0 0 5px #ff00cc, 0 0 10px #00f0ff, 0 0 20px #ff00cc;
    }

    .arcade-card p {
      font-size: 12px;
      color: #fff;
      margin: 10px 0;
      text-shadow: 1px 1px #000;
    }

    .arcade-card p span {
      color: #ffeb3b;
    }

    /* ==== Status Bars ==== */
    .status {
      margin-top: 20px;
      text-align: left;
    }

    .status-label {
      font-size: 10px;
      margin: 8px 0;
      color: #ffea00;
      text-shadow: 1px 1px #000;
    }

    .bar {
      width: 100%;
      height: 15px;
      background: #222;
      border: 2px solid #fff;
      border-radius: 8px;
      overflow: hidden;
      margin-bottom: 10px;
    }

    .bar-fill {
      height: 100%;
      transition: width 0.5s ease-in-out;
    }

    .hp { background: linear-gradient(90deg, #ff0000, #ff5757); }
    .exp { background: linear-gradient(90deg, #00f0ff, #0077ff); }
    .level { background: linear-gradient(90deg, #22f56c, #1afe29); }

    @keyframes pulse {
      0% { box-shadow: 0 0 25px #22f56c, 0 0 10px #1afe29; }
      50% { box-shadow: 0 0 40px #ff00cc, 0 0 20px #00f0ff; }
      100% { box-shadow: 0 0 25px #00f0ff, 0 0 10px #ff00cc; }
    }

    /* Responsive */
    @media (max-width: 500px) {
      .arcade-card {
        width: 90%;
        padding: 20px;
      }

      .arcade-card img {
        width: 180px;
      }
    }
  </style>
</head>
<body>
  <div class="arcade-card">
    <img src="fai.JPG" alt="Atchara">
    <h1>SIRIPORN SOOKYING</h1>
    <p><span>Email:</span> siriporn253311@gmail.com</p>
    <p><span>Department:</span> Computer Engineering</p>
    <p><span>Faculty:</span> Engineering and Industrial Technology</p>

    <!-- Status Section -->
    <div class="status">
      <div class="status-label">HP</div>
      <div class="bar"><div class="bar-fill hp" style="width: 80%;"></div></div>

      <div class="status-label">EXP</div>
      <div class="bar"><div class="bar-fill exp" style="width: 65%;"></div></div>

      <div class="status-label">LEVEL</div>
      <div class="bar"><div class="bar-fill level" style="width: 45%;"></div></div>
    </div>
  </div>
</body>
</html>
