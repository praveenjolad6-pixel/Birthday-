<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy Birthday Chandrakala 🎉</title>

<style>
body {
    margin: 0;
    padding: 0;
    text-align: center;
    font-family: 'Segoe UI', sans-serif;
    background: linear-gradient(135deg, #ff9a9e, #fad0c4);
    color: white;
    overflow: hidden;
}

h1 {
    margin-top: 60px;
    font-size: 42px;
}

h2 {
    font-size: 28px;
}

.card {
    background: rgba(255,255,255,0.2);
    padding: 20px;
    margin: 20px auto;
    width: 85%;
    border-radius: 15px;
    backdrop-filter: blur(10px);
}

#message {
    font-size: 18px;
    min-height: 120px;
}

button {
    padding: 12px 25px;
    font-size: 18px;
    border: none;
    border-radius: 25px;
    background: #ff4d6d;
    color: white;
    cursor: pointer;
    margin-top: 20px;
}

button:hover {
    background: #ff1e4d;
}

/* Balloons */
.balloon {
    position: absolute;
    bottom: -100px;
    width: 40px;
    height: 60px;
    border-radius: 50%;
    animation: float 6s infinite;
}

@keyframes float {
    0% {transform: translateY(0);}
    100% {transform: translateY(-800px);}
}
</style>
</head>

<body>

<h1>🎂 Happy Birthday 🎂</h1>
<h2>Chandrakala 💖</h2>

<div class="card">
    <div id="message"></div>

    <button onclick="showSurprise()">🎁 Click for Surprise</button>
</div>

<!-- Balloons -->
<div class="balloon" style="left:20%; background:#ff4d4d;"></div>
<div class="balloon" style="left:40%; background:#4da6ff; animation-delay:2s;"></div>
<div class="balloon" style="left:60%; background:#ffff66; animation-delay:4s;"></div>
<div class="balloon" style="left:80%; background:#66ff99; animation-delay:1s;"></div>

<!-- Music -->
<audio autoplay loop>
    <source src="https://www2.cs.uic.edu/~i101/SoundFiles/HappyBirthday.mid" type="audio/midi">
</audio>

<script>
// Typing Effect
let text = "Wishing you a day filled with happiness, a year filled with success, and a life filled with beautiful moments ✨\n\nStay happy, keep smiling 😊 and keep shining always 🌸";
let i = 0;

function typeEffect() {
    if (i < text.length) {
        document.getElementById("message").innerHTML += text.charAt(i);
        i++;
        setTimeout(typeEffect, 40);
    }
}

typeEffect();

// Surprise Button
function showSurprise() {
    alert("🎉 Once again Happy Birthday Chandrakala! 💖 Stay blessed and keep smiling always 😊");
}
</script>

</body>
</html>
