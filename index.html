# Jogo-de-luta-simples-
Apenas um jogo de luta simples 
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Blue vs Red</title>

<style>
* {
    box-sizing: border-box;
    image-rendering: pixelated;
}

body {
    margin: 0;
    background: #111;
    color: white;
    font-family: monospace;
    overflow: hidden;
    text-align: center;
}

#menu {
    position: fixed;
    inset: 0;
    background: #151515;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    z-index: 10;
}

#menu h1 {
    font-size: 45px;
    margin-bottom: 30px;
}

#start {
    background: #22aa55;
    border: 4px solid white;
    color: white;
    padding: 15px 40px;
    font-size: 25px;
    font-family: monospace;
    cursor: pointer;
}

#game {
    display: none;
    width: 100vw;
    height: 100vh;
    position: relative;
    background:
        linear-gradient(#55aadd 0 65%, #26752d 65% 100%);
}

/* Barras de vida */

.health {
    position: absolute;
    top: 20px;
    width: 35%;
    height: 30px;
    background: #333;
    border: 4px solid white;
}

#blueHealthBox {
    left: 5%;
}

#redHealthBox {
    right: 5%;
}

.healthBar {
    height: 100%;
    width: 100%;
}

#blueHealth {
    background: #168cff;
}

#redHealth {
    background: #ff2222;
}

.name {
    position: absolute;
    top: -25px;
    font-size: 18px;
}

#blueName {
    left: 0;
}

#redName {
    right: 0;
}

/* Arena */

#arena {
    position: absolute;
    left: 5%;
    right: 5%;
    top: 15%;
    bottom: 20%;
    border: 5px solid #222;
    overflow: hidden;
}

.player {
    position: absolute;
    width: 55px;
    height: 55px;
    border-radius: 50%;
    border: 5px solid #111;
}

#blue {
    background: #008cff;
    left: 20%;
    top: 50%;
}

#red {
    background: #ff2222;
    left: 75%;
    top: 50%;
}

/* Joysticks */

.joystick {
    position: absolute;
    bottom: 25px;
    width: 130px;
    height: 130px;
    border-radius: 50%;
    background: #444;
    border: 5px solid #aaa;
    touch-action: none;
}

#blueJoystick {
    left: 25px;
}

#redJoystick {
    right: 25px;
}

.stick {
    position: absolute;
    width: 55px;
    height: 55px;
    background: #888;
    border: 4px solid white;
    border-radius: 50%;
    left: 32px;
    top: 32px;
}

/* Ataques */

.attack {
    position: absolute;
    bottom: 60px;
    width: 70px;
    height: 70px;
    border-radius: 50%;
    border: 4px solid white;
    color: white;
    font-size: 30px;
    font-family: monospace;
}

#blueAttack {
    left: 180px;
    background: #087cff;
}

#redAttack {
    right: 180px;
    background: #ee2222;
}

#message {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-size: 45px;
    display: none;
    background: #111;
    border: 5px solid white;
    padding: 20px;
}
</style>
</head>

<body>

<div id="menu">
    <h1>🔵 BLUE VS RED 🔴</h1>
    <button id="start">▶ COMEÇAR JOGO</button>
</div>

<div id="game">

    <div id="blueHealthBox" class="health">
        <span id="blueName" class="name">BLUE</span>
        <div id="blueHealth" class="healthBar"></div>
    </div>

    <div id="redHealthBox" class="health">
        <span id="redName" class="name">RED</span>
        <div id="redHealth" class="healthBar"></div>
    </div>

    <div id="arena">
        <div id="blue" class="player"></div>
        <div id="red" class="player"></div>

        <div id="message"></div>
    </div>

    <!-- Joystick azul -->
    <div id="blueJoystick" class="joystick">
        <div class="stick"></div>
    </div>

    <!-- Ataque azul -->
    <button id="blueAttack" class="attack">👊</button>

    <!-- Ataque vermelho -->
    <button id="redAttack" class="attack">👊</button>

    <!-- Joystick vermelho -->
    <div id="redJoystick" class="joystick">
        <div class="stick"></div>
    </div>

</div>

<script>
const startButton = document.getElementById("start");
const menu = document.getElementById("menu");
const game = document.getElementById("game");

const blue = document.getElementById("blue");
const red = document.getElementById("red");

const blueHealth = document.getElementById("blueHealth");
const redHealth = document.getElementById("redHealth");

const message = document.getElementById("message");

let blueHP = 100;
let redHP = 100;

let blueX = 20;
let blueY = 50;

let redX = 75;
let redY = 50;

let gameRunning = false;

const speed = 0.7;

/* Começar */

startButton.onclick = () => {
    menu.style.display = "none";
    game.style.display = "block";
    gameRunning = true;
};

/* Atualizar personagens */

function updatePlayers() {
    blue.style.left = blueX + "%";
    blue.style.top = blueY + "%";

    red.style.left = redX + "%";
    red.style.top = redY + "%";
}

/* Controle por teclado
   Azul = WASD
   Vermelho = setas
*/

document.addEventListener("keydown", e => {

    if (!gameRunning) return;

    // Azul
    if (e.key === "w") blueY -= speed;
    if (e.key === "s") blueY += speed;
    if (e.key === "a") blueX -= speed;
    if (e.key === "d") blueX += speed;

    // Vermelho
    if (e.key === "ArrowUp") redY -= speed;
    if (e.key === "ArrowDown") redY += speed;
    if (e.key === "ArrowLeft") redX -= speed;
    if (e.key === "ArrowRight") redX += speed;

    limitarPosicoes();
    updatePlayers();
});

/* Ataque */

function attack(player) {

    if (!gameRunning) return;

    let distance = Math.sqrt(
        Math.pow(blueX - redX, 2) +
        Math.pow(blueY - redY, 2)
    );

    if (distance < 13) {

        if (player === "blue") {
            redHP -= 10;
            redHealth.style.width = redHP + "%";
        }

        if (player === "red") {
            blueHP -= 10;
            blueHealth.style.width = blueHP + "%";
        }

        verificarVencedor();
    }
}

document.getElementById("blueAttack").onclick = () => {
    attack("blue");
};

document.getElementById("redAttack").onclick = () => {
    attack("red");
};

/* Limites da arena */

function limitarPosicoes() {

    blueX = Math.max(2, Math.min(94, blueX));
    blueY = Math.max(2, Math.min(88, blueY));

    redX = Math.max(2, Math.min(94, redX));
    redY = Math.max(2, Math.min(88, redY));
}

/* Vitória */

function verificarVencedor() {

    if (blueHP <= 0) {
        vencer("🔴 RED VENCEU!");
    }

    if (redHP <= 0) {
        vencer("🔵 BLUE VENCEU!");
    }
}

function vencer(texto) {

    gameRunning = false;

    message.innerText = texto;
    message.style.display = "block";

    setTimeout(() => {
        location.reload();
    }, 3000);
}

/* Joystick */

function criarJoystick(joystickID, player) {

    const joystick = document.getElementById(joystickID);
    const stick = joystick.querySelector(".stick");

    let ativo = false;

    joystick.addEventListener("pointerdown", e => {
        ativo = true;
        joystick.setPointerCapture(e.pointerId);
    });

    joystick.addEventListener("pointermove", e => {

        if (!ativo || !gameRunning) return;

        const rect = joystick.getBoundingClientRect();

        const centroX = rect.left + rect.width / 2;
        const centroY = rect.top + rect.height / 2;

        let dx = e.clientX - centroX;
        let dy = e.clientY - centroY;

        const distancia = Math.sqrt(dx * dx + dy * dy);
        const limite = 38;

        if (distancia > limite) {
            dx = dx / distancia * limite;
            dy = dy / distancia * limite;
        }

        stick.style.transform =
            `translate(${dx}px, ${dy}px)`;

        if (Math.abs(dx) > 10) {
            if (player === "blue")
                blueX += dx / 100;

            if (player === "red")
                redX += dx / 100;
        }

        if (Math.abs(dy) > 10) {
            if (player === "blue")
                blueY += dy / 100;

            if (player === "red")
                redY += dy / 100;
        }

        limitarPosicoes();
        updatePlayers();
    });

    joystick.addEventListener("pointerup
