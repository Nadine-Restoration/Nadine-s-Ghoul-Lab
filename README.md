<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Nadine’s Ghoul Lab</title>

<link href="https://fonts.googleapis.com/css2?family=Cherry+Bomb+One&family=Nunito&display=swap" rel="stylesheet">

<style>
body {
  margin: 0;
  background: radial-gradient(circle at top, #3a003a, #0b0b0b);
  color: #ffb6d9;
  font-family: 'Nunito', sans-serif;
  overflow-x: hidden;
}

/* Sparkles */
.sparkle {
  position: fixed;
  width: 6px;
  height: 6px;
  background: #ffb6d9;
  border-radius: 50%;
  animation: sparkle 6s infinite;
  opacity: 0.7;
}

@keyframes sparkle {
  0% { transform: translateY(0); opacity: 0; }
  50% { opacity: 1; }
  100% { transform: translateY(-100vh); opacity: 0; }
}

/* Bats */
.bat {
  position: fixed;
  font-size: 24px;
  animation: fly 10s linear infinite;
}

@keyframes fly {
  from { transform: translateX(-10%); }
  to { transform: translateX(110%); }
}

header {
  text-align: center;
  padding: 60px 20px;
}

header img {
  max-width: 200px;
  margin-bottom: 20px;
  filter: drop-shadow(0 0 15px #ff4da6);
}

header h1 {
  font-family: 'Cherry Bomb One', cursive;
  font-size: 3rem;
  color: #ff4da6;
  text-shadow: 0 0 15px #ff4da6;
}

section {
  max-width: 1100px;
  margin: auto;
  padding: 60px 20px;
}

h2 {
  font-family: 'Cherry Bomb One', cursive;
  color: #ff4da6;
  font-size: 2.2rem;
}

.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 25px;
}

.card {
  background: #120012;
  border: 2px solid #ff4da6;
  border-radius: 15px;
  padding: 25px;
  box-shadow: 0 0 20px rgba(255,77,166,0.25);
}

.card:hover {
  transform: scale(1.03);
}

form {
  background: #120012;
  border: 2px solid #ff4da6;
  border-radius: 15px;
  padding: 30px;
}

input, textarea, select {
  width: 100%;
  padding: 12px;
  margin-bottom: 20px;
  border-radius: 10px;
  border: none;
  background: #0b0b0b;
  color: #ffb6d9;
}

button {
  width: 100%;
  padding: 15px;
  background: #ff4da6;
  border: none;
  border-radius: 12px;
  font-family: 'Cherry Bomb One', cursive;
  font-size: 1.2rem;
  cursor: pointer;
}

button:hover {
  background: #ffb6d9;
}

footer {
  text-align: center;
  padding: 30px;
  color: #aaa;
}
</style>
</head>

<body>

<!-- Sparkles -->
<div class="sparkle" style="left:10%;"></div>
<div class="sparkle" style="left:40%; animation-delay:2s;"></div>
<div class="sparkle" style="left:70%; animation-delay:4s;"></div>

<!-- Bats -->
<div class="bat" style="top:20%;">🦇</div>
<div class="bat" style="top:60%; animation-delay:5s;">🦇</div>

<header>
  <img src="logo.png" alt="Nadine’s Ghoul Lab Logo">
  <h1>Nadine’s Ghoul Lab</h1>
  <p>Frightfully Fab Restoration & Custom Accessories</p>
</header>

<section>
  <h2>🧪 Services & Pricing</h2>
  <div class="cards">
    <div class="card">
      <h3>Hair Restoration</h3>
      <p>💸 $35 – $120+</p>
      <p>Pricing depends on condition & style requested.</p>
    </div>
    <div class="card">
      <h3>Reroots</h3>
      <p>💸 $60 – $180+</p>
      <p>Fiber type & complexity affect pricing.</p>
    </div>
    <div class="card">
      <h3>3D Resin Accessories</h3>
      <p>💸 $10 – $75+</p>
      <p>Custom-designed and hand-finished.</p>
    </div>
    <div class="card">
      <h3>Full Custom Dolls</h3>
      <p>💸 $150+</p>
      <p>Quote required for all full customs.</p>
    </div>
  </div>
</section>

<section>
  <h2>🖤 Custom Request / Booking</h2>
  <form action="https://formspree.io/f/yourformid" method="POST">
    <input type="text" name="name" placeholder="Name" required>
    <input type="email" name="email" placeholder="Email" required>
    <select name="service">
      <option>Hair Restoration</option>
      <option>Reroot</option>
      <option>3D Resin Accessories</option>
      <option>Full Custom Doll</option>
    </select>
    <textarea name="details" rows="5" placeholder="Tell me about your ghoul…" required></textarea>
    <button type="submit">Submit Request 💀</button>
  </form>
</section>

<footer>
© 2025 Nadine’s Ghoul Lab | Online Commissions Only
</footer>

</body>
</html>
