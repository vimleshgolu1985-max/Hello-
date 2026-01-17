# Hello-
<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>PALLAVI MADAM JI</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      background: #5a2d82; /* royal purple */
      font-family: Arial, sans-serif;
      overflow: hidden;
    }h1 {
  color: white;
  font-size: 2.5rem;
  cursor: pointer;
  text-align: center;
}

.colors {
  display: none;
  flex-wrap: wrap;
  gap: 15px;
  justify-content: center;
}

.color-box {
  width: 70px;
  height: 70px;
  border-radius: 10px;
  cursor: pointer;
}

.message {
  position: fixed;
  bottom: 20px;
  background: white;
  padding: 12px 20px;
  border-radius: 20px;
  font-size: 1rem;
  display: none;
}

  </style>
</head>
<body>  <h1 id="title">PALLAVI MADAM JI 🎀</h1>  <div class="colors" id="colors">
    <div class="color-box" style="background:red"></div>
    <div class="color-box" style="background:blue"></div>
    <div class="color-box" style="background:green"></div>
    <div class="color-box" style="background:orange"></div>
    <div class="color-box" style="background:pink"></div>
    <div class="color-box" style="background:yellow"></div>
  </div>  <div class="message" id="message"></div>  <script>
    const title = document.getElementById('title');
    const colors = document.getElementById('colors');
    const messageBox = document.getElementById('message');

    const messages = [
      "Apni health ka dhyan rakhiye 💖",
      "Aap bahut special ho 🌸",
      "Aap hi best ho ✨",
      "Hamesha muskurate rahiye 😊",
      "Aap sabke liye inspiration ho 🌟",
      "Dil se dua hai aap hamesha khush raho 💝",
      "Aapki smile sab kuch beautiful bana deti hai 💫",
      "Aap jaise log bahut rare hote hain 💕"
    ];

    title.onclick = () => {
      title.style.display = 'none';
      colors.style.display = 'flex';
    };

    document.querySelectorAll('.color-box').forEach(box => {
      box.onclick = () => {
        const msg = messages[Math.floor(Math.random() * messages.length)];
        messageBox.innerText = msg;
        messageBox.style.display = 'block';
      };
    });
  </script></body>
</html>
