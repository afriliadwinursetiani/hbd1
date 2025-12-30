


<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Dino's Birthday Quest</title>
    <link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap" rel="stylesheet">
    <style>
        :root {
            --sky-top: #2b32b2;
            --sky-bottom: #ff9966;
            --glass-bg: rgba(255, 255, 255, 0.15);
            --glass-border: rgba(255, 255, 255, 0.3);
            --text-glow: 0 0 10px rgba(255, 255, 255, 0.5);
        }

        * {
            box-sizing: border-box;
            user-select: none;
            -webkit-user-select: none;
            touch-action: none;
        }

        body {
            margin: 0;
            padding: 0;
            font-family: 'Press Start 2P', cursive;
            background-color: #050505;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            color: #fff;
            overflow: hidden;
        }

        /* GAME CONTAINER - RESPONSIVE FIX */
        #game-container {
            position: relative;
            width: 100%;
            max-width: 900px;
            max-height: 90vh;
            
            aspect-ratio: 16 / 9; 
            
            border: 4px solid #444;
            box-shadow: 0 0 50px rgba(0,0,0,0.9);
            background: linear-gradient(to bottom, var(--sky-top), var(--sky-bottom));
            overflow: hidden;
            border-radius: 8px;
        }

        #game-container::after {
            content: "";
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
            background: linear-gradient(rgba(18, 16, 16, 0) 50%, rgba(0, 0, 0, 0.25) 50%), linear-gradient(90deg, rgba(255, 0, 0, 0.06), rgba(0, 255, 0, 0.02), rgba(0, 0, 255, 0.06));
            background-size: 100% 2px, 3px 100%;
            pointer-events: none;
            z-index: 5;
        }
        
        #game-container::before {
            content: "";
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
            background: radial-gradient(circle, transparent 60%, rgba(0,0,0,0.6) 100%);
            pointer-events: none;
            z-index: 5;
        }

        canvas {
            display: block;
            width: 100%;
            height: 100%;
            image-rendering: pixelated;
        }

        .ui-layer {
            position: absolute;
            top: 20px;
            left: 20px;
            z-index: 4;
            pointer-events: none;
            text-shadow: 2px 2px 0 #000;
        }

        .score-board { font-size: 1.2rem; color: #fff; }
        .target { font-size: 0.7rem; color: #ddd; margin-top: 5px; }

        .screen {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 90%;
            max-width: 450px;
            background: var(--glass-bg);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border: 2px solid var(--glass-border);
            border-radius: 15px;
            padding: 25px;
            text-align: center;
            z-index: 10;
            display: flex;
            flex-direction: column;
            gap: 15px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.5);
            animation: popIn 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }

        .hidden { display: none !important; }

        h1 {
            font-size: 1.2rem;
            color: #FFD700;
            text-shadow: var(--text-glow);
            margin: 0;
            line-height: 1.4;
        }

        p {
            font-size: 0.7rem;
            line-height: 1.5;
            margin: 0;
            color: #eee;
        }

        input {
            font-family: 'Press Start 2P', cursive;
            padding: 12px;
            border: 2px solid rgba(255,255,255,0.3);
            background: rgba(0,0,0,0.5);
            color: #fff;
            border-radius: 5px;
            text-align: center;
            width: 100%;
            outline: none;
            transition: border-color 0.3s;
            font-size: 0.7rem;
        }
        input:focus { border-color: #FFD700; }

        button {
            font-family: 'Press Start 2P', cursive;
            padding: 12px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            font-size: 0.7rem;
            color: #fff;
            transition: transform 0.1s, box-shadow 0.3s;
            box-shadow: 0 5px 15px rgba(0,0,0,0.3);
            text-transform: uppercase;
            margin-top: 10px;
        }
        button:active { transform: scale(0.95); box-shadow: none; }

        .btn-start { background: linear-gradient(45deg, #11998e, #38ef7d); }
        .btn-lose { background: linear-gradient(45deg, #cb2d3e, #ef473a); }
        .btn-win { background: linear-gradient(45deg, #ff9966, #ff5e62); }

        #end-canvas-container {
            width: 100%;
            height: 0;
            padding-bottom: 56.25%; 
            position: relative;
            margin: 10px 0;
            border-radius: 10px;
            overflow: hidden;
            background: rgba(0,0,0,0.3);
            border: 1px solid rgba(255,255,255,0.1);
        }
        #endCanvas {
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
        }

        @keyframes popIn {
            from { opacity: 0; transform: translate(-50%, -40%) scale(0.9); }
            to { opacity: 1; transform: translate(-50%, -50%) scale(1); }
        }

        #sound-btn {
            position: absolute;
            bottom: 15px;
            right: 15px;
            background: rgba(255,255,255,0.15);
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255,255,255,0.2);
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            z-index: 20;
            font-size: 1rem;
            transition: background 0.3s;
        }
        #sound-btn:hover { background: rgba(255,255,255,0.3); }

    </style>
</head>
<body>

<div id="game-container">
    <canvas id="gameCanvas"></canvas>

    <div class="ui-layer">
        <div class="score-board">SCORE: <span id="score">0</span></div>
        <div class="target">GOAL: 1000</div>
    </div>

    <div id="start-screen" class="screen">
        <h1>Dino's Birthday</h1>
        <p>Bawa Dino sampai garis finish!</p>
        <p>Hindari kaktus.</p>
        <input type="text" id="player-name" placeholder="Nama Ulang Tahun..." maxlength="10">
        <button class="btn-start" id="btn-start">MULAI</button>
    </div>

    <div id="result-screen" class="screen hidden">
        <h1 id="result-title">SELESAI!</h1>
        <div id="end-canvas-container">
            <canvas id="endCanvas"></canvas>
        </div>
        <p id="result-message">Pesan disini.</p>
        <button id="btn-restart" class="btn-lose">MAIN LAGI</button>
    </div>

    <div id="sound-btn">🔊</div>
</div>

<script>
/**
 * ENGINE GAME & VISUALS
 */
const canvas = document.getElementById('gameCanvas');
const ctx = canvas.getContext('2d');
const endCanvas = document.getElementById('endCanvas');
const endCtx = endCanvas.getContext('2d');

// UI Elements
const scoreEl = document.getElementById('score');
const startScreen = document.getElementById('start-screen');
const resultScreen = document.getElementById('result-screen');
const resultTitle = document.getElementById('result-title');
const resultMessage = document.getElementById('result-message');
const restartBtn = document.getElementById('btn-restart');
const nameInput = document.getElementById('player-name');

// Game State
let gameSpeed = 6;
let score = 0;
let isPlaying = false;
let frame = 0;
let playerName = "Sahabat";
let soundEnabled = true;
let endAnimationId = null;

// Physics
const gravity = 0.6;
const dino = {
    x: 50,
    y: 0,
    width: 44, 
    height: 48,
    dy: 0,
    jumpForce: 11,
    grounded: false
};

// Objects
let obstacles = [];
let particles = [];
let candles = [];
let clouds = [];
let mountains = [];
let bgObjects = []; 
let sun = { x: 0, y: 0, r: 0 };

// --- SPUITES ---

const dinoSprite = [
    "00000000011000000000", 
    "00000000111100000000", 
    "00000000111100000000",
    "00000011111110000000", 
    "00000012222210000000", 
    "00000112222211000000", 
    "00000111111111000000", 
    "00001111111111100000", 
    "00001111111111100000",
    "00000111111111000000", 
    "00000111111111000000",
    "00000001111000000000", 
    "00000001111000000000",
    "00000000011000000000", 
    "00000000011000000000"
];

const bouquetSprite = [
    "0004444000", 
    "0044444400",
    "0024444200", 
    "0022222200", 
    "0111111100", 
    "0011111000",
    "0001110000",
    "0000100000", 
    "0000100000"
];

const cakeSprite = [
    "004444444444444400",
    "004444444444444400",
    "003333333333333300",
    "003333333333333300",
    "000033333333330000",
    "000033333333330000",
    "022222222222222220",
    "022222222222222220",
    "0111100000000011110",
    "0111100000000011110",
    "0111100000000011110",
    "0111100000000011110"
];

const flowerSprite = [
    "00000444444000000",
    "00044444444440000",
    "00444444444444000",
    "00443333333344000",
    "00043333333340000",
    "00004333333400000",
    "00000022000000000",
    "00000022000000000",
    "00000000000000000",
    "00000001100000000",
    "00000001100000000",
    "00000011100000000",
    "00000111100000000"
];

const cactusSprite = [
    "001100",
    "011100",
    "022200",
    "122221",
    "111111",
    "011100",
    "011100",
    "011100"
];

// --- AUDIO ---
const AudioContext = window.AudioContext || window.webkitAudioContext;
const audioCtx = new AudioContext();

function playSound(type) {
    if (!soundEnabled) return;
    if (audioCtx.state === 'suspended') audioCtx.resume();
    const osc = audioCtx.createOscillator();
    const gain = audioCtx.createGain();
    osc.connect(gain);
    gain.connect(audioCtx.destination);
    const now = audioCtx.currentTime;
    if (type === 'jump') {
        osc.type = 'triangle';
        osc.frequency.setValueAtTime(150, now);
        osc.frequency.linearRampToValueAtTime(300, now + 0.1);
        gain.gain.setValueAtTime(0.1, now);
        gain.gain.linearRampToValueAtTime(0.01, now + 0.1);
        osc.start(); osc.stop(now + 0.1);
    } else if (type === 'score') {
        osc.type = 'sine';
        osc.frequency.setValueAtTime(600, now);
        osc.frequency.linearRampToValueAtTime(1200, now + 0.1);
        gain.gain.setValueAtTime(0.05, now);
        gain.gain.linearRampToValueAtTime(0.01, now + 0.2);
        osc.start(); osc.stop(now + 0.2);
    } else if (type === 'hit') {
        osc.type = 'sawtooth';
        osc.frequency.setValueAtTime(100, now);
        osc.frequency.exponentialRampToValueAtTime(10, now + 0.3);
        gain.gain.setValueAtTime(0.2, now);
        gain.gain.linearRampToValueAtTime(0.01, now + 0.3);
        osc.start(); osc.stop(now + 0.3);
    }
}

function playHappyBirthday() {
    if (!soundEnabled) return;
    if (audioCtx.state === 'suspended') audioCtx.resume();

    const now = audioCtx.currentTime;
    const beat = 0.4; 
    // Melody: G G A G C B | G G A G D C | G G G(high) E C B A | F F E C D C
    // Freqs: G4=392, A4=440, B4=493, C5=523, D5=587, E5=659, F5=698, G5=783

    const notes = [
        {f:392, d:beat}, {f:392, d:beat}, {f:440, d:beat*2}, 
        {f:392, d:beat*2}, {f:523, d:beat*2}, {f:493, d:beat*4},
        
        {f:392, d:beat}, {f:392, d:beat}, {f:440, d:beat*2}, 
        {f:392, d:beat*2}, {f:587, d:beat*2}, {f:523, d:beat*4},
        
        {f:392, d:beat}, {f:392, d:beat*2}, {f:783, d:beat*2}, 
        {f:659, d:beat*2}, {f:523, d:beat*2}, {f:493, d:beat*2}, {f:440, d:beat*4},
        
        {f:698, d:beat}, {f:698, d:beat*2}, {f:659, d:beat*2}, 
        {f:523, d:beat*2}, {f:587, d:beat*2}, {f:523, d:beat*4}
    ];

    let startTime = now;
    
    notes.forEach(note => {
        const osc = audioCtx.createOscillator();
        const gain = audioCtx.createGain();
        osc.connect(gain); 
        gain.connect(audioCtx.destination);
        
        osc.type = 'triangle';
        osc.frequency.value = note.f;
        
        gain.gain.setValueAtTime(0, startTime);
        gain.gain.linearRampToValueAtTime(0.1, startTime + 0.05);
        gain.gain.setValueAtTime(0.1, startTime + note.d - 0.1);
        gain.gain.linearRampToValueAtTime(0, startTime + note.d);
        
        osc.start(startTime);
        osc.stop(startTime + note.d);
        startTime += note.d;
    });
}

// --- SETUP ---
function resize() {
    canvas.width = 800;
    canvas.height = 450;
    endCanvas.width = 400;
    endCanvas.height = 225;
    dino.y = canvas.height - 100 - dino.height;
    sun.r = 50; sun.x = canvas.width * 0.8; sun.y = canvas.height * 0.3;
}
window.addEventListener('resize', resize);
resize();

function initBackground() {
    clouds = [];
    for(let i=0; i<6; i++) clouds.push({ x: Math.random()*canvas.width, y: Math.random()*(canvas.height/2), w: 40 + Math.random()*30, speed: 0.2 + Math.random()*0.3 });
    
    mountains = [];
    for(let i=0; i<3; i++) mountains.push({ x: i*300, y: canvas.height-100, w: 300, h: 100+Math.random()*150, color: i%2==0 ? '#342E37' : '#25202A' });

    bgObjects = [];
    for(let i=0; i<canvas.width * 2; i += 120 + Math.random()*100) {
        const type = Math.random() > 0.6 ? 'dino_party' : 'flower';
        bgObjects.push({
            x: i,
            y: canvas.height - 100,
            type: type,
            colorOffset: Math.random() * 0.2
        });
    }
}

// --- INPUT ---
function jump() {
    if (!isPlaying) return;
    if (dino.grounded) {
        dino.dy = -dino.jumpForce;
        dino.grounded = false;
        playSound('jump');
    }
}
document.addEventListener('keydown', (e) => { if(e.code === 'Space' || e.code === 'ArrowUp') jump(); });
canvas.addEventListener('mousedown', jump);
canvas.addEventListener('touchstart', (e) => { e.preventDefault(); jump(); });

document.getElementById('btn-start').addEventListener('click', startGame);
restartBtn.addEventListener('click', () => {
    cancelAnimationFrame(endAnimationId);
    resultScreen.classList.add('hidden');
    startScreen.classList.remove('hidden');
});
document.getElementById('sound-btn').addEventListener('click', () => {
    soundEnabled = !soundEnabled;
    document.getElementById('sound-btn').innerText = soundEnabled ? '🔊' : '🔇';
});

// --- GAME LOOP ---

function startGame() {
    const inputName = nameInput.value.trim();
    if (inputName) playerName = inputName;
    
    score = 0;
    gameSpeed = 6;
    isPlaying = true;
    obstacles = [];
    candles = [];
    dino.y = canvas.height - 100 - dino.height;
    dino.dy = 0;
    
    startScreen.classList.add('hidden');
    resultScreen.classList.add('hidden');
    scoreEl.innerText = '0';
    
    initBackground();
    loop();
}

function spawnObstacle() {
    const h = 30 + Math.random() * 30;
    obstacles.push({ x: canvas.width, y: canvas.height - 100 - h + 5, w: 30, h: h });
}
function spawnCandle() {
    candles.push({ x: canvas.width, y: canvas.height - 180 - Math.random()*80, w: 20, h: 30, collected: false });
}

function update() {
    if (!isPlaying) return;
    
    score++;
    scoreEl.innerText = Math.floor(score / 10);
    if (score % 500 === 0) gameSpeed += 0.5;
    if (score >= 10000) { showResult(true); }

    dino.dy += gravity;
    dino.y += dino.dy;
    if (dino.y + dino.height > canvas.height - 100) {
        dino.y = canvas.height - 100 - dino.height;
        dino.dy = 0;
        dino.grounded = true;
    } else { dino.grounded = false; }

    if (frame % 100 === 0) spawnObstacle();
    if (frame % 250 === 0) spawnCandle();

    obstacles.forEach((obs, i) => {
        obs.x -= gameSpeed;
        if (collision(dino, obs)) showResult(false);
        if (obs.x + obs.w < 0) obstacles.splice(i, 1);
    });

    candles.forEach((c, i) => {
        c.x -= gameSpeed;
        if (!c.collected && collision(dino, c)) {
            c.collected = true;
            score += 300;
            createParticles(c.x, c.y, '#FFD700');
            playSound('score');
        }
        if (c.x + c.w < 0) candles.splice(i, 1);
    });

    clouds.forEach(c => { c.x -= c.speed; if (c.x + c.w*2 < 0) c.x = canvas.width; });
    mountains.forEach(m => { m.x -= gameSpeed * 0.1; if (m.x + m.w < 0) m.x = canvas.width; });
    bgObjects.forEach(obj => {
        obj.x -= gameSpeed * 0.05; 
        if (obj.x < -50) obj.x = canvas.width + Math.random() * 200;
    });

    particles.forEach((p, i) => {
        p.x += p.vx; p.y += p.vy; p.life--;
        if (p.life <= 0) particles.splice(i, 1);
    });

    frame++;
}

function drawMinecraftGround(context, width, height) {
    const groundY = height - 100;
    const blockSize = 20;

    // 1. Isi Tanah Coklat (Dirt)
    context.fillStyle = '#795548';
    context.fillRect(0, groundY, width, 100);

    // 2. Gambar Blok Rumput (Green) di atas
    for (let x = 0; x < width; x += blockSize) {
        context.fillStyle = '#4CAF50';
        context.fillRect(x, groundY, blockSize, blockSize);

        // Tambahkan tekstur pixel acak
        context.fillStyle = '#388E3C';
        if ((x/blockSize) % 2 === 0) {
            context.fillRect(x + 5, groundY + 2, 4, 4);
            context.fillRect(x + 12, groundY + 12, 4, 4);
        } else {
            context.fillRect(x + 8, groundY + 6, 4, 4);
        }
        
        // Tepi atas blok
        context.fillStyle = '#66BB6A'; 
        context.fillRect(x, groundY, blockSize, 2);
    }
}

function draw() {
    ctx.clearRect(0, 0, canvas.width, canvas.height);

    let grad = ctx.createRadialGradient(sun.x, sun.y, sun.r * 0.5, sun.x, sun.y, sun.r * 2);
    grad.addColorStop(0, 'rgba(255, 255, 200, 0.8)');
    grad.addColorStop(0.5, 'rgba(255, 150, 50, 0.3)');
    grad.addColorStop(1, 'rgba(255, 100, 50, 0)');
    ctx.fillStyle = grad;
    ctx.fillRect(0, 0, canvas.width, canvas.height);
    ctx.fillStyle = '#FFF5CB';
    ctx.beginPath();
    ctx.arc(sun.x, sun.y, sun.r, 0, Math.PI*2);
    ctx.fill();

    ctx.fillStyle = 'rgba(255, 255, 255, 0.4)';
    clouds.forEach(c => {
        ctx.beginPath();
        ctx.arc(c.x, c.y, c.w, 0, Math.PI * 2);
        ctx.arc(c.x + c.w*0.8, c.y - c.w*0.2, c.w*0.7, 0, Math.PI * 2);
        ctx.arc(c.x - c.w*0.8, c.y - c.w*0.2, c.w*0.7, 0, Math.PI * 2);
        ctx.fill();
    });

    mountains.forEach(m => {
        ctx.fillStyle = m.color;
        ctx.beginPath();
        ctx.moveTo(m.x, m.y);
        ctx.lineTo(m.x + m.w/2, m.y - m.h);
        ctx.lineTo(m.x + m.w, m.y);
        ctx.fill();
    });

    bgObjects.forEach(obj => {
        if (obj.type === 'flower') {
            drawSpriteCtx(ctx, flowerSprite, obj.x, obj.y - 25, 2, '#E91E63');
        } else if (obj.type === 'dino_party') {
            let color = '#9C27B0'; 
            if (obj.colorOffset > 0.1) color = '#E91E63';
            drawSpriteCtx(ctx, dinoSprite, obj.x, obj.y - 48, 3, color);
            drawSpriteCtx(ctx, bouquetSprite, obj.x + 35, obj.y - 35, 2, '#ffcc80');
        }
    });

    drawMinecraftGround(ctx, canvas.width, canvas.height);

    candles.forEach(c => {
        if (!c.collected) {
            ctx.fillStyle = '#EEE';
            ctx.fillRect(c.x, c.y + 10, c.w, c.h - 10);
            ctx.fillStyle = Math.random() > 0.5 ? '#FF5722' : '#FFC107';
            ctx.fillRect(c.x + 5, c.y, 10, 10);
        }
    });

    obstacles.forEach(obs => {
        drawSpriteCtx(ctx, cactusSprite, obs.x, obs.y, 4, '#2ecc71');
    });

    let propY = dino.y;
    if(dino.grounded) propY += Math.sin(frame * 0.3) * 3;
    
    drawSpriteCtx(ctx, dinoSprite, dino.x, propY, 4, '#2196F3');
    drawSpriteCtx(ctx, bouquetSprite, dino.x + 42, propY + 20, 4, '#E91E63');

    particles.forEach(p => {
        ctx.fillStyle = p.color;
        ctx.globalAlpha = p.life / 20;
        ctx.fillRect(p.x, p.y, 4, 4);
        ctx.globalAlpha = 1;
    });
}

// --- ENDING SYSTEM ---

function showResult(win) {
    isPlaying = false;
    resultScreen.classList.remove('hidden');
    
    setTimeout(playHappyBirthday, 500);

    if (win) {
        resultTitle.innerText = "SELAMAT!";
        resultTitle.style.color = "#FFD700";
        resultMessage.innerHTML = `Selamat Ulang Tahun, <strong>${playerName}</strong>!<br>Kamu hebat sekali!`;
        restartBtn.className = "btn-win";
        restartBtn.innerText = "RAYAKAN LAGI";
        startEndAnimation(true);
    } else {
        resultTitle.innerText = "YAH...";
        resultTitle.style.color = "#EF5350";
        resultMessage.innerHTML = `Selamat Ulang Tahun, <strong>${playerName}</strong>!<br>Jangan sedih dan tetap semangat ya!`;
        restartBtn.className = "btn-lose";
        restartBtn.innerText = "COBA LAGI";
        startEndAnimation(false);
    }
}

// --- REALISTIC BALLOON DRAWING ---
function drawRealBalloon(ctx, x, y, r, color) {
    // 1. Gambar Tali (String) - Goyang sedikit
    ctx.beginPath();
    ctx.moveTo(x, y + r);
    // Tali melengkung acak
    let stringCurve = Math.sin(Date.now() * 0.005 + x) * 5;
    ctx.quadraticCurveTo(x + stringCurve, y + r + 15, x, y + r + 30);
    ctx.strokeStyle = 'rgba(255,255,255,0.5)';
    ctx.lineWidth = 1;
    ctx.stroke();

    // 2. Badan Balon (Sphere 3D Effect dengan Radial Gradient)
    let grad = ctx.createRadialGradient(x - r*0.3, y - r*0.3, r*0.1, x, y, r);
    grad.addColorStop(0, 'rgba(255,255,255,0.9)'); // Highlight sangat terang
    grad.addColorStop(0.2, color); // Warna asli
    grad.addColorStop(1, adjustColor(color, -40)); // Bayangan tepi (lebih gelap)

    ctx.fillStyle = grad;
    ctx.beginPath();
    ctx.arc(x, y, r, 0, Math.PI * 2);
    ctx.fill();

    // 3. Highlight Specular (Kilau Kaca/Karet)
    ctx.fillStyle = 'rgba(255,255,255,0.4)';
    ctx.beginPath();
    ctx.ellipse(x - r*0.35, y - r*0.35, r*0.15, r*0.08, Math.PI / 4, 0, Math.PI*2);
    ctx.fill();

    // 4. Knot (Simpul kecil di bawah)
    ctx.fillStyle = color;
    ctx.beginPath();
    ctx.moveTo(x - 2, y + r - 1);
    ctx.lineTo(x + 2, y + r - 1);
    ctx.lineTo(x, y + r + 3);
    ctx.fill();
}

// Helper untuk mencerahkan/menggelapkan warna Hex
function adjustColor(color, amount) {
    return '#' + color.replace(/^#/, '').replace(/../g, color => ('0'+Math.min(255, Math.max(0, parseInt(color, 16) + amount)).toString(16)).substr(-2));
}

function startEndAnimation(isWin) {
    let eFrame = 0;
    
    // BALOON BESAR (REALISTIK)
    let balloons = [];
    const balloonColors = ['#EF5350', '#42A5F5', '#FFCA28', '#AB47BC', '#66BB6A', '#FF7043', '#EC407A', '#26A69A'];
    
    for(let i=0; i<12; i++) {
        balloons.push({
            x: Math.random() * endCanvas.width,
            y: endCanvas.height + 50 + Math.random() * 200,
            speed: 0.5 + Math.random() * 1.5,
            wobble: Math.random() * Math.PI * 2,
            wobbleSpeed: 0.02 + Math.random() * 0.05,
            color: balloonColors[Math.floor(Math.random() * balloonColors.length)],
            radius: 10 + Math.random() * 5 // Radius untuk balon realistik
        });
    }

    // CONFETTI SYSTEM (PAMPETI)
    let confettiParticles = [];
    const confettiColors = ['#FFD700', '#FF5252', '#448AFF', '#69F0AE', '#E040FB'];
    for(let i=0; i<60; i++) {
        confettiParticles.push({
            x: Math.random() * endCanvas.width,
            y: -10 - Math.random() * endCanvas.height,
            vx: (Math.random() - 0.5) * 2,
            vy: 1 + Math.random() * 2,
            color: confettiColors[Math.floor(Math.random() * confettiColors.length)],
            rotation: Math.random() * 360,
            rotSpeed: (Math.random() - 0.5) * 10
        });
    }
    
    function endLoop() {
        endCtx.clearRect(0, 0, endCanvas.width, endCanvas.height);
        
        endCtx.fillStyle = isWin ? "rgba(46, 204, 113, 0.2)" : "rgba(52, 73, 94, 0.2)";
        endCtx.fillRect(0,0,endCanvas.width, endCanvas.height);

        const cx = endCanvas.width / 2 - 25;
        const cy = endCanvas.height / 2 + 20;
        
        const bounce = Math.sin(eFrame * 0.05) * 5; 
        const finalY = cy + bounce;

        // --- GAMBAR CONFETTI (PAMPETI) ---
        confettiParticles.forEach(p => {
            p.y += p.vy;
            p.x += p.vx + Math.sin(eFrame * 0.05) * 0.5;
            p.rotation += p.rotSpeed;

            if (p.y > endCanvas.height) {
                p.y = -10;
                p.x = Math.random() * endCanvas.width;
            }

            endCtx.save();
            endCtx.translate(p.x, p.y);
            endCtx.rotate(p.rotation * Math.PI / 180);
            endCtx.fillStyle = p.color;
            endCtx.fillRect(-3, -3, 6, 6);
            endCtx.restore();
        });

        // --- GAMBAR BALOON (REALISTIK) ---
        balloons.forEach(b => {
            b.y -= b.speed; 
            b.wobble += b.wobbleSpeed; 
            let wobbleX = Math.sin(b.wobble) * 0.5;
            
            if (b.y < -100) {
                b.y = endCanvas.height + 100;
                b.x = Math.random() * endCanvas.width;
            }

            // Panggil fungsi gambar balon realistik baru
            drawRealBalloon(endCtx, b.x + wobbleX, b.y, b.radius, b.color);
        });

        // Gambar Dino
        drawSpriteCtx(endCtx, dinoSprite, cx, finalY, 4, '#2196F3');

        if (isWin) {
            drawSpriteCtx(endCtx, bouquetSprite, cx + 20, finalY + 20, 4, '#E91E63');
            drawSpriteCtx(endCtx, cakeSprite, cx - 30, finalY - 10, 4, '#ffcc80');
        } else {
            drawSpriteCtx(endCtx, bouquetSprite, cx + 20, finalY + 20, 4, '#E91E63');
        }

        eFrame++;
        endAnimationId = requestAnimationFrame(endLoop);
    }
    endLoop();
}

function drawSpriteCtx(context, spriteMap, startX, startY, pixelSize, mainColor) {
    const rows = spriteMap.length;
    const cols = spriteMap[0].length;
    
    for (let r = 0; r < rows; r++) {
        for (let c = 0; c < cols; c++) {
            const char = spriteMap[r][c];
            if (char !== '0') {
                let color = mainColor;
                
                if (mainColor === '#2196F3') {
                    if (char === '2') color = '#64B5F6'; 
                    if (char === '1') color = '#1565C0'; 
                    if (r===1 && c===9) color = 'white';
                    if (r===1 && c===10) color = 'black';
                } 
                else if (mainColor === '#E91E63') {
                    if (char === '4') color = '#E91E63'; 
                    if (char === '2') color = '#FFEB3B'; 
                    if (char === '1') color = '#FFFFFF'; 
                    if(r >= 7) color = '#D32F2F'; 
                }
                else if (mainColor === '#9C27B0' || mainColor === '#E91E63') {
                    if (char === '2') color = '#BA68C8';
                    if (char === '1') color = '#7B1FA2';
                }
                else if (mainColor === '#ffcc80') {
                    if (char === '4') color = '#EF5350';
                    if (char === '2') color = '#FFCC80';
                    if (char === '1') color = '#A1887F';
                }
                else if (spriteMap === flowerSprite) {
                     if (char === '4') color = '#F48FB1';
                     if (char === '2') color = '#880E4F';
                     if (char === '3') color = '#FCE4EC';
                }

                context.fillStyle = color;
                context.fillRect(startX + c * pixelSize, startY + r * pixelSize, pixelSize, pixelSize);
            }
        }
    }
}

function collision(a, b) {
    return (a.x < b.x + b.w && a.x + a.width > b.x &&
            a.y < b.y + b.h && a.y + a.height > b.y);
}

function createParticles(x, y, color) {
    for (let i = 0; i < 10; i++) {
        particles.push({
            x: x, y: y,
            vx: (Math.random() - 0.5) * 5,
            vy: (Math.random() - 0.5) * 5,
            life: 20,
            color: color
        });
    }
}

function loop() {
    update();
    draw();
    if (isPlaying) requestAnimationFrame(loop);
}

resize();
initBackground();
draw();

</script>
</body>
</html>
