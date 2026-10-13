<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#fff2f4">
<title>Bhumika, One Small Thing 💗</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Patrick+Hand&family=Quicksand:wght@400;500;600;700&family=Caveat:wght@600;700&display=swap" rel="stylesheet">

<style>
:root {
  --ink: #573247;
  --pink: #ed347c;
  --hot: #f45d98;
  --cream: #fff5ed;
  --muted: #805f70;
}

* {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  min-height: 100vh;
  color: var(--ink);
  font-family: 'Patrick Hand', 'Quicksand', cursive;
  background:
    radial-gradient(
      ellipse at 50% 20%,
      #fffaf1 0%,
      #fff5ed 48%,
      #ffe7ef 100%
    );
  overflow-x: hidden;
}

/* Soft background decorations */

body::before {
  content: "";
  position: fixed;
  inset: 0;
  pointer-events: none;
  opacity: .32;
  background-image:
    radial-gradient(circle at 7% 20%, #f7a6c5 0 2px, transparent 3px),
    radial-gradient(circle at 91% 15%, #f7a6c5 0 3px, transparent 4px),
    radial-gradient(circle at 13% 79%, #f7a6c5 0 2px, transparent 3px),
    radial-gradient(circle at 85% 72%, #f7a6c5 0 2px, transparent 3px);
  z-index: 0;
}

.wrap {
  width: min(650px, 94%);
  margin: auto;
  padding: 18px 0 28px;
  position: relative;
  z-index: 1;
}

.brand {
  text-align: center;
  font-family: 'Quicksand', sans-serif;
  font-size: 11px;
  font-weight: 700;
  letter-spacing: 1.7px;
  color: #ce4779;
  text-transform: uppercase;
  margin: 8px 0 14px;
}

/* Progress indicators */

.progress {
  display: flex;
  justify-content: center;
  gap: 6px;
  margin: 0 0 14px;
}

.dot {
  height: 6px;
  width: 19px;
  border-radius: 20px;
  background: #f4c9d8;
  transition: .25s;
}

.dot.on {
  width: 31px;
  background: var(--pink);
}

/* Paper-style pages */

.card {
  display: none;
  position: relative;
  isolation: isolate;
  background: rgba(255, 250, 245, .94);
  border: 2px solid #fff;
  border-radius: 20px;
  padding: clamp(21px, 5vw, 35px);
  text-align: center;
  box-shadow:
    0 7px 0 #f7d9df,
    0 15px 40px #bd64801c;
  animation: enter .3s ease;
  overflow: hidden;
}

.card::before {
  content: "✿  ˚｡⋆";
  position: absolute;
  top: 9px;
  left: 12px;
  color: #f39abb;
  font-size: 17px;
  opacity: .9;
  z-index: -1;
}

.card::after {
  content: "♡";
  position: absolute;
  right: 15px;
  top: 8px;
  color: #f06b9e;
  font-size: 23px;
  transform: rotate(14deg);
  z-index: -1;
}

.card.active {
  display: block;
}

@keyframes enter {
  from {
    opacity: 0;
    transform: translateY(7px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.emoji {
  font-size: 43px;
  margin: 4px 0 10px;
}

.pill {
  display: inline-block;
  border-radius: 999px;
  background: #ffe4ee;
  color: #bc3c72;
  font-family: 'Quicksand', sans-serif;
  font-size: 10px;
  letter-spacing: 1px;
  font-weight: 700;
  padding: 8px 12px;
  margin-bottom: 14px;
}

h1 {
  font-family: 'Caveat', 'Patrick Hand', cursive;
  font-size: clamp(43px, 10vw, 62px);
  line-height: .98;
  margin: 0 0 17px;
  font-weight: 700;
}

h2 {
  font-family: 'Patrick Hand', cursive;
  font-size: clamp(29px, 7vw, 38px);
  line-height: 1.1;
  margin: 0 0 13px;
}

p {
  font-size: clamp(17px, 4.2vw, 20px);
  line-height: 1.43;
  color: var(--muted);
  margin: 10px 0;
}

strong,
.accent {
  color: #d93f7e;
  font-weight: 700;
}

/* Paper note */

.note {
  background: #fff0e2;
  border: 2px solid #f2c8ae;
  border-radius: 12px;
  padding: 14px;
  text-align: left;
  margin: 19px 0;
  color: #67465a;
  line-height: 1.45;
  font-size: 18px;
  box-shadow: 0 4px 0 #f9e0d1;
}

/* Buttons */

.row {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 10px;
  margin-top: 22px;
}

button,
.insta {
  font-family: 'Patrick Hand', 'Quicksand', sans-serif;
  font-size: 18px;
  font-weight: 700;
  border: 0;
  border-radius: 999px;
  padding: 12px 19px;
  cursor: pointer;
  transition: transform .18s, box-shadow .18s;
  position: relative;
  z-index: 2;
}

button:hover,
.insta:hover {
  transform: translateY(-2px);
}

.primary,
.accepted {
  color: white;
  background: linear-gradient(135deg, #ff6fa6, #e92f7b);
  box-shadow:
    0 5px 0 #c72b68,
    0 9px 18px #f0529133;
}

.secondary {
  background: #fff2f5;
  color: #7c4d65;
  border: 1px solid #f3c5d6;
  box-shadow: 0 3px 0 #f3d8e2;
}

.choice {
  display: block;
  width: 100%;
  text-align: left;
  margin: 10px auto;
  background: #fff6f6;
  border: 1.5px solid #f0c7d3;
  border-radius: 14px;
  color: #594052;
  box-shadow: 0 3px 0 #f7e2e4;
}

.choice:hover {
  background: #ffeaf2;
}

:focus-visible {
  outline: 3px solid #d93f7e;
  outline-offset: 3px;
}

/* Apology buttons */

.apology-buttons {
  position: relative;
  min-height: 108px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  gap: 12px;
  margin-top: 17px;
}

.not-accepted {
  background: #fff3f2;
  color: #6e4d5c;
  border: 1px solid #edc8d2;
  box-shadow: 0 4px 0 #efd9dc;
  touch-action: manipulation;
}

#message {
  min-height: 28px;
  font-size: 19px;
  font-weight: 700;
  color: #d93f7e;
}

/* Instagram link */

.insta {
  display: inline-block;
  text-decoration: none;
  color: white;
  background: linear-gradient(
    110deg,
    #ff638d,
    #ed3e8c,
    #ba70d9
  );
  box-shadow:
    0 5px 0 #c82d73,
    0 9px 18px #e65d972e;
  margin-top: 16px;
}

.small {
  font-family: 'Quicksand', sans-serif;
  font-size: 11px;
  color: #a08491;
}

.footer {
  text-align: center;
  font-family: 'Caveat', cursive;
  font-size: 20px;
  color: #a16b85;
  padding: 19px 8px 0;
}

/* Floating flowers */

.flower {
  position: fixed;
  bottom: -35px;
  pointer-events: none;
  z-index: 0;
  opacity: .65;
  animation: rise linear infinite;
}

@keyframes rise {
  to {
    transform: translateY(-110vh) rotate(280deg);
  }
}

/* Decorative flowers inside cards */

.corner-flower {
  position: absolute;
  font-size: 28px;
  opacity: .5;
  pointer-events: none;
}

.corner-flower.left {
  left: 7px;
  bottom: 14px;
  transform: rotate(-20deg);
}

.corner-flower.right {
  right: 7px;
  bottom: 14px;
  transform: rotate(20deg);
}

/* Mobile styling */

@media (max-width: 420px) {
  button,
  .insta {
    font-size: 17px;
    padding: 12px 16px;
  }

  .card {
    border-radius: 18px;
  }

  .wrap {
    width: 93%;
  }
}

/* Respect reduced-motion settings */

@media (prefers-reduced-motion: reduce) {
  *,
  *::before,
  *::after {
    animation-duration: .01ms !important;
    transition-duration: .01ms !important;
    scroll-behavior: auto !important;
  }
}
</style>
</head>

<body>

<div id="flowers" aria-hidden="true"></div>

<main class="wrap">

  <div class="brand">
    A tiny case file · made with 💗
  </div>

  <div
    class="progress"
    id="progress"
    aria-label="Page progress"
  ></div>


  <!-- PAGE 1: OPENING -->

  <section class="card active">

    <div class="emoji">🚨💌</div>

    <div class="pill">BREAKING NEWS</div>

    <h1>
      Bhumika <span class="accent">vs.</span> Arup
    </h1>

    <p>
      A small misunderstanding has somehow become
      a whole international crisis. 😭
    </p>

    <p>
      <strong>Bhumika:</strong>
      Chief Justice of Being Mad
      <br>
      <strong>Arup:</strong>
      Professional Overthinker
    </p>

    <div class="note">
      📰 Latest update: Arup admits his communication
      skills may need a software update.
    </div>

    <div class="row">
      <button class="primary" onclick="showPage(1)">
        Open the case file →
      </button>
    </div>

    <p class="small">
      One silly case file. One sincere apology.
      No courtroom snacks.
    </p>

    <span class="corner-flower left">🌸</span>
    <span class="corner-flower right">🌷</span>

  </section>


  <!-- PAGE 2: INVESTIGATION -->

  <section class="card">

    <div class="emoji">🕵️‍♀️🔎</div>

    <h2>What went wrong?</h2>

    <p>Choose the closest explanation, Your Honour.</p>

    <button
      class="choice"
      onclick="theory('Texts need subtitles. 😭')"
    >
      📱 Miscommunication — texts need subtitles.
    </button>

    <button
      class="choice"
      onclick="theory('Brain.exe stopped working at the worst moment. 🫠')"
    >
      🧠 Brain.exe stopped working.
    </button>

    <button
      class="choice"
      onclick="theory('A little communication update was needed. 🔄')"
    >
      🔄 A little communication update was needed.
    </button>

    <p id="theoryResult" class="accent" aria-live="polite"></p>

    <div class="row">
      <button class="secondary" onclick="showPage(0)">
        ← Back
      </button>

      <button class="primary" onclick="showPage(2)">
        Next →
      </button>
    </div>

    <span class="corner-flower left">🌼</span>
    <span class="corner-flower right">🌸</span>

  </section>


  <!-- PAGE 3: SINCERE APOLOGY -->

  <section class="card">

    <div class="emoji">🥺🤍</div>

    <h2>Jokes aside…</h2>

    <p>
      Bhumika, I’m sorry this misunderstanding
      happened and that things ended up this way.
    </p>

    <p>
      I don’t want to dismiss how you feel, argue
      about who’s right, or make excuses. I should
      listen properly and explain myself more clearly.
    </p>

    <p>
      <strong>You don’t have to forgive me right away.</strong>
      I just wanted to say sorry sincerely.
      I’ll respect your space.
    </p>

    <div class="note">
      — Arup, the idiot trying to communicate
      like a normal human being. 🫡
    </div>

    <div class="row">
      <button class="secondary" onclick="showPage(1)">
        ← Back
      </button>

      <button class="primary" onclick="showPage(3)">
        See the verdict ⚖️
      </button>
    </div>

    <span class="corner-flower left">🌷</span>
    <span class="corner-flower right">🌼</span>

  </section>


  <!-- PAGE 4: VERDICT -->

  <section class="card">

    <div class="emoji">⚖️🍓</div>

    <h2>The court’s verdict</h2>

    <p>
      After reviewing the evidence,
      the court finds Arup…
    </p>

    <div class="note">
      ☑️ Guilty of overthinking
      <br>
      ☑️ Guilty of not explaining things clearly enough
      <br>
      ☑️ Sentenced to listen properly and do better
      <br>
      ☑️ Allowed to hope for a conversation—not demand one
    </div>

    <p>Your Honour, what’s the verdict?</p>

    <div class="row">
      <button class="secondary" onclick="showPage(4)">
        Still angry 😤
      </button>

      <button class="primary" onclick="showPage(4)">
        You made me smile 😂
      </button>

      <button class="secondary" onclick="showPage(4)">
        Let’s talk 💬
      </button>
    </div>

    <span class="corner-flower left">🌸</span>
    <span class="corner-flower right">🌷</span>

  </section>


  <!-- PAGE 5: APOLOGY RESPONSE -->

  <section class="card">

    <div class="emoji">💗🫶</div>

    <h2>One last question…</h2>

    <p>
      Has the apology been accepted, Your Honour?
    </p>

    <p class="small">
      The runaway button is just a joke—you can
      still choose honestly.
    </p>

    <div class="apology-buttons">

      <button class="accepted" onclick="accepted()">
        💗 Apology Accepted
      </button>

      <button class="not-accepted" id="noBtn">
        😤 Not Accepted
      </button>

    </div>

    <p id="message" aria-live="polite"></p>

    <div class="row">
      <button class="secondary" onclick="showPage(3)">
        ← Back
      </button>

      <button class="primary" onclick="showPage(5)">
        One last thing… 💌
      </button>
    </div>

    <span class="corner-flower left">🌼</span>
    <span class="corner-flower right">🌸</span>

  </section>


  <!-- PAGE 6: ENDING AND INSTAGRAM -->

  <section class="card">

    <div class="emoji">💌🌷</div>

    <h2>Case file: almost closed</h2>

    <p>
      You don’t have to be okay every day.
      Your feelings are valid, and your pace is yours.
    </p>

    <div class="note">
      No pressure and no drama—just one person who’d
      like a chance to clear up the misunderstanding
      respectfully.
    </div>

    <p>
      <strong>If and when you’re comfortable, we can talk.</strong>
      ❤️
    </p>

    <p>
      Arup may be slightly nervous if you reply.
      Scientifically unverified. 😂
    </p>

    <a
      class="insta"
      href="https://www.instagram.com/_allabout.arup_/"
      target="_blank"
      rel="noopener noreferrer"
    >
      💌 Talk to Arup on Instagram
    </a>

    <p class="small">
      This opens Arup’s profile.
      You decide whether you’d like to reconnect.
    </p>

    <div class="row">
      <button class="secondary" onclick="showPage(0)">
        ↻ Replay
      </button>
    </div>

    <span class="corner-flower left">🌸</span>
    <span class="corner-flower right">🌷</span>

  </section>


  <div class="footer">
    Made with a little courage, a little humour,
    and a sincere apology. 💗
  </div>

</main>


<script>

/* PAGE NAVIGATION */

const pages = [...document.querySelectorAll(".card")];

const progress = document.getElementById("progress");

pages.forEach((_, i) => {
  const dot = document.createElement("span");

  dot.className = "dot" + (i === 0 ? " on" : "");

  progress.appendChild(dot);
});

function showPage(index) {
  pages.forEach((page, i) => {
    page.classList.toggle("active", i === index);
  });

  [...progress.children].forEach((dot, i) => {
    dot.classList.toggle("on", i === index);
  });

  window.scrollTo({
    top: 0,
    behavior: "smooth"
  });
}


/* INVESTIGATION CHOICES */

function theory(text) {
  document.getElementById("theoryResult").textContent = text;
}


/* APOLOGY ACCEPTED */

function accepted() {
  document.getElementById("message").textContent =
    "🥹❤️ CASE CLOSED! Arup’s happiness is now charging… 🍫🎉";

  const button = document.getElementById("noBtn");

  button.textContent = "😳 Wait, really?";

  button.style.position = "relative";
  button.style.left = "";
  button.style.top = "";
}


/* MOVING NOT-ACCEPTED BUTTON */

const noBtn = document.getElementById("noBtn");

let escapes = 0;

function moveNo(event) {
  if (escapes >= 5) {
    noBtn.textContent = "Okay, you can tap me 😅";

    noBtn.style.position = "relative";
    noBtn.style.left = "";
    noBtn.style.top = "";

    return;
  }

  if (event) {
    event.preventDefault();
  }

  escapes++;

  const margin = 12;
  const width = noBtn.offsetWidth;

  const maxX = Math.max(
    margin,
    window.innerWidth - width - margin
  );

  const maxY = Math.max(
    margin,
    window.innerHeight - noBtn.offsetHeight - margin
  );

  noBtn.style.position = "fixed";

  noBtn.style.left =
    (margin + Math.random() * (maxX - margin)) + "px";

  noBtn.style.top =
    (margin + Math.random() * (maxY - margin)) + "px";

  noBtn.style.zIndex = "20";

  noBtn.textContent =
    escapes >= 4
      ? "Catch me first! 🏃‍♀️"
      : "Not Accepted 😤";
}

noBtn.addEventListener("pointerenter", moveNo);
noBtn.addEventListener("click", moveNo);

noBtn.addEventListener(
  "touchstart",
  moveNo,
  { passive: false }
);


/* FLOATING FLOWERS AND HEARTS */

const flowerBox = document.getElementById("flowers");

const symbols = ["🌸", "💗", "🌷", "✨", "🌼"];

for (let i = 0; i < 14; i++) {
  const flower = document.createElement("span");

  flower.className = "flower";

  flower.textContent =
    symbols[Math.floor(Math.random() * symbols.length)];

  flower.style.left = Math.random() * 100 + "%";

  flower.style.animationDuration =
    (10 + Math.random() * 12) + "s";

  flower.style.animationDelay =
    (-Math.random() * 18) + "s";

  flower.style.fontSize =
    (12 + Math.random() * 13) + "px";

  flowerBox.appendChild(flower);
}

</script>

</body>
</html>
