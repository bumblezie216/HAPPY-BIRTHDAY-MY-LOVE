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
    font-family: Georgia, "Times New Roman", serif;
    color: #fffaf7;
    overflow-x: hidden;
    background:
        radial-gradient(circle at 50% 8%, rgba(255,226,184,.55), transparent 22%),
        linear-gradient(
            180deg,
            #536f9d 0%,
            #7088ad 20%,
            #9ba4bf 38%,
            #c09eac 55%,
            #d9aa9e 72%,
            #e8c39f 88%,
            #f1d8b2 100%
        );
}
/* =========================
   BACKGROUND
========================= */
.sky {
    position: fixed;
    inset: 0;
    z-index: -10;
    pointer-events: none;
    overflow: hidden;
}
.sun {
    position: absolute;
    width: 170px;
    height: 170px;
    border-radius: 50%;
    background: #ffe5b8;
    top: 8%;
    left: 50%;
    transform: translateX(-50%);
    box-shadow:
        0 0 35px rgba(255,225,174,.7),
        0 0 100px rgba(255,205,160,.35);
}
.sun::after {
    content: "";
    position: absolute;
    inset: -35px;
    border-radius: 50%;
    background: radial-gradient(circle, rgba(255,230,185,.25), transparent 65%);
}
.moon {
    position: absolute;
    width: 75px;
    height: 75px;
    right: 9%;
    top: 14%;
    border-radius: 50%;
    background: #fff6df;
    box-shadow: 0 0 25px rgba(255,247,225,.45);
    opacity: .75;
}
.moon::after {
    content: "";
    position: absolute;
    width: 75px;
    height: 75px;
    background: #7385aa;
    border-radius: 50%;
    left: 22px;
    top: -10px;
}
.star {
    position: absolute;
    color: rgba(255,255,255,.8);
    animation: twinkle 3s ease-in-out infinite;
    text-shadow: 0 0 10px rgba(255,255,255,.45);
}
@keyframes twinkle {
    0%,100% { opacity: .3; transform: scale(.8); }
    50% { opacity: 1; transform: scale(1.2); }
}
.s1 { left: 8%; top: 13%; animation-delay: .3s; }
.s2 { left: 19%; top: 29%; animation-delay: 1s; }
.s3 { right: 23%; top: 27%; animation-delay: 1.8s; }
.s4 { right: 7%; top: 38%; animation-delay: .7s; }
.s5 { left: 42%; top: 22%; animation-delay: 2.2s; }
.s6 { left: 5%; top: 47%; animation-delay: 1.3s; }
.s7 { right: 39%; top: 45%; animation-delay: .4s; }
.floating {
    position: fixed;
    bottom: -40px;
    pointer-events: none;
    opacity: .45;
    animation: floatUp linear forwards;
    z-index: 0;
}
@keyframes floatUp {
    from {
        transform: translateY(0) rotate(0deg);
        opacity: 0;
    }
    15% { opacity: .5; }
    to {
        transform: translateY(-115vh) rotate(360deg);
        opacity: 0;
    }
}
/* =========================
   LAYOUT
========================= */
.container {
    width: min(920px, 92%);
    margin: auto;
}
section {
    padding: 55px 0;
}
.card {
    background: rgba(255,248,244,.22);
    border: 1px solid rgba(255,255,255,.38);
    border-radius: 30px;
    padding: 30px;
    margin: 25px 0;
    backdrop-filter: blur(14px);
    -webkit-backdrop-filter: blur(14px);
    box-shadow: 0 15px 45px rgba(78,66,92,.12);
}
h1,
h2,
h3 {
    margin-top: 0;
}
h1 {
    font-size: clamp(3rem, 10vw, 6rem);
    line-height: .95;
    margin-bottom: 18px;
    text-shadow: 0 5px 25px rgba(88,69,91,.2);
}
h2 {
    font-size: clamp(2rem, 6vw, 3.2rem);
}
h3 {
    font-size: 1.45rem;
}
p {
    font-size: 1.08rem;
    line-height: 1.8;
}
/* =========================
   HERO
========================= */
.hero {
    min-height: 100vh;
    display: flex;
    align-items: center;
    text-align: center;
    padding: 50px 0;
}
.hero-content {
    width: 100%;
}
.eyebrow {
    letter-spacing: 3px;
    text-transform: uppercase;
    font-size: .8rem;
    opacity: .8;
}
.hero-subtitle {
    font-size: 1.35rem;
    max-width: 650px;
    margin: 25px auto;
}
.music-button {
    margin-top: 22px;
    font-size: 1.05rem;
    padding: 15px 25px;
    border-radius: 999px;
}
/* =========================
   BUTTONS
========================= */
button {
    border: none;
    cursor: pointer;
    font-family: inherit;
    color: #4d4960;
    background: linear-gradient(135deg, #dcecff, #f5d8df, #ffe2bd);
    padding: 14px 20px;
    border-radius: 18px;
    font-size: 1rem;
    transition: transform .2s ease, box-shadow .2s ease, opacity .2s ease;
    box-shadow: 0 8px 20px rgba(74,66,91,.13);
}
button:hover {
    transform: translateY(-3px);
    box-shadow: 0 12px 25px rgba(74,66,91,.18);
}
button:active {
    transform: scale(.96);
}
button:disabled {
    opacity: .5;
    cursor: default;
    transform: none;
}
.primary {
    background: linear-gradient(135deg, #cce7f5, #d9d5ed, #f3ccd2);
}
.small-note {
    font-size: .9rem;
    opacity: .75;
}
/* =========================
   LOVE LETTER
========================= */
.letter {
    max-width: 760px;
    margin: auto;
}
.letter p {
    font-size: 1.13rem;
}
/* =========================
   PROGRESS
========================= */
.progress-wrap {
    margin: 20px 0 35px;
}
.progress-text {
    text-align: center;
    margin-bottom: 10px;
    font-size: .95rem;
}
.progress-bar {
    height: 13px;
    border-radius: 999px;
    background: rgba(255,255,255,.25);
    overflow: hidden;
}
.progress-fill {
    width: 0%;
    height: 100%;
    border-radius: inherit;
    background: linear-gradient(90deg, #c9e8f5, #d9d5ec, #f4ced0, #f5d6ad);
    transition: width .7s ease;
}
/* =========================
   GAME CARDS
========================= */
.game {
    position: relative;
    overflow: hidden;
}
.game-number {
    display: inline-block;
    padding: 7px 13px;
    border-radius: 999px;
    background: rgba(255,255,255,.25);
    font-size: .8rem;
    letter-spacing: 1px;
    margin-bottom: 12px;
}
.game-complete {
    display: none;
    margin-top: 15px;
    font-size: 1rem;
}
.game-complete.show {
    display: block;
}
/* =========================
   GAME 1: PRESENTS
========================= */
.present-area {
    display: flex;
    justify-content: center;
    gap: 18px;
    flex-wrap: wrap;
    margin-top: 25px;
}
.present {
    font-size: 3.6rem;
    padding: 22px;
    min-width: 120px;
    background: rgba(255,255,255,.24);
}
.present.opened {
    animation: presentOpen .5s ease;
}
@keyframes presentOpen {
    0% { transform: scale(1); }
    50% { transform: scale(1.25) rotate(-7deg); }
    100% { transform: scale(1); }
}
.present-message {
    min-height: 55px;
    margin-top: 25px;
    font-size: 1.15rem;
}
/* =========================
   GAME 2: CAKE
========================= */
.cake {
    width: 220px;
    margin: 35px auto 20px;
    text-align: center;
    position: relative;
}
.cake-top {
    height: 65px;
    border-radius: 18px 18px 10px 10px;
    background: linear-gradient(#f8d9d9, #e9b8bf);
    position: relative;
}
.cake-bottom {
    height: 85px;
    border-radius: 10px 10px 25px 25px;
    background: linear-gradient(#f1c8c1, #dca7a8);
    margin-top: 6px;
}
.candle-row {
    position: absolute;
    top: -62px;
    left: 0;
    width: 100%;
    display: flex;
    justify-content: center;
    gap: 30px;
}
.candle {
    width: 14px;
    height: 50px;
    background: linear-gradient(#d9e9f7, #b7cde4);
    border-radius: 5px;
    position: relative;
    cursor: pointer;
}
.flame {
    position: absolute;
    width: 18px;
    height: 25px;
    background: #ffe4a9;
    border-radius: 50% 50% 50% 10%;
    transform: rotate(45deg);
    left: -2px;
    top: -23px;
    box-shadow: 0 0 15px #ffe4a9;
    transition: opacity .3s;
}
.flame.out {
    opacity: 0;
}
.cake-message {
    text-align: center;
    min-height: 30px;
}
/* =========================
   GAME 3: STARS
========================= */
.star-game {
    position: relative;
    height: 330px;
    border-radius: 25px;
    overflow: hidden;
    background:
        radial-gradient(circle at 20% 20%, rgba(255,255,255,.2), transparent 12%),
        linear-gradient(160deg, rgba(51,72,108,.55), rgba(111,102,138,.45), rgba(191,145,157,.5));
    border: 1px solid rgba(255,255,255,.25);
}
.catch-star {
    position: absolute;
    font-size: 2rem;
    padding: 7px;
    background: transparent;
    box-shadow: none;
    text-shadow: 0 0 15px rgba(255,255,255,.8);
}
.catch-star:hover {
    box-shadow: none;
    transform: scale(1.25);
}
.star-score {
    text-align: center;
    margin: 18px 0;
    font-size: 1.15rem;
}
/* =========================
   GAME 4: QUIZ
========================= */
.quiz-question {
    display: none;
}
.quiz-question.active {
    display: block;
    animation: fadeIn .35s ease;
}
@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(8px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}
.quiz-options {
    display: grid;
    gap: 12px;
    margin-top: 20px;
}
.quiz-option {
    width: 100%;
    text-align: left;
    background: rgba(255,255,255,.27);
    color: #fff;
    border: 1px solid rgba(255,255,255,.28);
}
.quiz-option.correct {
    background: rgba(183,225,208,.65);
    color: #394f49;
}
.quiz-option.wrong {
    background: rgba(239,186,190,.65);
    color: #5d4146;
}
.quiz-feedback {
    min-height: 35px;
    margin-top: 18px;
}
.quiz-next {
    margin-top: 10px;
}
.quiz-score {
    text-align: center;
    font-size: 1.3rem;
    margin-top: 20px;
}
/* =========================
   GAME 5: OTTER OCEAN
========================= */
.ocean {
    position: relative;
    height: 300px;
    border-radius: 28px;
    overflow: hidden;
    background:
        linear-gradient(
            180deg,
            rgba(177,218,231,.8),
            rgba(113,171,194,.8),
            rgba(75,132,159,.9)
        );
    border: 1px solid rgba(255,255,255,.3);
}
.wave {
    position: absolute;
    width: 150%;
    height: 80px;
    left: -25%;
    bottom: -30px;
    border-radius: 50% 50% 0 0;
    background: rgba(220,243,247,.25);
    animation: waveMove 5s ease-in-out infinite;
}
.wave.two {
    bottom: 5px;
    animation-delay: -2s;
    opacity: .55;
}
@keyframes waveMove {
    0%,100% { transform: translateX(-3%); }
    50% { transform: translateX(3%); }
}
.otter {
    position: absolute;
    font-size: 3rem;
    padding: 8px;
    background: transparent;
    box-shadow: none;
    transition: left .5s ease, top .5s ease, transform .3s ease;
}
.otter:hover {
    box-shadow: none;
    transform: scale(1.2) rotate(-5deg);
}
.ocean-message {
    min-height: 35px;
    text-align: center;
    margin-top: 18px;
}
/* =========================
   GAME 6: FLOWERS
========================= */
.flower-garden {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 15px;
    margin-top: 25px;
}
.flower {
    min-height: 100px;
    font-size: 2.6rem;
    background: rgba(255,255,255,.2);
}
.flower-text {
    text-align: center;
    min-height: 60px;
    margin-top: 20px;
}
/* =========================
   FINAL
========================= */
.final {
    text-align: center;
    padding: 100px 0 120px;
}
.secret-button {
    font-size: 1.15rem;
    padding: 18px 28px;
}
.secret-letter {
    display: none;
    margin-top: 30px;
    animation: fadeIn .8s ease;
}
.secret-letter.show {
    display: block;
}
.signature {
    font-size: 1.4rem;
    margin-top: 30px;
}
/* =========================
   CONFETTI
========================= */
.confetti {
    position: fixed;
    top: -30px;
    z-index: 50;
    pointer-events: none;
    animation: confettiFall 4s linear forwards;
}
@keyframes confettiFall {
    to {
        transform: translateY(115vh) rotate(720deg);
        opacity: 0;
    }
}
/* =========================
   MOBILE
========================= */
@media (max-width: 650px) {
    section {
        padding: 40px 0;
    }
    .card {
        padding: 22px;
        border-radius: 24px;
    }
    .sun {
        width: 125px;
        height: 125px;
    }
    .flower-garden {
        grid-template-columns: repeat(2, 1fr);
    }
    .present {
        min-width: 95px;
        font-size: 2.8rem;
        padding: 17px;
    }
    .star-game {
        height: 290px;
    }
    .ocean {
        height: 270px;
    }
}
@media (prefers-reduced-motion: reduce) {
    *,
    *::before,
    *::after {
        animation-duration: .01ms !important;
        animation-iteration-count: 1 !important;
        scroll-behavior: auto !important;
    }
}
</style>
</head>
<body>
<div class="sky">
    <div class="sun"></div>
    <div class="moon"></div>
    <span class="star s1">✦</span>
    <span class="star s2">✧</span>
    <span class="star s3">✦</span>
    <span class="star s4">⋆</span>
    <span class="star s5">✧</span>
    <span class="star s6">✦</span>
    <span class="star s7">⋆</span>
</div>
<main class="container">
<!-- =========================
     HERO
========================= -->
<section class="hero">
    <div class="hero-content">
        <div class="eyebrow">
            A little birthday universe
        </div>
        <h1>
            Happy Birthday<br>
            Lola 💙
        </h1>
        <p class="hero-subtitle">
            Today the sky feels a little softer,
            the stars feel a little brighter,
            and the universe has one very important
            reason to celebrate.
            <br><br>
            <strong>You.</strong> 🌅
        </p>
        <!-- MUSIC BUTTON IS NOW AT THE TOP -->
        <button class="music-button primary" id="musicButton">
            🎵 Play Happy Birthday
        </button>
        <p class="small-note">
            Tap the button when you're ready for your birthday song.
        </p>
        <br>
        <button id="beginButton">
            🎁 Begin Your Birthday Adventure
        </button>
    </div>
</section>
<!-- =========================
     LOVE LETTER
========================= -->
<section>
    <div class="card letter">
        <div class="eyebrow">
            From Bree / Putiputi
        </div>
        <h2>
            For my Lola 💙
        </h2>
        <p>
            If I could give you anything for your birthday,
            I would give you a sky full of sunsets,
            a peaceful ocean,
            every star in the universe,
            and every quiet moment that makes you feel safe.
        </p>
        <p>
            Since I cannot put the whole universe inside a birthday box,
            I made you a tiny piece of one instead.
        </p>
        <p>
            So this little world is yours.
            Explore it, play the games,
            find the surprises,
            and most importantly...
            remember how incredibly loved you are.
        </p>
        <p>
            Happy 27th birthday, my love. 🌸
        </p>
    </div>
</section>
<!-- =========================
     PROGRESS
========================= -->
<section id="games">
    <div class="card">
        <h2>
            Your Birthday Adventure ✨
        </h2>
        <p>
            Six little challenges are waiting for you.
            Complete them all to unlock your final surprise.
        </p>
        <div class="progress-wrap">
            <div class="progress-text" id="progressText">
                0 / 6 birthday games completed
            </div>
            <div class="progress-bar">
                <div class="progress-fill" id="progressFill"></div>
            </div>
        </div>
    </div>
<!-- =========================
     GAME 1
========================= -->
<div class="card game" id="game1">
    <span class="game-number">
        GAME ONE
    </span>
    <h2>
        Pick Your Present 🎁
    </h2>
    <p>
        Three mysterious presents have appeared.
        Only one message can be opened from each.
        Pick whichever one calls to you.
    </p>
    <div class="present-area">
        <button class="present" data-message="A little reminder that no matter how far apart we are, you always have a home in my heart. 💙">
            🎁
        </button>
        <button class="present" data-message="If I could wrap up one thing for you, it would be every beautiful sunset you have yet to see. 🌅">
            🎁
        </button>
        <button class="present" data-message="Secret birthday truth: you are one of my favourite people in this entire universe. ⭐">
            🎁
        </button>
    </div>
    <div class="present-message" id="presentMessage">
        Choose a present...
    </div>
    <div class="game-complete" id="complete1">
        ✨ Present opened! Game One complete.
    </div>
</div>
<!-- =========================
     GAME 2
========================= -->
<div class="card game" id="game2">
    <span class="game-number">
        GAME TWO
    </span>
    <h2>
        Make a Birthday Wish 🎂
    </h2>
    <p>
        Three candles are waiting.
        Tap each flame to blow it out.
        When they're all gone, your birthday wish appears.
    </p>
    <div class="cake">
        <div class="candle-row">
            <div class="candle">
                <div class="flame"></div>
            </div>
            <div class="candle">
                <div class="flame"></div>
            </div>
            <div class="candle">
                <div class="flame"></div>
            </div>
        </div>
        <div class="cake-top"></div>
        <div class="cake-bottom"></div>
    </div>
    <div class="cake-message" id="cakeMessage">
        3 candles still glowing ✨
    </div>
    <div class="game-complete" id="complete2">
        🌟 Wish made! Game Two complete.
    </div>
</div>
<!-- =========================
     GAME 3
========================= -->
<div class="card game" id="game3">
    <span class="game-number">
        GAME THREE
    </span>
    <h2>
        Catch the Stars ⭐
    </h2>
    <p>
        Five stars are hiding in the evening sky.
        Tap them before they disappear!
    </p>
    <div class="star-score" id="starScore">
        Stars collected: 0 / 5
    </div>
    <div class="star-game" id="starGame"></div>
    <div class="game-complete" id="complete3">
        🌟 You caught every star! Game Three complete.
    </div>
</div>
<!-- =========================
     GAME 4
========================= -->
<div class="card game" id="game4">
    <span class="game-number">
        GAME FOUR
    </span>
    <h2>
        How Well Do You Know Lola? 💙
    </h2>
    <p>
        Ten questions.
        No cheating.
        Let's see how closely you've been paying attention. 👀
    </p>
    <div id="quiz">
        <!-- Q1 -->
        <div class="quiz-question active">
            <h3>
                1. What is Lola's favourite colour?
            </h3>
            <div class="quiz-options">
                <button class="quiz-option" data-correct="true">
                    Baby blue
                </button>
                <button class="quiz-option">
                    Burgundy
                </button>
                <button class="quiz-option">
                    Bright red
                </button>
                <button class="quiz-option">
                    Emerald green
                </button>
            </div>
        </div>
        <!-- Q2 -->
        <div class="quiz-question">
            <h3>
                2. Which animal does Lola love?
            </h3>
            <div class="quiz-options">
                <button class="quiz-option">
                    Penguins
                </button>
                <button class="quiz-option" data-correct="true">
                    Otters
                </button>
                <button class="quiz-option">
                    Dolphins
                </button>
                <button class="quiz-option">
                    Foxes
                </button>
            </div>
        </div>
        <!-- Q3 -->
        <div class="quiz-question">
            <h3>
                3. What does Lola like to drink?
            </h3>
            <div class="quiz-options">
                <button class="quiz-option">
                    Hot chocolate
                </button>
                <button class="quiz-option">
                    Green tea
                </button>
                <button class="quiz-option" data-correct="true">
                    Black coffee
                </button>
                <button class="quiz-option">
                    Lemonade
                </button>
            </div>
        </div>
        <!-- Q4 -->
        <div class="quiz-question">
            <h3>
                4. Which food does Lola love?
            </h3>
            <div class="quiz-options">
                <button class="quiz-option">
                    Pizza
                </button>
                <button class="quiz-option" data-correct="true">
                    Sushi
                </button>
                <button class="quiz-option">
                    Tacos
                </button>
                <button class="quiz-option">
                    Burgers
                </button>
            </div>
        </div>
        <!-- Q5 -->
        <div class="quiz-question">
            <h3>
                5. What does Lola want to see someday?
            </h3>
            <div class="quiz-options">
                <button class="quiz-option">
                    A desert
                </button>
                <button class="quiz-option">
                    A volcano
                </button>
                <button class="quiz-option" data-correct="true">
                    The ocean
                </button>
                <button class="quiz-option">
                    A rainforest
                </button>
            </div>
        </div>
        <!-- Q6 -->
        <div class="quiz-question">
            <h3>
                6. What is something Lola is known for being like during chaos?
            </h3>
            <div class="quiz-options">
                <button class="quiz-option" data-correct="true">
                    Calm
                </button>
                <button class="quiz-option">
                    Loud
                </button>
                <button class="quiz-option">
                    Easily distracted
                </button>
                <button class="quiz-option">
                    Dramatic
                </button>
            </div>
        </div>
        <!-- Q7 -->
        <div class="quiz-question">
            <h3>
                7. What kind of coffee does Lola like?
            </h3>
            <div class="quiz-options">
                <button class="quiz-option">
                    Sweet iced coffee
                </button>
                <button class="quiz-option">
                    Cappuccino
                </button>
                <button class="quiz-option">
                    Vanilla latte
                </button>
                <button class="quiz-option" data-correct="true">
                    Black coffee
                </button>
            </div>
        </div>
        <!-- Q8 -->
        <div class="quiz-question">
            <h3>
                8. Which creature appears in Lola's birthday universe?
            </h3>
            <div class="quiz-options">
                <button class="quiz-option">
                    🐺 Wolf
                </button>
                <button class="quiz-option" data-correct="true">
                    🦦 Otter
                </button>
                <button class="quiz-option">
                    🦊 Fox
                </button>
                <button class="quiz-option">
                    🐼 Panda
                </button>
            </div>
        </div>
        <!-- Q9 -->
        <div class="quiz-question">
            <h3>
                9. What is Lola turning?
            </h3>
            <div class="quiz-options">
                <button class="quiz-option">
                    25
                </button>
                <button class="quiz-option">
                    26
                </button>
                <button class="quiz-option" data-correct="true">
                    27
                </button>
                <button class="quiz-option">
                    28
                </button>
            </div>
        </div>
        <!-- Q10 -->
        <div class="quiz-question">
            <h3>
                10. What colour belongs to Lola's birthday universe?
            </h3>
            <div class="quiz-options">
                <button class="quiz-option">
                    Neon yellow
                </button>
                <button class="quiz-option">
                    Bright orange
                </button>
                <button class="quiz-option" data-correct="true">
                    Soft baby blue
                </button>
                <button class="quiz-option">
                    Fluorescent green
                </button>
            </div>
        </div>
        <div class="quiz-feedback" id="quizFeedback"></div>
        <button class="quiz-next" id="quizNext" style="display:none;">
            Next question →
        </button>
        <div class="quiz-score" id="quizScore"></div>
    </div>
    <div class="game-complete" id="complete4">
        💙 You survived the Lola quiz! Game Four complete.
    </div>
</div>
<!-- =========================
     GAME 5
========================= -->
<div class="card game" id="game5">
    <span class="game-number">
        GAME FIVE
    </span>
    <h2>
        Find Lola's Otter 🦦
    </h2>
    <p>
        Something is hiding beneath the waves.
        Tap the ocean until you find it.
    </p>
    <div class="ocean" id="ocean">
        <div class="wave"></div>
        <div class="wave two"></div>
        <button class="otter" id="otter">
            🦦
        </button>
    </div>
    <div class="ocean-message" id="oceanMessage">
        Where could the little otter be? 🌊
    </div>
    <div class="game-complete" id="complete5">
        🦦 You found the otter! Game Five complete.
    </div>
</div>
<!-- =========================
     GAME 6
========================= -->
<div class="card game" id="game6">
    <span class="game-number">
        GAME SIX
    </span>
    <h2>
        Make the Garden Bloom 🌸
    </h2>
    <p>
        Six flowers are waiting to bloom.
        Tap each one to reveal a little reason
        why Lola is loved.
    </p>
    <div class="flower-garden">
        <button class="flower" data-reason="Because your presence makes ordinary moments feel special. 💙">
            🌱
        </button>
        <button class="flower" data-reason="Because there is something incredibly comforting about you. 🌸">
            🌱
        </button>
        <button class="flower" data-reason="Because you have a way of making someone feel at home. 🏡">
            🌱
        </button>
        <button class="flower" data-reason="Because your smile deserves its own constellation. ⭐">
            🌱
        </button>
        <button class="flower" data-reason="Because you are one of the most precious parts of my universe. 🌌">
            🌱
        </button>
        <button class="flower" data-reason="Because loving you feels like finding a little piece of peace in a very noisy world. 💙">
            🌱
        </button>
    </div>
    <div class="flower-text" id="flowerText">
        Your garden is waiting...
    </div>
    <div class="game-complete" id="complete6">
        🌸 The whole garden is blooming! Game Six complete.
    </div>
</div>
</section>
<!-- =========================
     FINAL SURPRISE
========================= -->
<section class="final">
    <h2>
        You made it. 💙
    </h2>
    <p>
        Six games.
        Ten Lola questions.
        One very special birthday girl.
    </p>
    <button class="secret-button" id="secretButton">
        💙 Open Your Final Surprise
    </button>
    <div class="card secret-letter" id="secretLetter">
        <h2>
            Happy 27th Birthday, my love. 🌅
        </h2>
        <p>
            I hope this next chapter brings you softer mornings,
            beautiful sunsets,
            peaceful nights,
            oceans you finally get to see,
            and so many little moments that make you smile.
        </p>
        <p>
            I wish I could give you the whole sky,
            but somehow our paths crossed,
            and I ended up finding something even more precious.
        </p>
        <p>
            You.
        </p>
        <p>
            So whenever you look at the stars,
            I hope you remember that somewhere in this enormous universe,
            there is a girl who loves you more than words can properly explain.
        </p>
        <p>
            You are my favourite little piece of the universe.
            ⭐🌊🌸💙
        </p>
        <p class="signature">
            With all my love,<br>
            Bree / Putiputi 💙
        </p>
    </div>
</section>
</main>
<script>
/* =========================
   BASIC STATE
========================= */
let completedGames = new Set();
function completeGame(number) {
    if (completedGames.has(number)) return;
    completedGames.add(number);
    const complete = document.getElementById("complete" + number);
    if (complete) {
        complete.classList.add("show");
    }
    updateProgress();
    if (completedGames.size === 6) {
        createConfetti(80);
    }
}
function updateProgress() {
    const count = completedGames.size;
    const percentage = (count / 6) * 100;
    document.getElementById("progressText").textContent =
        count + " / 6 birthday games completed";
    document.getElementById("progressFill").style.width =
        percentage + "%";
}
/* =========================
   HAPPY BIRTHDAY AUDIO
========================= */
let audioContext = null;
let musicPlaying = false;
const notes = {
    G4: 392.00,
    A4: 440.00,
    B4: 493.88,
    C5: 523.25,
    D5: 587.33,
    E5: 659.25,
    F5: 698.46,
    G5: 783.99
};
const melody = [
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
function playNote(frequency, startTime, duration) {
    if (!audioContext) return;
    const oscillator = audioContext.createOscillator();
    const gain = audioContext.createGain();
    oscillator.type = "sine";
    oscillator.frequency.value = frequency;
    gain.gain.setValueAtTime(0.0001, startTime);
    gain.gain.exponentialRampToValueAtTime(0.13, startTime + 0.025);
    gain.gain.exponentialRampToValueAtTime(
        0.0001,
        startTime + duration
    );
    oscillator.connect(gain);
    gain.connect(audioContext.destination);
    oscillator.start(startTime);
    oscillator.stop(startTime + duration + .03);
}
function playBirthdaySong() {
    if (!audioContext) {
        audioContext = new (
            window.AudioContext ||
            window.webkitAudioContext
        )();
    }
    if (audioContext.state === "suspended") {
        audioContext.resume();
    }
    const now = audioContext.currentTime + .1;
    let time = now;
    melody.forEach(([note, duration]) => {
        playNote(
            notes[note],
            time,
            duration * .9
        );
        time += duration;
    });
    musicPlaying = true;
    document.getElementById("musicButton").textContent =
        "🎵 Happy Birthday is playing!";
    setTimeout(() => {
        musicPlaying = false;
        document.getElementById("musicButton").textContent =
            "🎵 Play Happy Birthday Again";
    }, (time - now) * 1000 + 300);
}
document.getElementById("musicButton").addEventListener(
    "click",
    playBirthdaySong
);
/* =========================
   BEGIN BUTTON
   ALSO STARTS MUSIC
========================= */
document.getElementById("beginButton").addEventListener(
    "click",
    () => {
        if (!musicPlaying) {
            playBirthdaySong();
        }
        document.getElementById("games").scrollIntoView({
            behavior: "smooth"
        });
    }
);
/* =========================
   GAME 1: PRESENTS
========================= */
const presents = document.querySelectorAll(".present");
const presentMessage = document.getElementById("presentMessage");
presents.forEach(present => {
    present.addEventListener("click", () => {
        presents.forEach(item => {
            item.classList.remove("opened");
        });
        present.classList.add("opened");
        presentMessage.textContent =
            present.dataset.message;
        completeGame(1);
        createConfetti(15);
    });
});
/* =========================
   GAME 2: CANDLES
========================= */
const flames = document.querySelectorAll(".flame");
const cakeMessage = document.getElementById("cakeMessage");
flames.forEach(flame => {
    flame.addEventListener("click", () => {
        if (flame.classList.contains("out")) return;
        flame.classList.add("out");
        const remaining =
            document.querySelectorAll(".flame:not(.out)").length;
        if (remaining > 0) {
            cakeMessage.textContent =
                remaining + " candle" +
                (remaining === 1 ? "" : "s") +
                " still glowing ✨";
        } else {
            cakeMessage.textContent =
                "Make your biggest birthday wish... 🌟";
            completeGame(2);
            createConfetti(30);
        }
    });
});
/* =========================
   GAME 3: CATCH STARS
========================= */
const starGame = document.getElementById("starGame");
const starScore = document.getElementById("starScore");
let starsCollected = 0;
function createStar() {
    const star = document.createElement("button");
    star.className = "catch-star";
    star.type = "button";
    star.textContent = "⭐";
    star.setAttribute("aria-label", "Catch star");
    const maxX = Math.max(10, starGame.clientWidth - 55);
    const maxY = Math.max(10, starGame.clientHeight - 60);
    star.style.left =
        Math.random() * maxX + "px";
    star.style.top =
        Math.random() * maxY + "px";
    star.addEventListener("click", () => {
        if (star.dataset.caught) return;
        star.dataset.caught = "true";
        starsCollected++;
        star.remove();
        starScore.textContent =
            "Stars collected: " +
            starsCollected +
            " / 5";
        createConfetti(5);
        if (starsCollected >= 5) {
            completeGame(3);
            starScore.textContent =
                "✨ All five stars collected! ✨";
        }
    });
    starGame.appendChild(star);
}
for (let i = 0; i < 5; i++) {
    createStar();
}
/* =========================
   GAME 4: QUIZ
========================= */
const quizQuestions =
    document.querySelectorAll(".quiz-question");
const quizFeedback =
    document.getElementById("quizFeedback");
const quizNext =
    document.getElementById("quizNext");
const quizScore =
    document.getElementById("quizScore");
let currentQuestion = 0;
let quizPoints = 0;
let answeredCurrent = false;
quizQuestions.forEach((question, questionIndex) => {
    const options =
        question.querySelectorAll(".quiz-option");
    options.forEach(option => {
        option.addEventListener("click", () => {
            if (answeredCurrent) return;
            answeredCurrent = true;
            const isCorrect =
                option.dataset.correct === "true";
            options.forEach(item => {
                item.disabled = true;
                if (item.dataset.correct === "true") {
                    item.classList.add("correct");
                }
            });
            if (isCorrect) {
                quizPoints++;
                option.classList.add("correct");
                quizFeedback.textContent =
                    "You got it! 💙";
                createConfetti(7);
            } else {
                option.classList.add("wrong");
                quizFeedback.textContent =
                    "Not quite! The correct answer is highlighted above. 🌸";
            }
            if (questionIndex < quizQuestions.length - 1) {
                quizNext.style.display = "inline-block";
            } else {
                quizScore.textContent =
                    "You scored " +
                    quizPoints +
                    " / 10 💙";
                completeGame(4);
                createConfetti(25);
            }
        });
    });
});
quizNext.addEventListener("click", () => {
    quizQuestions[currentQuestion]
        .classList.remove("active");
    currentQuestion++;
    quizQuestions[currentQuestion]
        .classList.add("active");
    quizFeedback.textContent = "";
    quizNext.style.display = "none";
    answeredCurrent = false;
});
/* =========================
   GAME 5: OTTER
========================= */
const ocean = document.getElementById("ocean");
const otter = document.getElementById("otter");
const oceanMessage = document.getElementById("oceanMessage");
function moveOtter() {
    const maxX =
        Math.max(20, ocean.clientWidth - 65);
    const maxY =
        Math.max(20, ocean.clientHeight - 75);
    otter.style.left =
        Math.random() * maxX + "px";
    otter.style.top =
        Math.random() * maxY + "px";
}
moveOtter();
otter.addEventListener("click", () => {
    oceanMessage.textContent =
        "You found Lola's little ocean friend! 🦦💙";
    completeGame(5);
    createConfetti(18);
});
/* =========================
   GAME 6: FLOWERS
========================= */
const flowers =
    document.querySelectorAll(".flower");
const flowerText =
    document.getElementById("flowerText");
let flowersOpened = 0;
flowers.forEach(flower => {
    flower.addEventListener("click", () => {
        if (flower.dataset.opened) return;
        flower.dataset.opened = "true";
        flowersOpened++;
        flower.textContent = "🌸";
        flowerText.textContent =
            flower.dataset.reason;
        flower.style.transform =
            "scale(1.08)";
        createConfetti(4);
        if (flowersOpened >= flowers.length) {
            completeGame(6);
            flowerText.textContent =
                "🌸 The whole garden is blooming because of you. 💙";
            createConfetti(30);
        }
    });
});
/* =========================
   FINAL SURPRISE
========================= */
const secretButton =
    document.getElementById("secretButton");
const secretLetter =
    document.getElementById("secretLetter");
secretButton.addEventListener("click", () => {
    if (completedGames.size < 6) {
        secretButton.textContent =
            "✨ Complete all six games first!";
        setTimeout(() => {
            secretButton.textContent =
                "💙 Open Your Final Surprise";
        }, 2500);
        return;
    }
    secretLetter.classList.add("show");
    secretButton.textContent =
        "🌸 Your surprise is open";
    createConfetti(70);
    secretLetter.scrollIntoView({
        behavior: "smooth",
        block: "center"
    });
});
/* =========================
   FLOATING DECORATIONS
========================= */
const floatingSymbols = [
    "💙",
    "✨",
    "⭐",
    "🌸",
    "🦋",
    "🌊"
];
function createFloatingSymbol() {
    const element =
        document.createElement("div");
    element.className = "floating";
    element.textContent =
        floatingSymbols[
            Math.floor(
                Math.random() *
                floatingSymbols.length
            )
        ];
    element.style.left =
        Math.random() * 100 + "%";
    element.style.fontSize =
        (12 + Math.random() * 15) + "px";
    element.style.animationDuration =
        (8 + Math.random() * 8) + "s";
    document.body.appendChild(element);
    setTimeout(() => {
        element.remove();
    }, 17000);
}
setInterval(createFloatingSymbol, 1300);
/* =========================
   CONFETTI
========================= */
function createConfetti(amount) {
    const symbols = [
        "💙",
        "✨",
        "⭐",
        "🌸",
        "🦋",
        "🌊"
    ];
    for (let i = 0; i < amount; i++) {
        const piece =
            document.createElement("div");
        piece.className = "confetti";
        piece.textContent =
            symbols[
                Math.floor(
                    Math.random() *
                    symbols.length
                )
            ];
        piece.style.left =
            Math.random() * 100 + "%";
        piece.style.fontSize =
            (12 + Math.random() * 18) + "px";
        piece.style.animationDuration =
            (2.5 + Math.random() * 2.5) + "s";
        piece.style.animationDelay =
            Math.random() * .7 + "s";
        document.body.appendChild(piece);
        setTimeout(() => {
            piece.remove();
        }, 6000);
    }
}
</script>
</body>
</html>
