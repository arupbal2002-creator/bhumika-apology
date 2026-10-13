<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Bhumika vs Arup 💗</title>

<style>
:root {
  --pink: #ff78a5;
  --pink-dark: #e94e83;
  --cream: #fff8f0;
  --ink: #342833;
  --muted: #766773;
  --white: #ffffff;
}

* {
  box-sizing: border-box;
}

body {
  margin: 0;
  min-height: 100vh;
  font-family: Arial, Helvetica, sans-serif;
  color: var(--ink);
  background: linear-gradient(
    145deg,
    #fff1f6,
    var(--cream) 55%,
    #ffe8ef
  );
  overflow-x: hidden;
}

/* FLOATING FLOWERS AND HEARTS */

.petals {
  position: fixed;
  inset: 0;
  pointer-events: none;
  overflow: hidden;
  z-index: 0;
}

.petal {
  position: absolute;
  bottom: -50px;
  opacity: 0.6;
  animation: floatUp linear infinite;
}

@keyframes floatUp {
  from {
    transform: translateY(0) rotate(0deg);
  }

  to {
    transform: translateY(-115vh) rotate(360deg);
  }
}

/* MAIN CONTAINER */

.wrap {
  position: relative;
  z-index: 1;
  width: min(680px, 92%);
  margin: 0 auto;
  padding: 28px 0 45px;
}

.topline {
  text-align: center;
  color: var(--pink-dark);
  font-weight: 800;
  font-size: 12px;
  letter-spacing: 2px;
  text-transform: uppercase;
  margin-bottom: 12px;
}

/* PAGE CARDS */

.card {
  background: rgba(255, 255, 255, 0.93);
  border: 1px solid rgba(255, 120, 165, 0.25);
  border-radius: 26px;
  padding: clamp(22px, 5vw, 38px);
  box-shadow: 0 18px 55px rgba(173, 81, 116, 0.12);
  text-align: center;
  display: none;
  animation: appear 0.35s ease;
}

.card.active {
  display: block;
}

@keyframes appear {
  from {
    opacity: 0;
    transform: translateY(10px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.emoji {
  font-size: 45px;
  margin: 3px 0 12px;
}

h1,
h2 {
  line-height: 1.2;
  margin: 0 0 14px;
}

h1 {
  font-size: clamp(28px, 6vw, 40px);
}

h2 {
  font-size: clamp(24px, 5vw, 32px);
}

p {
  line-height: 1.65;
  font-size: 16px;
  color: var(--muted);
}

.highlight {
  color: var(--pink-dark);
  font-weight: 800;
}

.tag {
  display: inline-block;
  background: #fff0f5;
  color: #b43b68;
  padding: 7px 12px;
  border-radius: 999px;
  font-size: 12px;
  font-weight: bold;
  margin-bottom: 16px;
}

.note {
  background: #fff8ef;
  border: 1px dashed #f2b4c9;
  border-radius: 16px;
  padding: 15px;
  margin: 20px 0 0;
  text-align: left;
}

/* PROGRESS INDICATORS */

.progress {
  display: flex;
  gap: 6px;
  justify-content: center;
  margin: 0 0 15px;
}

.dot {
  width: 7px;
  height: 7px;
  border-radius: 50%;
  background: #f4cad8;
}

.dot.on {
  background: var(--pink-dark);
}

/* BUTTONS */

.btn-row {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  gap: 12px;
  margin-top: 24px;
}

button,
.insta-btn {
  border: 0;
  border-radius: 999px;
  padding: 14px 19px;
  font-size: 15px;
  font-weight: 800;
  cursor: pointer;
  transition: transform 0.18s ease, box-shadow 0.18s ease;
}

button:hover,
.insta-btn:hover {
  transform: translateY(-2px);
}

.primary {
  color: white;
  background: linear-gradient(135deg, #ff82ad, #ed568c);
  box-shadow: 0 8px 20px rgba(237, 86, 140, 0.23);
}

.secondary {
  color: #6e5260;
  background: #fff0f5;
  border: 1px solid #ffd0df;
}

/* INVESTIGATION OPTIONS */

.choice {
  display: block;
  width: 100%;
  max-width: 420px;
  margin: 10px auto;
  text-align: left;
  background: #fff7fa;
  color: var(--ink);
  border: 1px solid #f7cada;
  border-radius: 16px;
}

.choice:hover {
  background: #ffeaf2;
}

/* APOLOGY BUTTONS */

.apology-buttons {
  position: relative;
  min-height: 130px;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  gap: 14px;
  margin-top: 22px;
}

.accepted-btn {
  background: linear-gradient(135deg, #ff82ad, #ed568c);
  color: white;
  box-shadow: 0 8px 20px rgba(237, 86, 140, 0.23);
}

.not-accepted-btn {
  background: #f1edf0;
  color: #51434d;
  border: 1px solid #e6dce2;
  position: relative;
  touch-action: manipulation;
}

#apologyMessage {
  color: var(--pink-dark);
  font-weight: 800;
  font-size: 17px;
  min-height: 28px;
  margin-top: 18px;
}

/* INSTAGRAM BUTTON */

.insta-btn {
  display: inline-block;
  margin-top: 15px;
  padding: 16px 24px;
  color: white;
  text-decoration: none;
  background: linear-gradient(
    45deg,
    #ff758c,
    #ff7eb3,
    #c56cf0
  );
  box-shadow: 0 8px 20px rgba(255, 105, 150, 0.25);
}

.small {
  font-size: 12px;
  color: #9a8792;
}

.footer {
  text-align: center;
  font-size: 12px;
  color: #a38e99;
  margin-top: 18px;
}

/* MOBILE RESPONSIVE */

@media (max-width: 420px) {
  button,
  .insta-btn {
    font-size: 14px;
    padding: 13px 16px;
  }

  .apology-buttons {
    min-height: 150px;
  }
}

@media (prefers-reduced-motion: reduce) {
  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    transition-duration: 0.01ms !important;
  }
}
</style>
</head>

<body>

<!-- FLOATING FLOWERS -->
<div class="petals" id="petals" aria-hidden="true"></div>

<main class="wrap">

  <div class="topline">
    Officially Unofficial Case File • No. 001 💗
  </div>

  <div class="progress" id="progress" aria-label="Page progress"></div>

  <!-- PAGE 1: INTRODUCTION -->

  <section class="card active" data-page="0">

    <div class="emoji">🚨💌</div>

    <span class="tag">BREAKING NEWS</span>

    <h1>Bhumika vs Arup</h1>

    <p>
      A small misunderstanding has somehow become
      a full international crisis.
    </p>

    <p>
      One side is
      <span class="highlight">
        Bhumika, Chief Justice of Being Mad
      </span>.
      <br>

      The other side is
      <span class="highlight">
        Arup, Professional Overthinker
      </span>.
    </p>

    <div class="note">
      📰 Latest update: The accused admits his
      communication skills may need a software update.
    </div>

    <div class="btn-row">
      <button class="primary" onclick="goTo(1)">
        Open the case file →
      </button>
    </div>

    <p class="small">
      Contains mild nonsense, one sincere apology,
      and absolutely no courtroom snacks.
    </p>

  </section>

  <!-- PAGE 2: INVESTIGATION -->

  <section class="card" data-page="1">

    <div class="emoji">🕵️‍♀️🔎</div>

    <h2>Investigation Time</h2>

    <p>
      What probably happened here?
      Select the closest explanation, Your Honour.
    </p>

    <button
      class="choice"
      onclick="pickTheory('The message got misunderstood. Text messages need subtitles. 😭')"
    >
      📱 Miscommunication: texts need subtitles.
    </button>

    <button
      class="choice"
      onclick="pickTheory('Brain.exe stopped working at the worst possible moment. 🫠')"
    >
      🧠 Brain.exe stopped working at the worst moment.
    </button>

    <button
      class="choice"
      onclick="pickTheory('Both sides needed a tiny software update. 🔄')"
    >
      🔄 Both sides needed a tiny software update.
    </button>

    <p
      id="theoryResult"
      class="highlight"
      aria-live="polite"
    ></p>

    <div class="btn-row">

      <button class="secondary" onclick="goTo(0)">
        ← Back
      </button>

      <button class="primary" onclick="goTo(2)">
        Continue →
      </button>

    </div>

  </section>

  <!-- PAGE 3: SINCERE APOLOGY -->

  <section class="card" data-page="2">

    <div class="emoji">🥺🤍</div>

    <h2>Jokes Aside…</h2>

    <p>
      Bhumika, I'm sorry that this misunderstanding
      happened and that things ended up this way.
    </p>

    <p>
      I don't want to dismiss how you feel, argue
      about who's right, or make excuses. I should
      listen properly and explain myself more clearly.
    </p>

    <p>
      <span class="highlight">
        You don't have to forgive me right away.
      </span>

      I just wanted to say sorry sincerely,
      and I'll respect your space.
    </p>

    <div class="note">
      — From Arup, the idiot currently trying to
      communicate like a normal human being. 🫡
    </div>

    <div class="btn-row">

      <button class="secondary" onclick="goTo(1)">
        ← Back
      </button>

      <button class="primary" onclick="goTo(3)">
        Proceed to the verdict ⚖️
      </button>

    </div>

  </section>

  <!-- PAGE 4: COURT VERDICT -->

  <section class="card" data-page="3">

    <div class="emoji">⚖️🍓</div>

    <h2>The Court's Verdict</h2>

    <p>
      After reviewing the evidence, the court finds Arup:
    </p>

    <div class="note">
      ☑️ Guilty of overthinking
      <br>

      ☑️ Guilty of not explaining things well enough
      <br>

      ☑️ Sentenced to listen properly and do better
      <br>

      ☑️ Allowed to hope for a conversation—but not demand one
    </div>

    <p>
      Now, Your Honour, you may deliver your verdict. 😤
    </p>

    <div class="btn-row">

      <button class="secondary" onclick="goTo(4)">
        I'm still angry 😤
      </button>

      <button class="primary" onclick="goTo(4)">
        Okay, you made me smile 😂
      </button>

      <button class="secondary" onclick="goTo(4)">
        Let's clear things up 💬
      </button>

    </div>

  </section>

  <!-- PAGE 5: APOLOGY ACCEPTED OR NOT -->

  <section class="card" data-page="4">

    <div class="emoji">💗🫶</div>

    <h2>One Last Question…</h2>

    <p>
      Has the apology been accepted, Your Honour?
    </p>

    <p class="small">
      P.S. The next button is a silly joke.
      You can still choose whichever answer feels right.
    </p>

    <div class="apology-buttons" id="apologyButtons">

      <button
        class="accepted-btn"
        onclick="acceptedApology()"
      >
        💗 Apology Accepted
      </button>

      <button
        class="not-accepted-btn"
        id="notAccepted"
      >
        😤 Not Accepted
      </button>

    </div>

    <p id="apologyMessage" aria-live="polite"></p>

    <div class="btn-row">

      <button class="secondary" onclick="goTo(3)">
        ← Back to verdict
      </button>

      <button class="primary" onclick="goTo(5)">
        One last thing… 💌
      </button>

    </div>

  </section>

  <!-- PAGE 6: INSTAGRAM -->

  <section class="card" data-page="5">

    <div class="emoji">📱💌</div>

    <h2>Case File: Almost Closed</h2>

    <p>
      Bhumika, no pressure and no drama—just one
      person who'd like a chance to clear up the
      misunderstanding respectfully.
    </p>

    <p>
      <span class="highlight">
        If and when you're comfortable, we can talk.
      </span>
      ❤️
    </p>

    <p>
      Arup may be slightly nervous when you reply.
      This is a scientifically unverified fact. 😂
    </p>

    <a
      class="insta-btn"
      href="https://www.instagram.com/_allabout.arup_/"
      target="_blank"
      rel="noopener noreferrer"
    >
      💌 TALK TO ARUP ON INSTAGRAM
    </a>

    <p class="small">
      This opens Arup's Instagram profile.
      You decide whether you'd like to reconnect.
    </p>

    <div class="btn-row">
      <button class="secondary" onclick="goTo(0)">
        ↻ Replay the case
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

const cards = Array.from(
  document.querySelectorAll(".card")
);

const progress = document.getElementById("progress");

/* CREATE PROGRESS DOTS */

cards.forEach((card, index) => {

  const dot = document.createElement("span");

  dot.className = "dot" + (index === 0 ? " on" : "");

  progress.appendChild(dot);

});

/* CHANGE PAGE */

function goTo(index) {

  cards.forEach((card, i) => {

    card.classList.toggle("active", i === index);

  });

  Array.from(progress.children).forEach((dot, i) => {

    dot.classList.toggle("on", i === index);

  });

  window.scrollTo({
    top: 0,
    behavior: "smooth"
  });

}

/* INVESTIGATION OPTIONS */

function pickTheory(message) {

  document.getElementById("theoryResult").textContent =
    message;

}

/* APOLOGY ACCEPTED BUTTON */

function acceptedApology() {

  document.getElementById("apologyMessage").textContent =
    "🥹❤️ CASE CLOSED! Arup's happiness has returned to 1% battery… now charging! 🍫🎉";

  const noButton = document.getElementById("notAccepted");

  noButton.textContent = "😳 Wait, really?";

  noButton.style.transform = "scale(0.95)";

}

/* MOVING NOT-ACCEPTED BUTTON */

const noButton = document.getElementById("notAccepted");

let moveCount = 0;

function moveNoButton(event) {

  if (event) {
    event.preventDefault();
  }

  moveCount++;

  /*
    After several escapes, the button settles down
    so the joke doesn't become frustrating.
  */

  if (moveCount > 6) {

    noButton.textContent = "Okay, you can tap me now 😅";

    noButton.style.position = "relative";
    noButton.style.left = "";
    noButton.style.top = "";

    return;

  }

  const margin = 12;

  const buttonWidth = noButton.offsetWidth;
  const buttonHeight = noButton.offsetHeight;

  const maxX = Math.max(
    margin,
    window.innerWidth - buttonWidth - margin
  );

  const maxY = Math.max(
    margin,
    window.innerHeight - buttonHeight - margin
  );

  noButton.style.position = "fixed";

  noButton.style.left =
    (margin + Math.random() * (maxX - margin)) + "px";

  noButton.style.top =
    (margin + Math.random() * (maxY - margin)) + "px";

  noButton.style.zIndex = "1000";

  noButton.textContent =
    moveCount >= 4
      ? "Catch me first! 🏃‍♀️"
      : "Not Accepted 😤";

}

/* DESKTOP AND MOBILE EVENTS */

noButton.addEventListener(
  "pointerenter",
  moveNoButton
);

noButton.addEventListener(
  "click",
  moveNoButton
);

noButton.addEventListener(
  "touchstart",
  moveNoButton,
  { passive: false }
);

/* FLOATING FLOWERS AND HEARTS */

const petals = document.getElementById("petals");

const symbols = ["🌸", "💗", "🌷", "✨"];

for (let i = 0; i < 18; i++) {

  const petal = document.createElement("span");

  petal.className = "petal";

  petal.textContent =
    symbols[Math.floor(Math.random() * symbols.length)];

  petal.style.left =
    Math.random() * 100 + "%";

  petal.style.animationDuration =
    (9 + Math.random() * 12) + "s";

  petal.style.animationDelay =
    (-Math.random() * 18) + "s";

  petal.style.fontSize =
    (12 + Math.random() * 15) + "px";

  petals.appendChild(petal);

}

</script>

</body>
</html>
