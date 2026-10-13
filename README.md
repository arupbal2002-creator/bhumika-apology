<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#fff2f6">
<title>Bhumika, One Small Thing 💗</title>

<style>
:root {
  --pink: #f45f98;
  --pink2: #ff8db5;
  --ink: #392b35;
  --muted: #766875;
  --cream: #fff9f4;
  --line: #f7d4e1;
}

* {
  box-sizing: border-box;
}

body {
  margin: 0;
  min-height: 100vh;
  font-family: system-ui, -apple-system, "Segoe UI", sans-serif;
  color: var(--ink);
  background:
    radial-gradient(circle at 10% 5%, #ffe0eb 0, transparent 30%),
    radial-gradient(circle at 90% 90%, #ffe6ef 0, transparent 35%),
    #fff8f5;
  overflow-x: hidden;
}

.wrap {
  width: min(620px, 92%);
  margin: auto;
  padding: 26px 0 30px;
  position: relative;
  z-index: 1;
}

.brand {
  text-align: center;
  font-size: 12px;
  font-weight: 800;
  letter-spacing: 2px;
  color: #d94e83;
  text-transform: uppercase;
  margin: 4px 0 16px;
}

/* PAGE PROGRESS */

.progress {
  display: flex;
  justify-content: center;
  gap: 6px;
  margin: 0 0 18px;
}

.dot {
  height: 6px;
  width: 22px;
  border-radius: 20px;
  background: #f4d4df;
  transition: 0.25s;
}

.dot.on {
  width: 32px;
  background: var(--pink);
}

/* PAGE CARDS */

.card {
  display: none;
  background: rgba(255, 255, 255, 0.94);
  border: 1px solid #f9d9e4;
  border-radius: 26px;
  padding: clamp(22px, 5vw, 36px);
  text-align: center;
  box-shadow: 0 18px 55px #c65c8212;
  animation: enter 0.3s ease;
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
  font-size: 42px;
  margin: 0 0 12px;
}

.pill {
  display: inline-block;
  border-radius: 999px;
  background: #fff0f5;
  color: #bf3e70;
  font-size: 11px;
  letter-spacing: 1.4px;
  font-weight: 800;
  padding: 8px 12px;
  margin-bottom: 16px;
}

h1 {
  font-size: clamp(30px, 7vw, 43px);
  line-height: 1.12;
  letter-spacing: -1.2px;
  margin: 0 0 16px;
}

h2 {
  font-size: clamp(24px, 5vw, 32px);
  line-height: 1.2;
  margin: 0 0 14px;
  letter-spacing: -0.5px;
}

p {
  font-size: 16px;
  line-height: 1.65;
  color: var(--muted);
  margin: 10px 0;
}

strong,
.accent {
  color: #dc4c83;
}

.note {
  background: var(--cream);
  border: 1px dashed #efb7cc;
  border-radius: 16px;
  padding: 15px;
  text-align: left;
  margin: 20px 0;
  color: #66535f;
  line-height: 1.6;
}

/* BUTTONS */

.row {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 10px;
  margin-top: 23px;
}

button,
.insta {
  font: inherit;
  font-size: 14px;
  font-weight: 750;
  border: 0;
  border-radius: 999px;
  padding: 14px 19px;
  cursor: pointer;
  transition: transform 0.18s, box-shadow 0.18s;
}

button:hover,
.insta:hover {
  transform: translateY(-2px);
}

.primary,
.accepted {
  color: white;
  background: linear-gradient(135deg, var(--pink2), var(--pink));
  box-shadow: 0 8px 20px #f45f982e;
}

.secondary {
  background: #fff0f5;
  color: #7b4a60;
  border: 1px solid #f7d4e1;
}

/* INVESTIGATION CHOICES */

.choice {
  display: block;
  width: 100%;
  text-align: left;
  margin: 10px auto;
  background: #fff8fb;
  border: 1px solid var(--line);
  border-radius: 15px;
  color: #594650;
}

.choice:hover {
  background: #ffeaf2;
}

.choice:focus-visible,
button:focus-visible,
a:focus-visible {
  outline: 3px solid #dc4c83;
  outline-offset: 3px;
}

/* APOLOGY BUTTONS */

.apology-buttons {
  position: relative;
  min-height: 110px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  gap: 12px;
  margin-top: 18px;
}

.not-accepted {
  background: #f2edf0;
  color: #5b4b55;
  border: 1px solid #e7dce3;
  touch-action: manipulation;
}

#message {
  min-height: 28px;
  font-weight: 800;
  color: #d94e83;
}

/* INSTAGRAM BUTTON */

.insta {
  display: inline-block;
  text-decoration: none;
  color: white;
  background: linear-gradient(
    110deg,
    #ff758c,
    #ff7eb3,
    #c56cf0
  );
  box-shadow: 0 8px 20px #e65d972e;
  margin-top: 16px;
}

.small {
  font-size: 12px;
  color: #a08e99;
}

.footer {
  text-align: center;
  font-size: 12px;
  color: #a18d98;
  padding: 18px 8px 0;
}

/* FLOATING FLOWERS */

.flower {
  position: fixed;
  bottom: -35px;
  pointer-events: none;
  z-index: 0;
  opacity: 0.55;
  animation: rise linear infinite;
}

@keyframes rise {
  to {
    transform: translateY(-110vh) rotate(280deg);
  }
}

/* MOBILE DESIGN */

@media (max-width: 420px) {
  button,
  .insta {
    font-size: 13px;
    padding: 13px 15px;
  }

  .card {
    border-radius: 22px;
  }
}

/* REDUCED MOTION ACCESSIBILITY */

@media (prefers-reduced-motion: reduce) {
  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    transition-duration: 0.01ms !important;
    scroll-behavior: auto !important;
  }
}
</style>
</head>

<body>

<!-- FLOATING FLOWERS AND HEARTS -->
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
      📰 Latest update: Arup admits his
      communication skills may need a software update.
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

  </section>


  <!-- PAGE 2: INVESTIGATION -->

  <section class="card">

    <div class="emoji">🕵️‍♀️</div>

    <h2>What went wrong?</h2>

    <p>
      Choose the closest explanation, Your Honour.
    </p>

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
      onclick="theory('Both sides could use a little software update. 🔄')"
    >
      🔄 A little communication update was needed.
    </button>

    <p
      id="theoryResult"
      class="accent"
      aria-live="polite"
    ></p>

    <div class="row">

      <button class="secondary" onclick="showPage(0)">
        ← Back
      </button>

      <button class="primary" onclick="showPage(2)">
        Next →
      </button>

    </div>

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

  </section>


  <!-- PAGE 4: COURT VERDICT -->

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

    <p>
      Your Honour, what’s the verdict?
    </p>

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

  </section>


  <!-- PAGE 5: APOLOGY BUTTONS -->

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

      <button
        class="accepted"
        onclick="accepted()"
      >
        💗 Apology Accepted
      </button>

      <button
        class="not-accepted"
        id="noBtn"
      >
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

  </section>


  <!-- PAGE 6: INSTAGRAM -->

  <section class="card">

    <div class="emoji">📱💌</div>

    <h2>Case file: almost closed</h2>

    <p>
      No pressure and no drama—just one person
      who’d like a chance to clear up the
      misunderstanding respectfully.
    </p>

    <p>
      <strong>
        If and when you’re comfortable, we can talk.
      </strong>
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


/* CREATE PROGRESS INDICATORS */

pages.forEach((_, i) => {

  const dot = document.createElement("span");

  dot.className = "dot" + (i === 0 ? " on" : "");

  progress.appendChild(dot);

});


/* CHANGE PAGE */

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


/* INVESTIGATION OPTIONS */

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
  const height = noBtn.offsetHeight;

  const maxX = Math.max(
    margin,
    window.innerWidth - width - margin
  );

  const maxY = Math.max(
    margin,
    window.innerHeight - height - margin
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


/* DESKTOP AND MOBILE EVENTS */

noBtn.addEventListener("pointerenter", moveNo);

noBtn.addEventListener("click", moveNo);

noBtn.addEventListener(
  "touchstart",
  moveNo,
  { passive: false }
);


/* FLOATING FLOWERS AND HEARTS */

const flowerBox = document.getElementById("flowers");

const symbols = ["🌸", "💗", "🌷", "✨"];

for (let i = 0; i < 14; i++) {

  const flower = document.createElement("span");

  flower.className = "flower";

  flower.textContent =
    symbols[Math.floor(Math.random() * symbols.length)];

  flower.style.left =
    Math.random() * 100 + "%";

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
