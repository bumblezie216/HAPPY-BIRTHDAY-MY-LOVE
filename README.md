<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Lola 💙</title>
<style>
* {
    box-sizing: border-box;
}
html {
    scroll-behavior: smooth;
}
body {
    margin: 0;
    min-height: 100vh;
    overflow-x: hidden;
    font-family: Georgia, "Times New Roman", serif;
    color: #fffaf5;
    background:
        linear-gradient(
            180deg,
            #28375f 0%,
            #526a91 22%,
            #8298b5 42%,
            #b99caf 62%,
            #d8aa9a 78%,
            #ead0a9 100%
        );
}
/* =====================================================
   BACKGROUND SKY
===================================================== */
.sky {
    position: fixed;
    inset: 0;
    overflow: hidden;
    pointer-events: none;
    z-index: 0;
}
.sun {
    position: absolute;
    width: 190px;
    height: 190px;
    left: 50%;
    top: 68%;
    transform: translate(-50%, -50%);
    border-radius: 50%;
    background: #f9dfb2;
    box-shadow:
        0 0 35px rgba(249,223,178,.7),
        0 0 90px rgba(229,183,154,.45);
    opacity: .7;
}
.moon {
    position: absolute;
    width: 75px;
    height: 75px;
    right: 13%;
    top: 9%;
    border-radius: 50%;
    background: #f8f2df;
    box-shadow:
        0 0 25px rgba(248,242,223,.65),
        0 0 55px rgba(248,242,223,.25);
}
/* =====================================================
   STARS
===================================================== */
.star {
    position: absolute;
    width: 3px;
    height: 3px;
    border-radius: 50%;
    background: #fffaf2;
    box-shadow:
        0 0 6px rgba(255,250,242,.8);
    animation:
        twinkle 3s infinite alternate;
}
@keyframes twinkle {
    from {
        opacity: .3;
        transform: scale(.7);
    }
    to {
        opacity: .85;
        transform: scale(1.3);
    }
}
/* =====================================================
   FLOATING ELEMENTS
===================================================== */
.floating {
    position: fixed;
    bottom: -50px;
    pointer-events: none;
    z-index: 20;
    animation:
        floatUp linear forwards;
}
@keyframes floatUp {
    0% {
        transform:
            translateY(0)
            rotate(0deg);
        opacity: 0;
    }
    12% {
        opacity: .9;
    }
    100% {
        transform:
            translateY(-115vh)
            rotate(280deg);
        opacity: 0;
    }
}
/* =====================================================
   MAIN
===================================================== */
main {
    position: relative;
    z-index: 2;
    padding:
        60px
        16px
        100px;
    text-align: center;
}
/* =====================================================
   INTRO
===================================================== */
.intro {
    min-height: 82vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
.eyebrow {
    margin-bottom: 15px;
    font-size: 13px;
    letter-spacing: 5px;
    text-transform: uppercase;
    color: #f8eee6;
    opacity: .85;
}
h1 {
    margin: 0;
    font-size:
        clamp(48px, 12vw, 100px);
    line-height: .9;
    color: #fff8f0;
    text-shadow:
        0 4px 18px rgba(42,54,82,.2);
    animation:
        titleAppear 1.5s ease;
}
.name {
    display: block;
    color: #dcecf2;
    font-style: italic;
    text-shadow:
        0 0 16px rgba(220,236,242,.4);
}
.intro-text {
    max-width: 680px;
    margin:
        30px
        auto
        0;
    font-size:
        clamp(18px,4vw,24px);
    line-height: 1.7;
    color: #fff9f3;
    opacity: 0;
    animation:
        fadeIn 2s ease .6s forwards;
}
.scroll {
    margin-top: 45px;
    font-size: 12px;
    letter-spacing: 3px;
    opacity: .7;
    animation:
        bounce 2s infinite;
}
@keyframes titleAppear {
    from {
        opacity: 0;
        transform:
            translateY(25px)
            scale(.94);
    }
    to {
        opacity: 1;
        transform:
            translateY(0)
            scale(1);
    }
}
@keyframes fadeIn {
    from {
        opacity: 0;
    }
    to {
        opacity: 1;
    }
}
@keyframes bounce {
    0%,100% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(9px);
    }
}
/* =====================================================
   GLASS CARDS
===================================================== */
.card {
    width:
        min(94vw, 760px);
    margin:
        45px
        auto;
    padding:
        38px
        24px;
    border-radius: 30px;
    background:
        rgba(245,247,249,.17);
    border:
        1px solid
        rgba(255,250,245,.32);
    backdrop-filter:
        blur(15px);
    box-shadow:
        0 20px 50px
        rgba(50,55,80,.14);
}
.card h2 {
    margin-top: 0;
    font-size:
        clamp(28px,6vw,40px);
    color: #e8f3f5;
    text-shadow:
        0 2px 10px rgba(45,55,80,.15);
}
.card p {
    font-size: 18px;
    line-height: 1.85;
    color: #fffaf6;
}
/* =====================================================
   BIRTHDAY GAMES
===================================================== */
.game-intro {
    margin-bottom: 30px;
}
.game {
    margin:
        28px
        0;
    padding:
        27px
        18px;
    border-radius: 24px;
    background:
        rgba(244,245,248,.13);
    border:
        1px solid
        rgba(255,250,245,.22);
}
.game h3 {
    margin-top: 0;
    font-size: 25px;
    color: #f7eee4;
}
.game p {
    font-size: 16px;
}
/* =====================================================
   BUTTONS
===================================================== */
button {
    min-height: 44px;
    border: none;
    padding:
        12px
        20px;
    margin: 6px;
    border-radius: 50px;
    background:
        #f3e8d7;
    color:
        #43516f;
    font-family:
        Georgia,
        "Times New Roman",
        serif;
    font-size: 16px;
    cursor: pointer;
    box-shadow:
        0 5px 16px
        rgba(50,55,80,.14);
    transition:
        transform .25s ease,
        box-shadow .25s ease;
}
button:hover {
    transform:
        translateY(-3px);
    box-shadow:
        0 8px 22px
        rgba(50,55,80,.2);
}
button:active {
    transform:
        scale(.96);
}
/* =====================================================
   PRESENT GAME
===================================================== */
.presents {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 8px;
    margin-top: 20px;
}
.present {
    font-size: 52px;
    background: transparent;
    box-shadow: none;
    padding: 8px;
}
.present:hover {
    background: transparent;
    box-shadow: none;
    transform:
        translateY(-7px)
        rotate(-4deg)
        scale(1.08);
}
/* =====================================================
   CANDLE GAME
===================================================== */
.cake {
    margin: 15px 0;
    font-size: 75px;
    cursor: pointer;
    transition:
        transform .25s ease;
}
.cake:hover {
    transform:
        scale(1.08);
}
.candle-count {
    font-size: 16px;
    opacity: .85;
}
/* =====================================================
   STAR GAME
===================================================== */
.star-game {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 8px;
    margin-top: 20px;
}
.game-star {
    min-width: 44px;
    font-size: 27px;
    padding: 8px;
    background: transparent;
    color: white;
    box-shadow: none;
}
.game-star:hover {
    background: transparent;
    box-shadow: none;
    transform:
        scale(1.2);
}
.game-star.collected {
    opacity: .25;
    transform:
        scale(.7);
}
/* =====================================================
   QUIZ
===================================================== */
.quiz-options {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}
.quiz-options button {
    max-width: 250px;
}
/* =====================================================
   OCEAN GAME
===================================================== */
.ocean {
    position: relative;
    height: 220px;
    overflow: hidden;
    border-radius: 24px;
    margin-top: 20px;
    background:
        linear-gradient(
            180deg,
            #9bbbc5,
            #7298aa,
            #587f94
        );
}
.wave {
    position: absolute;
    left: -10%;
    width: 120%;
    height: 40px;
    border-radius: 50%;
    background:
        rgba(236,247,245,.25);
    animation:
        waveMove 5s ease-in-out infinite alternate;
}
.wave.one {
    top: 45px;
}
.wave.two {
    top: 105px;
    animation-delay: 1s;
}
.wave.three {
    top: 165px;
    animation-delay: 2s;
}
@keyframes waveMove {
    from {
        transform:
            translateX(-20px);
    }
    to {
        transform:
            translateX(20px);
    }
}
.otter {
    position: absolute;
    font-size: 42px;
    cursor: pointer;
    transition:
        transform .3s ease;
}
.otter:hover {
    transform:
        scale(1.2);
}
/* =====================================================
   PEONY GAME
===================================================== */
.flowers {
    display: grid;
    grid-template-columns:
        repeat(3, 1fr);
    gap: 12px;
    max-width: 400px;
    margin:
        20px
        auto;
}
.flower {
    min-height: 80px;
    font-size: 34px;
    padding: 10px;
    background:
        rgba(255,255,255,.12);
    border:
        1px solid
        rgba(255,255,255,.18);
    border-radius: 20px;
    box-shadow: none;
}
.flower.open {
    background:
        rgba(255,255,255,.24);
    transform:
        rotate(3deg);
}
/* =====================================================
   SECRET MESSAGE
===================================================== */
.secret {
    display: none;
    margin-top: 25px;
    padding: 22px;
    border-radius: 22px;
    background:
        rgba(255,255,255,.13);
    line-height: 1.8;
    font-size: 18px;
}
.secret.show {
    display: block;
    animation:
        fadeIn .8s ease;
}
/* =====================================================
   MUSIC
===================================================== */
.music-status {
    min-height: 30px;
    margin-top: 12px;
    font-size: 15px;
    opacity: .85;
}
/* =====================================================
   PROGRESS
===================================================== */
.progress {
    height: 10px;
    width: min(90%, 500px);
    margin:
        25px
        auto;
    border-radius: 20px;
    overflow: hidden;
    background:
        rgba(255,255,255,.18);
}
.progress-bar {
    height: 100%;
    width: 0%;
    border-radius: 20px;
    background:
        #e8ded0;
    transition:
        width .5s ease;
}
/* =====================================================
   FINAL
===================================================== */
.final {
    min-height: 55vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
.final-heart {
    font-size: 65px;
    animation:
        heartbeat 1.6s infinite;
}
@keyframes heartbeat {
    0%,100% {
        transform: scale(1);
    }
    50% {
        transform: scale(1.13);
    }
}
.signature {
    margin-top: 25px;
    font-size: 22px;
    font-style: italic;
    color: #e8f3f5;
}
/* =====================================================
   CONFETTI
===================================================== */
.confetti {
    position: fixed;
    top: -20px;
    z-index: 100;
    pointer-events: none;
    animation:
        confettiFall 3.5s linear forwards;
}
@keyframes confettiFall {
    0% {
        transform:
            translateY(0)
            rotate(0deg);
        opacity: 1;
    }
    100% {
        transform:
            translateY(110vh)
            rotate(650deg);
        opacity: 0;
    }
}
/* =====================================================
   MOBILE
===================================================== */
@media (max-width: 600px) {
    main {
        padding:
            40px
            12px
            80px;
    }
    .card {
        padding:
            30px
            18px;
    }
    .card p {
        font-size: 17px;
    }
    .sun {
        width: 150px;
        height: 150px;
    }
    .moon {
        width: 60px;
        height: 60px;
    }
    .flowers {
        gap: 8px;
    }
}
</style>
</head>
<body>
<!-- =====================================================
     BACKGROUND
===================================================== -->
<div class="sky">
    <div class="sun"></div>
    <div class="moon"></div>
    <div class="star" style="left:7%;top:8%;animation-delay:.3s"></div>
    <div class="star" style="left:16%;top:17%;animation-delay:1.1s"></div>
    <div class="star" style="left:27%;top:7%;animation-delay:.7s"></div>
    <div class="star" style="left:39%;top:15%;animation-delay:1.5s"></div>
    <div class="star" style="left:51%;top:6%;animation-delay:.4s"></div>
    <div class="star" style="left:64%;top:18%;animation-delay:1.2s"></div>
    <div class="star" style="left:77%;top:6%;animation-delay:.8s"></div>
    <div class="star" style="left:90%;top:21%;animation-delay:1.6s"></div>
    <div class="star" style="left:11%;top:31%;animation-delay:.5s"></div>
    <div class="star" style="left:24%;top:25%;animation-delay:1.4s"></div>
    <div class="star" style="left:47%;top:30%;animation-delay:.9s"></div>
    <div class="star" style="left:60%;top:27%;animation-delay:1.7s"></div>
    <div class="star" style="left:73%;top:34%;animation-delay:.6s"></div>
    <div class="star" style="left:87%;top:29%;animation-delay:1s"></div>
</div>
<main>
<!-- =====================================================
     INTRO
===================================================== -->
<section class="intro">
    <div class="eyebrow">
        A tiny universe made just for you
    </div>
    <h1>
        Happy Birthday
        <span class="name">Lola</span>
    </h1>
    <p class="intro-text">
        Today the sky feels a little softer,
        the stars feel a little brighter,
        and the universe has one very important
        reason to celebrate.
        <br><br>
        You. 💙
    </p>
    <div class="scroll">
        ↓ YOUR BIRTHDAY ADVENTURE STARTS HERE ↓
    </div>
</section>
<!-- =====================================================
     LOVE LETTER
===================================================== -->
<section class="card">
    <h2>For my Lola 💙</h2>
    <p>
        Happy 27th birthday to the girl who became
        one of the most beautiful parts of my world.
        <br><br>
        If I could give you anything today,
        I would give you every sunset,
        every peaceful night,
        every beautiful ocean,
        and every star in the sky.
        <br><br>
        Since I cannot exactly wrap up the universe
        and put it in a birthday box...
        I made you this little universe instead.
        <br><br>
        Every little thing here is a reminder
        that you are loved.
    </p>
</section>
<!-- =====================================================
     BIRTHDAY GAMES
===================================================== -->
<section class="card">
    <h2>🎮 Lola's Birthday Games</h2>
    <p class="game-intro">
        Your birthday mission has begun.
        Play the games below and unlock
        the final birthday surprise.
    </p>
    <div class="progress">
        <div
            id="progressBar"
            class="progress-bar">
        </div>
    </div>
    <p id="progressText">
        0 / 6 birthday games completed
    </p>
    <!-- GAME 1 -->
    <div class="game">
        <h3>🎁 Game One — Pick a Present</h3>
        <p>
            One of these presents contains
            a birthday message from Bree.
        </p>
        <div class="presents">
            <button
                class="present"
                data-message="You deserve every beautiful thing this world has to offer. 💙">
                🎁
            </button>
            <button
                class="present"
                data-message="If I could wrap up a sunset and give it to you, I would. 🌅">
                🎁
            </button>
            <button
                class="present"
                data-message="You are my favourite person in this enormous universe. ⭐">
                🎁
            </button>
        </div>
        <div
            id="presentResult"
            class="game-result">
        </div>
    </div>
    <!-- GAME 2 -->
    <div class="game">
        <h3>🎂 Game Two — Birthday Candles</h3>
        <p>
            Tap the cake to blow out the candles.
        </p>
        <div
            id="cake"
            class="cake"
            role="button"
            tabindex="0">
            🕯️🕯️🕯️
        </div>
        <div
            id="candleResult"
            class="game-result">
            3 candles are still glowing.
        </div>
    </div>
    <!-- GAME 3 -->
    <div class="game">
        <h3>⭐ Game Three — Catch the Stars</h3>
        <p>
            Catch all five stars to make
            Lola's birthday wish.
        </p>
        <div
            id="starGame"
            class="star-game">
        </div>
        <div
            id="starResult"
            class="game-result">
            0 / 5 stars collected
        </div>
    </div>
    <!-- GAME 4 -->
    <div class="game">
        <h3>💙 Game Four — How Well Do You Know Lola?</h3>
        <p id="quizQuestion">
            What colour does Lola love?
        </p>
        <div
            id="quizOptions"
            class="quiz-options">
            <button data-answer="wrong">
                Burgundy
            </button>
            <button data-answer="correct">
                Baby blue
            </button>
            <button data-answer="wrong">
                Green
            </button>
        </div>
        <div
            id="quizResult"
            class="game-result">
        </div>
    </div>
    <!-- GAME 5 -->
    <div class="game">
        <h3>🌊 Game Five — Find the Otter</h3>
        <p>
            Somewhere in the ocean is a little
            otter waiting to wish Lola happy birthday.
        </p>
        <div
            id="ocean"
            class="ocean">
            <div class="wave one"></div>
            <div class="wave two"></div>
            <div class="wave three"></div>
        </div>
        <div
            id="otterResult"
            class="game-result">
            Find the otter!
        </div>
    </div>
    <!-- GAME 6 -->
    <div class="game">
        <h3>🌸 Game Six — Blooming Birthday</h3>
        <p>
            Tap every flower to reveal
            six little reasons you are loved.
        </p>
        <div
            id="flowers"
            class="flowers">
        </div>
        <div
            id="flowerResult"
            class="game-result">
            0 / 6 flowers opened
        </div>
    </div>
</section>
<!-- =====================================================
     HAPPY BIRTHDAY MUSIC
===================================================== -->
<section class="card">
    <h2>🎵 A Birthday Song For You</h2>
    <p>
        No music file needed.
        <br><br>
        The Happy Birthday melody is created
        directly by this website.
    </p>
    <button
        id="musicButton"
        type="button">
        🎵 Play Happy Birthday
    </button>
    <div
        id="musicStatus"
        class="music-status">
    </div>
</section>
<!-- =====================================================
     FINAL SURPRISE
===================================================== -->
<section class="card">
    <h2>🎁 One Last Thing...</h2>
    <p>
        You have made it through your
        birthday adventure.
        <br><br>
        But there is one final message
        waiting for you.
    </p>
    <button
        id="secretButton"
        type="button">
        💙 Open Your Final Surprise
    </button>
    <div
        id="secret"
        class="secret">
        Happy 27th birthday, my love. 💙
        <br><br>
        I hope this next chapter of your life
        brings you softer mornings,
        beautiful sunsets,
        peaceful nights,
        oceans you finally get to see,
        and countless reasons to smile.
        <br><br>
        No matter how enormous this universe is,
        I am always going to be grateful
        that somehow our paths crossed.
        <br><br>
        You are my favourite little piece
        of the universe.
        <br><br>
        ⭐🌊🌸💙
    </div>
</section>
<!-- =====================================================
     FINAL
===================================================== -->
<section class="final">
    <div class="final-heart">
        💙
    </div>
    <h2>
        Happy 27th Birthday, Lola
    </h2>
    <p>
        I love you more than all the stars.
    </p>
    <p class="signature">
        With all my love,<br>
        Bree / Putiputi
    </p>
</section>
</main>
<script>
/* =====================================================
   FLOATING ELEMENTS
===================================================== */
const floatingSymbols = [
    "💙",
    "✨",
    "⭐",
    "🌸",
    "🦋",
    "🌊"
];
function createFloating() {
    const element =
        document.createElement("div");
    element.className =
        "floating";
    element.textContent =
        floatingSymbols[
            Math.floor(
                Math.random() *
                floatingSymbols.length
            )
        ];
    element.style.left =
        Math.random() * 100 + "vw";
    element.style.fontSize =
        (14 + Math.random() * 16) + "px";
    element.style.animationDuration =
        (7 + Math.random() * 6) + "s";
    document.body.appendChild(element);
    setTimeout(
        () => element.remove(),
        14000
    );
}
setInterval(
    createFloating,
    900
);
/* =====================================================
   GAME PROGRESS
===================================================== */
const completedGames =
    new Set();
function completeGame(number) {
    completedGames.add(number);
    const progress =
        Math.min(
            completedGames.size / 6 * 100,
            100
        );
    document.getElementById(
        "progressBar"
    ).style.width =
        progress + "%";
    document.getElementById(
        "progressText"
    ).textContent =
        completedGames.size +
        " / 6 birthday games completed";
    if (
        completedGames.size === 6
    ) {
        createConfetti();
        document.getElementById(
            "progressText"
        ).textContent =
            "🎉 All six games completed! 🎉";
    }
}
/* =====================================================
   GAME 1 — PRESENTS
===================================================== */
document
    .querySelectorAll(".present")
    .forEach(
        present => {
            present.addEventListener(
                "click",
                () => {
                    document.getElementById(
                        "presentResult"
                    ).textContent =
                        present.dataset.message;
                    completeGame(1);
                    createConfetti();
                }
            );
        }
    );
/* =====================================================
   GAME 2 — CANDLES
===================================================== */
let candles = 3;
const cake =
    document.getElementById("cake");
function blowCandle() {
    if (candles <= 0) {
        return;
    }
    candles--;
    if (candles === 2) {
        cake.textContent =
            "🕯️🕯️💨";
    } else if (candles === 1) {
        cake.textContent =
            "🕯️💨💨";
    } else {
        cake.textContent =
            "🎂✨";
    }
    document.getElementById(
        "candleResult"
    ).textContent =
        candles > 0
        ? candles +
          " candle" +
          (candles === 1 ? "" : "s") +
          " still glowing."
        : "🎉 All the candles are out! Make your birthday wish. 💙";
    if (candles === 0) {
        completeGame(2);
        createConfetti();
    }
}
cake.addEventListener(
    "click",
    blowCandle
);
cake.addEventListener(
    "keydown",
    event => {
        if (
            event.key === "Enter" ||
            event.key === " "
        ) {
            event.preventDefault();
            blowCandle();
        }
    }
);
/* =====================================================
   GAME 3 — STARS
===================================================== */
const starGame =
    document.getElementById(
        "starGame"
    );
let starsCollected = 0;
for (
    let i = 0;
    i < 5;
    i++
) {
    const star =
        document.createElement("button");
    star.type = "button";
    star.className =
        "game-star";
    star.textContent =
        "⭐";
    star.setAttribute(
        "aria-label",
        "Collect star " + (i + 1)
    );
    star.addEventListener(
        "click",
        () => {
            if (
                star.classList.contains(
                    "collected"
                )
            ) {
                return;
            }
            star.classList.add(
                "collected"
            );
            starsCollected++;
            document.getElementById(
                "starResult"
            ).textContent =
                starsCollected +
                " / 5 stars collected";
            if (
                starsCollected === 5
            ) {
                document.getElementById(
                    "starResult"
                ).textContent =
                    "🌟 Wish granted. May 27 bring you beautiful things. 💙";
                completeGame(3);
                createConfetti();
            }
        }
    );
    starGame.appendChild(
        star
    );
}
/* =====================================================
   GAME 4 — QUIZ
===================================================== */
document
    .querySelectorAll(
        "#quizOptions button"
    )
    .forEach(
        option => {
            option.addEventListener(
                "click",
                () => {
                    const result =
                        document.getElementById(
                            "quizResult"
                        );
                    if (
                        option.dataset.answer ===
                        "correct"
                    ) {
                        result.textContent =
                            "💙 Correct! You know Lola very well.";
                        completeGame(4);
                        createConfetti();
                    } else {
                        result.textContent =
                            "Not that one 😂 Try again!";
                    }
                }
            );
        }
    );
/* =====================================================
   GAME 5 — OTTER
===================================================== */
const ocean =
    document.getElementById(
        "ocean"
    );
const otter =
    document.createElement(
        "div"
    );
otter.className =
    "otter";
otter.textContent =
    "🦦";
otter.style.left =
    "72%";
otter.style.top =
    "48%";
ocean.appendChild(
    otter
);
otter.addEventListener(
    "click",
    () => {
        document.getElementById(
            "otterResult"
        ).textContent =
            "🦦 You found the birthday otter! It says: Happy birthday Lola! 💙";
        completeGame(5);
        createConfetti();
    }
);
/* =====================================================
   GAME 6 — PEONIES
===================================================== */
const flowerMessages = [
    "Because your smile makes ordinary days feel special. 🌸",
    "Because your heart is softer than you realise. 💙",
    "Because you make the world feel a little warmer. 🌷",
    "Because you are uniquely you. ✨",
    "Because you deserve to be celebrated today. 🌸",
    "Because you are loved more than words can explain. 💙"
];
const flowers =
    document.getElementById(
        "flowers"
    );
let flowersOpened = 0;
flowerMessages.forEach(
    (message, index) => {
        const flower =
            document.createElement(
                "button"
            );
        flower.type = "button";
        flower.className =
            "flower";
        flower.textContent =
            "🌸";
        flower.addEventListener(
            "click",
            () => {
                if (
                    flower.classList.contains(
                        "open"
                    )
                ) {
                    return;
                }
                flower.classList.add(
                    "open"
                );
                flower.textContent =
                    message;
                flowersOpened++;
                document.getElementById(
                    "flowerResult"
                ).textContent =
                    flowersOpened +
                    " / 6 flowers opened";
                if (
                    flowersOpened === 6
                ) {
                    document.getElementById(
                        "flowerResult"
                    ).textContent =
                        "🌸 The whole garden has bloomed for Lola. 💙";
                    completeGame(6);
                    createConfetti();
                }
            }
        );
        flowers.appendChild(
            flower
        );
    }
);
/* =====================================================
   HAPPY BIRTHDAY MUSIC
===================================================== */
let audioContext = null;
const frequencies = {
    G4: 392.00,
    A4: 440.00,
    B4: 493.88,
    C5: 523.25,
    D5: 587.33,
    E5: 659.25,
    F5: 698.46,
    G5: 783.99
};
const birthdayNotes = [
    ["G4", .28],
    ["G4", .28],
    ["A4", .55],
    ["G4", .55],
    ["C5", .55],
    ["B4", .9],
    ["G4", .28],
    ["G4", .28],
    ["A4", .55],
    ["G4", .55],
    ["D5", .55],
    ["C5", .9],
    ["G4", .28],
    ["G4", .28],
    ["G5", .55],
    ["E5", .55],
    ["C5", .55],
    ["B4", .55],
    ["A4", .9],
    ["F5", .28],
    ["F5", .28],
    ["E5", .55],
    ["C5", .55],
    ["D5", .55],
    ["C5", 1.1]
];
function playHappyBirthday() {
    audioContext =
        new (
            window.AudioContext ||
            window.webkitAudioContext
        )();
    let time =
        audioContext.currentTime;
    birthdayNotes.forEach(
        ([note, duration]) => {
            const oscillator =
                audioContext.createOscillator();
            const gain =
                audioContext.createGain();
            oscillator.type =
                "sine";
            oscillator.frequency.value =
                frequencies[note];
            gain.gain.setValueAtTime(
                .0001,
                time
            );
            gain.gain.exponentialRampToValueAtTime(
                .22,
                time + .025
            );
            gain.gain.exponentialRampToValueAtTime(
                .0001,
                time + duration - .03
            );
            oscillator.connect(gain);
            gain.connect(
                audioContext.destination
            );
            oscillator.start(
                time
            );
            oscillator.stop(
                time + duration
            );
            time += duration;
        }
    );
    document.getElementById(
        "musicStatus"
    ).textContent =
        "🎶 Happy Birthday is playing...";
    setTimeout(
        () => {
            document.getElementById(
                "musicStatus"
            ).textContent =
                "💙 Happy birthday, Lola.";
        },
        10000
    );
}
document
    .getElementById(
        "musicButton"
    )
    .addEventListener(
        "click",
        playHappyBirthday
    );
/* =====================================================
   SECRET
===================================================== */
document
    .getElementById(
        "secretButton"
    )
    .addEventListener(
        "click",
        () => {
            document
                .getElementById(
                    "secret"
                )
                .classList.add(
                    "show"
                );
            createConfetti();
        }
    );
/* =====================================================
   CONFETTI
===================================================== */
function createConfetti() {
    const symbols = [
        "💙",
        "✨",
        "⭐",
        "🌸",
        "🎉",
        "💫"
    ];
    for (
        let i = 0;
        i < 45;
        i++
    ) {
        const piece =
            document.createElement(
                "div"
            );
        piece.className =
            "confetti";
        piece.textContent =
            symbols[
                Math.floor(
                    Math.random() *
                    symbols.length
                )
            ];
        piece.style.left =
            Math.random() * 100 + "vw";
        piece.style.fontSize =
            (10 +
            Math.random() * 17) +
            "px";
        piece.style.animationDuration =
            (2.5 +
            Math.random() * 2.5) +
            "s";
        piece.style.animationDelay =
            Math.random() * .7 +
            "s";
        document.body.appendChild(
            piece
        );
        setTimeout(
            () => piece.remove(),
            5500
        );
    }
}
/* =====================================================
   INITIAL LITTLE CELEBRATION
===================================================== */
window.addEventListener(
    "load",
    () => {
        setTimeout(
            () => {
                createConfetti();
            },
            1200
        );
    }
);
</script>
</body>
</html>
