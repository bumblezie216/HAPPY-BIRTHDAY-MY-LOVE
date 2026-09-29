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
    color: white;
    background:
        linear-gradient(
            180deg,
            #17135c 0%,
            #403b91 18%,
            #7770bd 35%,
            #e5829d 55%,
            #ffae7d 72%,
            #ffd69b 100%
        );
}
/* =========================
   BACKGROUND
========================= */
.sky {
    position: fixed;
    inset: 0;
    overflow: hidden;
    pointer-events: none;
    z-index: 0;
}
/* Moon */
.moon {
    position: absolute;
    width: 90px;
    height: 90px;
    right: 12%;
    top: 9%;
    border-radius: 50%;
    background: #fff7d6;
    box-shadow:
        0 0 25px #fff4c7,
        0 0 70px rgba(255, 225, 170, 0.8);
}
/* Sun */
.sun {
    position: absolute;
    width: 210px;
    height: 210px;
    left: 50%;
    top: 63%;
    transform: translate(-50%, -50%);
    border-radius: 50%;
    background: #fff1b5;
    box-shadow:
        0 0 40px #ffe6a3,
        0 0 100px #ffb36d,
        0 0 180px #ff8c80;
    opacity: 0.7;
}
/* Stars */
.star {
    position: absolute;
    width: 3px;
    height: 3px;
    background: white;
    border-radius: 50%;
    box-shadow: 0 0 8px white;
    animation: twinkle 2s infinite alternate;
}
@keyframes twinkle {
    from {
        opacity: 0.2;
        transform: scale(0.6);
    }
    to {
        opacity: 1;
        transform: scale(1.5);
    }
}
/* =========================
   FLOATING ELEMENTS
========================= */
.floating {
    position: fixed;
    bottom: -50px;
    pointer-events: none;
    z-index: 10;
    animation: floatUp linear forwards;
}
@keyframes floatUp {
    0% {
        transform:
            translateY(0)
            rotate(0deg);
        opacity: 0;
    }
    10% {
        opacity: 1;
    }
    100% {
        transform:
            translateY(-115vh)
            rotate(360deg);
        opacity: 0;
    }
}
/* =========================
   CONTENT
========================= */
main {
    position: relative;
    z-index: 2;
    min-height: 100vh;
    padding:
        70px
        20px
        120px;
    text-align: center;
}
/* =========================
   OPENING
========================= */
.intro {
    min-height: 85vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
.eyebrow {
    margin-bottom: 18px;
    font-size: 14px;
    letter-spacing: 5px;
    text-transform: uppercase;
    opacity: 0.85;
    animation: fadeIn 2s ease;
}
h1 {
    margin: 0;
    font-size:
        clamp(48px, 12vw, 105px);
    line-height: 0.9;
    text-shadow:
        0 5px 25px rgba(50, 20, 80, 0.25);
    animation:
        titleAppear 1.8s ease;
}
.name {
    display: block;
    color: #dff8ff;
    font-style: italic;
    text-shadow:
        0 0 20px rgba(210, 250, 255, 0.5);
}
.intro-text {
    max-width: 650px;
    margin:
        30px
        auto
        0;
    font-size:
        clamp(18px, 4vw, 24px);
    line-height: 1.7;
    opacity: 0;
    animation:
        fadeIn 2s ease 0.8s forwards;
}
.scroll {
    margin-top: 50px;
    font-size: 13px;
    letter-spacing: 3px;
    opacity: 0.75;
    animation:
        bounce 2s infinite;
}
@keyframes titleAppear {
    from {
        opacity: 0;
        transform:
            translateY(30px)
            scale(0.9);
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
    0%, 100% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(10px);
    }
}
/* =========================
   GLASS CARDS
========================= */
.card {
    width: min(92vw, 720px);
    margin:
        45px
        auto;
    padding:
        40px
        28px;
    border-radius: 32px;
    background:
        rgba(255,255,255,0.16);
    border:
        1px solid
        rgba(255,255,255,0.35);
    backdrop-filter:
        blur(16px);
    box-shadow:
        0 25px 60px
        rgba(45, 20, 80, 0.22);
    transition:
        transform 0.5s ease,
        background 0.5s ease;
    animation:
        cardFloat 6s ease-in-out infinite;
}
.card:nth-child(even) {
    animation-delay: 1s;
}
.card:hover {
    transform:
        translateY(-8px)
        scale(1.01);
    background:
        rgba(255,255,255,0.22);
}
@keyframes cardFloat {
    0%, 100% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(-5px);
    }
}
.card h2 {
    margin-top: 0;
    font-size:
        clamp(28px, 6vw, 38px);
    color: #e8fbff;
    text-shadow:
        0 0 15px rgba(210,245,255,0.4);
}
.card p {
    font-size: 18px;
    line-height: 1.9;
    margin-bottom: 0;
}
/* =========================
   FAVOURITE THINGS
========================= */
.favourites {
    display: grid;
    grid-template-columns:
        repeat(
            auto-fit,
            minmax(130px, 1fr)
        );
    gap: 18px;
    margin-top: 30px;
}
.favourite {
    padding: 22px 10px;
    border-radius: 22px;
    background:
        rgba(255,255,255,0.13);
    border:
        1px solid
        rgba(255,255,255,0.25);
    transition:
        transform 0.3s ease;
}
.favourite:hover {
    transform:
        translateY(-8px)
        rotate(-2deg);
}
.favourite-icon {
    display: block;
    font-size: 35px;
    margin-bottom: 10px;
}
.favourite-text {
    font-size: 15px;
}
/* =========================
   BIG BIRTHDAY MESSAGE
========================= */
.big-message {
    font-size:
        clamp(30px, 7vw, 55px);
    line-height: 1.25;
    color: #fff5d7;
    text-shadow:
        0 4px 20px rgba(80,30,60,0.25);
}
/* =========================
   BUTTON
========================= */
button {
    margin-top: 30px;
    padding:
        16px
        30px;
    border: none;
    border-radius: 50px;
    background:
        #fff3d3;
    color:
        #44316e;
    font-family:
        Georgia,
        "Times New Roman",
        serif;
    font-size: 17px;
    cursor: pointer;
    box-shadow:
        0 10px 30px
        rgba(50,30,80,0.25);
    transition:
        transform 0.3s ease,
        box-shadow 0.3s ease;
}
button:hover {
    transform:
        scale(1.08);
    box-shadow:
        0 15px 40px
        rgba(50,30,80,0.35);
}
/* =========================
   SECRET MESSAGE
========================= */
.secret {
    display: none;
    margin-top: 30px;
    font-size: 20px;
    line-height: 1.8;
    animation:
        fadeIn 1s ease;
}
.secret.show {
    display: block;
}
/* =========================
   FINAL
========================= */
.final {
    min-height: 60vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
.final-heart {
    font-size: 65px;
    animation:
        heartbeat 1.5s infinite;
}
@keyframes heartbeat {
    0%, 100% {
        transform: scale(1);
    }
    50% {
        transform: scale(1.18);
    }
}
.signature {
    margin-top: 30px;
    font-size: 22px;
    font-style: italic;
    color: #e6faff;
}
/* =========================
   CONFETTI
========================= */
.confetti {
    position: fixed;
    width: 9px;
    height: 14px;
    top: -20px;
    z-index: 100;
    pointer-events: none;
    animation:
        confettiFall 3s linear forwards;
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
            rotate(720deg);
        opacity: 0;
    }
}
/* =========================
   MOBILE
========================= */
@media (max-width: 600px) {
    main {
        padding:
            40px
            15px
            80px;
    }
    .card {
        padding:
            32px
            20px;
    }
    .card p {
        font-size: 17px;
    }
    .sun {
        width: 160px;
        height: 160px;
    }
    .moon {
        width: 60px;
        height: 60px;
    }
}
</style>
</head>
<body>
<div class="sky">
    <div class="sun"></div>
    <div class="moon"></div>
    <!-- STARS -->
    <div class="star" style="left:8%; top:8%; animation-delay:.2s;"></div>
    <div class="star" style="left:18%; top:18%; animation-delay:1s;"></div>
    <div class="star" style="left:30%; top:7%; animation-delay:.5s;"></div>
    <div class="star" style="left:42%; top:16%; animation-delay:1.4s;"></div>
    <div class="star" style="left:54%; top:6%; animation-delay:.7s;"></div>
    <div class="star" style="left:68%; top:18%; animation-delay:1.2s;"></div>
    <div class="star" style="left:80%; top:7%; animation-delay:.3s;"></div>
    <div class="star" style="left:91%; top:23%; animation-delay:1.6s;"></div>
    <div class="star" style="left:12%; top:30%; animation-delay:.8s;"></div>
    <div class="star" style="left:25%; top:25%; animation-delay:1.1s;"></div>
    <div class="star" style="left:48%; top:29%; animation-delay:.4s;"></div>
    <div class="star" style="left:62%; top:31%; animation-delay:1.7s;"></div>
    <div class="star" style="left:74%; top:27%; animation-delay:.9s;"></div>
    <div class="star" style="left:88%; top:35%; animation-delay:.6s;"></div>
</div>
<main>
    <!-- OPENING -->
    <section class="intro">
        <div class="eyebrow">
            A little piece of the universe
        </div>
        <h1>
            Happy Birthday
            <span class="name">Lola</span>
        </h1>
        <p class="intro-text">
            Today the whole sky feels a little brighter,
            because somewhere in this enormous universe,
            you were born.
        </p>
        <div class="scroll">
            ↓ KEEP SCROLLING ↓
        </div>
    </section>
    <!-- MESSAGE -->
    <section class="card">
        <h2>For my Lola 💙</h2>
        <p>
            Happy 27th birthday to the girl who somehow became
            one of the most beautiful parts of my world.
            <br><br>
            If I could give you anything today, I would give you
            every sunset you have ever wanted to see,
            every peaceful night,
            every star in the sky,
            and every moment where you feel completely loved.
            <br><br>
            But since I cannot put the entire universe inside
            a birthday box, I made you this little corner of it instead.
        </p>
    </section>
    <!-- FAVOURITES -->
    <section class="card">
        <h2>Your little world 🌙</h2>
        <div class="favourites">
            <div class="favourite">
                <span class="favourite-icon">💙</span>
                <span class="favourite-text">
                    Baby blue
                </span>
            </div>
            <div class="favourite">
                <span class="favourite-icon">☕</span>
                <span class="favourite-text">
                    Black coffee
                </span>
            </div>
            <div class="favourite">
                <span class="favourite-icon">🦦</span>
                <span class="favourite-text">
                    Otters
                </span>
            </div>
            <div class="favourite">
                <span class="favourite-icon">🌊</span>
                <span class="favourite-text">
                    The ocean
                </span>
            </div>
            <div class="favourite">
                <span class="favourite-icon">🍣</span>
                <span class="favourite-text">
                    Sushi
                </span>
            </div>
            <div class="favourite">
                <span class="favourite-icon">⭐</span>
                <span class="favourite-text">
                    The stars
                </span>
            </div>
        </div>
    </section>
    <!-- BIRTHDAY MESSAGE -->
    <section class="card">
        <div class="big-message">
            27 looks beautiful on you. 💙
        </div>
        <p>
            I hope this year gives you reasons to smile
            that you never saw coming.
            <br><br>
            I hope you get to see the ocean.
            I hope you see beautiful skies.
            I hope you find peaceful mornings
            and gentle nights.
            <br><br>
            And I hope you always remember that
            somewhere in this world,
            there is someone who looks at you
            and thinks,
            <em>"That's my person."</em>
        </p>
    </section>
    <!-- SECRET BUTTON -->
    <section class="card">
        <h2>A little birthday surprise 🎁</h2>
        <p>
            I hid something here just for you.
        </p>
        <button onclick="showSecret()">
            Open it 💙
        </button>
        <div id="secret" class="secret">
            You are loved more than you probably realise.
            <br><br>
            You are someone's favourite person,
            someone's safe place,
            someone's home.
            <br><br>
            Happy birthday, my love.
            ⭐🌊💙
        </div>
    </section>
    <!-- FINAL -->
    <section class="final">
        <div class="final-heart">
            💙
        </div>
        <h2>
            Happy 27th Birthday, Lola
        </h2>
        <p class="signature">
            With all my love,<br>
            Bree / Putiputi
        </p>
    </section>
</main>
<script>
/* =========================
   FLOATING HEARTS
========================= */
const floatingSymbols = [
    "💙",
    "💗",
    "✨",
    "⭐",
    "🌸",
    "🦋"
];
function createFloating() {
    const element =
        document.createElement("div");
    element.className = "floating";
    element.innerHTML =
        floatingSymbols[
            Math.floor(
                Math.random() *
                floatingSymbols.length
            )
        ];
    element.style.left =
        Math.random() * 100 + "vw";
    element.style.fontSize =
        (14 + Math.random() * 18) + "px";
    element.style.animationDuration =
        (6 + Math.random() * 6) + "s";
    document.body.appendChild(element);
    setTimeout(() => {
        element.remove();
    }, 13000);
}
setInterval(createFloating, 700);
/* =========================
   SECRET MESSAGE
========================= */
function showSecret() {
    const secret =
        document.getElementById("secret");
    secret.classList.add("show");
    createConfetti();
}
/* =========================
   CONFETTI
========================= */
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
        i < 70;
        i++
    ) {
        const confetti =
            document.createElement("div");
        confetti.className =
            "confetti";
        confetti.innerHTML =
            symbols[
                Math.floor(
                    Math.random() *
                    symbols.length
                )
            ];
        confetti.style.left =
            Math.random() * 100 + "vw";
        confetti.style.fontSize =
            (10 + Math.random() * 18) + "px";
        confetti.style.animationDuration =
            (2 + Math.random() * 3) + "s";
        confetti.style.animationDelay =
            Math.random() * 0.8 + "s";
        document.body.appendChild(confetti);
        setTimeout(() => {
            confetti.remove();
        }, 5000);
    }
}
/* =========================
   BIRTHDAY SURPRISE
========================= */
window.addEventListener(
    "load",
    () => {
        setTimeout(() => {
            createConfetti();
        }, 1200);
    }
);
</script>
</body>
</html>
