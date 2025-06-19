<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Happy Birthday Divyanshi 🎂</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom right, #ffe0f0, #f0f8ff);
      overflow-x: hidden;
      color: #333;
      text-align: center;
    }
    h1 {
      margin-top: 60px;
      font-size: 2.8em;
      color: #ff69b4;
      animation: fadeIn 2s ease-in;
    }
    .birthdate {
      font-size: 1.2em;
      color: #666;
      margin-bottom: 30px;
    }
    .surprise-box {
      background-color: #fff;
      padding: 20px;
      margin: 20px auto;
      width: 90%;
      max-width: 600px;
      border-radius: 20px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
      cursor: pointer;
      transition: transform 0.2s;
    }
    .surprise-box:hover {
      transform: scale(1.02);
    }
    .hidden-content {
      display: none;
      animation: fadeIn 1s ease-in;
    }
    .poem, .message, .special {
      margin: 20px 0;
      white-space: pre-line;
      font-size: 1.1em;
    }
    .countdown {
      font-size: 1em;
      margin-top: 40px;
      color: #888;
    }
    .ending-line {
      font-style: italic;
      margin-top: 30px;
      color: #b35cc9;
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
    .balloons {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      background: url('https://i.ibb.co/hXkrWZf/balloons.gif') repeat;
      background-size: cover;
      opacity: 0.2;
      z-index: -1;
    }
  </style>
</head>
<body>
  <audio autoplay loop>
    <source src="https://cdn.pixabay.com/audio/2022/10/25/audio_909ac5fa36.mp3" type="audio/mpeg">
  </audio>  <div class="balloons"></div>  <h1>Happy Birthday Divyanshi! 🎉</h1>
  <div class="birthdate">Born on 31st August 2007</div>  <div class="surprise-box" onclick="revealSurprise()">
    🎁 Tap to unwrap your surprise!
  </div>  <div class="hidden-content" id="surprise">
    <div class="poem">
      Tareefon ke laayak ho tum, sitaron se bhi pyari,
      31 August ko aayi thi duniya mein ek muskaan suhaani.
      Har pal muskurana, jaise ho khushiyon ki baat,
      Tumse milkar lagta hai, dil ne paayi hai raahat.Na keh sake shayad sab baatein hum tumse,
  Par har ek lamha khaas hai, jab tum paas ho humse.
  Umeed hai ye din ho tumhaare liye khaas,
  Khush raho hamesha, yehi hai meri aas. 💫
</div>
<div class="message">
  Main chahta tha ki tumhara birthday kuch alag ho... isliye yeh chhoti si surprise page.
  Tum smile karti ho toh lagta hai duniya thoda aur pyaari hai.
  Mujhe nahi pata main kitna khaas hoon tumhare liye,
  lekin tum zaroor ho khaas mere liye. 💖
</div>
<div class="special">
  <strong>You are special because...</strong>
  <br>• Tumhaari muskaan din bana deti hai.  
  • Tum bina bole bhi sab kuch keh jaati ho.  
  • Jiske bhi life mein jaogi, uski duniya ko tum chaand aur sitaron ki tarah roshan kar dogi. 🌟🌙
</div>
<div class="ending-line">
  Jiske bhi life mein jaogi, uski duniya ko tum chaand aur sitaron ki tarah roshan kar dogi. 🌟🌙
</div>

  </div>  <div class="countdown" id="countdown"></div>  <script>
    function revealSurprise() {
      const content = document.getElementById('surprise');
      if (content.style.display !== 'block') {
        content.style.display = 'block';
        const sound = new Audio('https://cdn.pixabay.com/audio/2022/10/30/audio_cbbd9e12e3.mp3');
        sound.play();
      }
    }

    // Countdown
    const nextBD = new Date("August 31, " + (new Date().getMonth() > 7 ? new Date().getFullYear()+1 : new Date().getFullYear()));
    const countdown = document.getElementById("countdown");
    setInterval(() => {
      const now = new Date();
      const diff = nextBD - now;
      const days = Math.floor(diff / (1000 * 60 * 60 * 24));
      countdown.innerText = `Only ${days} days left until Divyanshi's next birthday! 🎉`;
    }, 1000);
  </script></body>
</html>
