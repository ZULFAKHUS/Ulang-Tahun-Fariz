<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Selamat Ulang Tahun Fariz!</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom, #cceeff, #e6f7ff);
      color: #003366;
      overflow-x: hidden;
    }
    header {
      text-align: center;
      padding: 2em;
      background: url('Alam.png') center/cover no-repeat;
      colo![Uploading Alam.png…]()
r: white;
    }
    h1 {
      font-size: 2.5em;
      margin: 0;
    }
    .countdown {
      font-size: 1.2em;
      margin-top: 1em;
    }
    .gallery {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1em;
      padding: 2em;
    }
    .gallery img, .gallery video {
      max-width: 300px;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    }
    .popup {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #ffffffcc;
      padding: 1em;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
      display: none;
    }
  </style>
</head>
<body>
  <header>
    <h1>Selamat Ulang Tahun, Fariz Iqbal Maulidi!</h1>
    <p class="countdown" id="countdown"></p>
  </header>

  <main>
    <section style="text-align: center; padding: 2em;">
      <p>Selamat ulang tahun adik, makasih sudah menjadi tua semoga lekas sadar dan tetap sabar. Aku masih di sini, selalu di sini siap untuk mengolok - olok!!</p>
    </section>

<section class="gallery">
<img src="Fariz![Fariz (1)](https://github.com/user-attachments/assets/3b2db![Fariz (2)](https://github.com/user-attachments/assets![Fariz (4)](https://github.com/user-attachments/assets/6d5b1b4a-d497-4a15-a3a5-f7f65e19facf)
/0![Fariz (3)](https://github.com/user-attachments/assets/bc0546e2-0d8e-4508-9780-ce71bffc220e)
eb2b3f5-9b69-4abc-b156-96a1a502b75a)
122-1e4d-4578-b412-6942520be6d6)
 (1).jpg" alt="Orang Aneh">
    </section>

  <section style="text-align: center; padding: 2em;">
      <audio controls autoplay loop>
        <source src="https://github.com/user-attachments/assets/e9efacfe-7d9e-4e88-a0d5-1f90093f1b8c Bergema Sampai Selamanya.mov" type="audio/mpeg">
      </audio>
    </section>
  </main>

  <div class="popup" id="popup">
    <p id="popup-message"></p>
  </div>

  <script>
    // Countdown
    const countdownElement = document.getElementById('countdown');
    const birthday = new Date('May 13, 2025 00:00:00').getTime();
    const interval = setInterval(() => {
      const now = new Date().getTime();
      const distance = birthday - now;

      if (distance < 0) {
        clearInterval(interval);
        countdownElement.innerText = 'Selamat ulang tahun!';
        return;
      }

      const days = Math.floor(distance / (1000 * 60 * 60 * 24));
      const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((distance % (1000 * 60)) / 1000);

      countdownElement.innerText = `Ulang tahun dalam ${days} hari, ${hours} jam, ${minutes} menit, ${seconds} detik`;
    }, 1000);

    // Pop-up messages
    const messages = [
      'Jangan sering begadang',
      'Jangan sering minum minuman kemasan dan serbuk',
      'Banyak air putih',
      'Diusahakan makan sedikit gapapa, asal minum air putih',
      'Jangan banyak merokok',
      'Jangan seperti batu'
    ];
    const popup = document.getElementById('popup');
    const popupMessage = document.getElementById('popup-message');
    let messageIndex = 0;

    setInterval(() => {
      popupMessage.innerText = messages[messageIndex];
      popup.style.display = 'block';
      setTimeout(() => {
        popup.style.display = 'none';
      }, 3000);
      messageIndex = (messageIndex + 1) % messages.length;
    }, 5000);
  </script>
</body>
</html>
riz
