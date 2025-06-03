<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>🎉 Selamat! Anda Mendapatkan Hadiah 🎁</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      height: 100vh;
      background: linear-gradient(to right, #00c6ff, #0072ff);
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      color: white;
      text-align: center;
    }

    h1 {
      font-size: 2.5em;
      margin-bottom: 10px;
    }

    p {
      font-size: 1.2em;
      margin-bottom: 40px;
    }

    #prankButton {
      padding: 15px 30px;
      font-size: 18px;
      background-color: #ffffff;
      color: #0072ff;
      border: none;
      border-radius: 8px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
      cursor: pointer;
      transition: transform 0.2s ease;
      position: absolute;
    }

    #prankButton:hover {
      transform: scale(1.1);
    }

    footer {
      position: fixed;
      bottom: 10px;
      font-size: 0.9em;
      color: rgba(255, 255, 255, 0.7);
    }
  </style>
</head>
<body>

  <h1>🎉 Selamat! Anda Mendapatkan Hadiah Rp10.000.000 🎁</h1>
  <p>Klik tombol di bawah ini untuk mengklaim hadiah spesial Anda!</p>

  <button id="prankButton">Klaim Sekarang</button>

  <footer><marquee>Hadiah Langsung Di Transfer Ke rekening Anda.🤑</marquee></footer>

  <script>
    const button = document.getElementById('prankButton');

    document.addEventListener('mousemove', function(e) {
      const x = e.clientX;
      const y = e.clientY;
      const offsetX = Math.random() * 200 - 100;
      const offsetY = Math.random() * 200 - 100;
      button.style.left = (x + offsetX) + 'px';
      button.style.top = (y + offsetY) + 'px';
    });

    button.addEventListener('click', () => {
      alert("Ups! Loe Ketipu 😄😄😄 Ini cuma prank kalo mau uang yah kerja lah wkwkwk!");
    });
  </script>

</body>
</html>
