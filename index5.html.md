<!DOCTYPE html>
<html lang="kk">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Немереміз Инабат</title>
  <style>
    body { font-family: sans-serif; text-align: center; background: #fff8f2; color: #333; margin: 0; padding: 0; }
    h1 { font-size: 2em; margin-top: 20px; }
    .info { margin: 20px auto; max-width: 500px; font-size: 18px; }
    .countdown { font-size: 24px; margin: 20px 0; font-weight: bold; }
    iframe { width: 100%; border: none; }
    .footer { margin-top: 30px; font-size: 16px; color: #555; }
  </style>
</head>
<body>
  <h1>Шілдехана: Немереміз Инабат</h1>
  <div class="info">
    <p>Құрметті туыстар мен достар!</p>
    <p>Сіздерді шілдеханаға шақырамыз 🎉</p>
    <p><strong>13 маусым, 12:00</strong></p>
    <p>Мекенжай: Қаратау 33 (п. Деркул, Орал)</p>
  </div>

  <iframe width="100%" height="300" src="https://www.youtube.com/embed/ZgoZXJ6BtFY?autoplay=1&loop=1&playlist=ZgoZXJ6BtFY" 
  title="YouTube video player" allow="autoplay; encrypted-media" allowfullscreen></iframe>

  <div class="countdown" id="timer">Таймер жүктелуде...</div>

  <iframe src="https://makemap.2gis.ru/widget?data=eJw1Ts1qwzAMfhftGorjOq7jB-jYrbfCRg8h1jaDExlHhXYh7z4l2XT60Pc7A5WABcMr0oBcIk7gP2bgZ0bwcMaO7wWhglwoY-GNn6GnREX4F6Vd_amF58hpdQgMOPUlZo407o-ftzHgA3yt_m-p4GsvfK5xf20XiiOLvicZFceOtzFNfdCnWhtXrcjUpjU38ccAXlu13CoYunyhKe6FM6SOwYv2aKxqjBa9sdZUkFa6UYfWaqfbxrXOHE9W5hEN4J1kym5K6fqNmN63J5c7Lr9pRFjs"
  height="400"
  sandbox="allow-same-origin allow-scripts allow-popups allow-forms allow-modals allow-top-navigation-by-user-activation"></iframe>

  <div class="footer">
    <p>Той иелері: ата-ажесі / папа-мамасы</p>
    <p>Байланыс: +7 705 514 3063</p>
  </div>

  <script>
    const deadline = new Date("2025-06-13T12:00:00").getTime();
    const timer = document.getElementById("timer");
    setInterval(() => {
      const now = new Date().getTime();
      const t = deadline - now;
      if (t <= 0) {
        timer.innerHTML = "Той басталды!";
        return;
      }
      const days = Math.floor(t / (1000 * 60 * 60 * 24));
      const hours = Math.floor((t % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
      const minutes = Math.floor((t % (1000 * 60 * 60)) / (1000 * 60));
      const seconds = Math.floor((t % (1000 * 60)) / 1000);
      timer.innerHTML = `${days} күн, ${hours} сағат, ${minutes} мин, ${seconds} сек қалды`;
    }, 1000);
  </script>
</body>
</html>