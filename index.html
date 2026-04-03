<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>GSlots Palace</title>
    <style>
        :root { --gray: #f2f2f7; --blue: #007aff; --gold: #f0c36d; --dark: #1c1c1e; --red: #ff3b30; }
        * { box-sizing: border-box; -webkit-tap-highlight-color: transparent; font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif; }
        
        body { background: #ffffff; margin: 0; display: flex; justify-content: center; min-height: 100vh; overflow-x: hidden; position: relative; }

        /* ТОТ САМЫЙ ПРОШЛЫЙ ФОН (ЧЕРНЫЕ ТРЕУГОЛЬНИКИ) */
        #particles-js {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 1; /* Нижний слой */
            pointer-events: none; /* Пропускает клики */
        }

        /* ХАБ */
        #hub-page { width: 100%; max-width: 414px; padding: 20px; min-height: 100vh; display: block; position: relative; z-index: 10; }
        .hub-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 25px; }
        .hub-header h1 { font-size: 28px; font-weight: 900; margin: 0; color: var(--dark); cursor: pointer; letter-spacing: -1px; }
        .hub-balance { background: #fff; padding: 10px 18px; border-radius: 25px; font-weight: 800; font-size: 15px; box-shadow: 0 4px 10px rgba(0,0,0,0.05); border: 1px solid #eee; }
        
        .game-card { background: #fff; border-radius: 24px; overflow: hidden; box-shadow: 0 6px 20px rgba(0,0,0,0.08); cursor: pointer; transition: 0.2s; border: 1px solid rgba(0,0,0,0.03); }
        .card-banner { height: 140px; display: flex; align-items: center; justify-content: center; background: linear-gradient(135deg, #000, #444); }
        .card-emoji { font-size: 60px; filter: drop-shadow(0 5px 10px rgba(0,0,0,0.2)); }
        .card-info { padding: 18px; }
        .card-title { font-weight: 900; font-size: 22px; color: var(--dark); }
        .card-subtitle { font-size: 12px; color: #8e8e93; font-weight: 700; text-transform: uppercase; letter-spacing: 1px; }

        /* СЛОТ */
        #slot-page { display: none; width: 100%; max-width: 414px; background: rgba(255,255,255,0.7); position: relative; min-height: 100vh; z-index: 20; }
        .back-bar { padding: 15px; display: flex; justify-content: space-between; align-items: center; background: rgba(255,255,255,0.9); backdrop-filter: blur(5px); border-bottom: 1px solid var(--gray); position: sticky; top: 0; z-index: 30; }
        .logo-btn { color: var(--dark); font-weight: 900; font-size: 20px; cursor: pointer; }
        
        .app { padding: 15px; display: flex; flex-direction: column; }
        .win-display { text-align: center; font-size: 28px; font-weight: 900; height: 45px; color: #000; margin-bottom: 5px; }
        .fs-counter { text-align: center; color: var(--red); font-weight: 800; font-size: 18px; margin-bottom: 5px; visibility: hidden; }
        
        .slot-window { background: #fff; border: 1px solid rgba(0,0,0,0.1); border-radius: 20px; overflow: hidden; position: relative; box-shadow: 0 10px 30px rgba(0,0,0,0.05); }
        .grid { display: grid; grid-template-columns: repeat(5, 1fr); gap: 1px; background: rgba(0,0,0,0.05); }
        .cell { aspect-ratio: 1/1; background: #fff; display: flex; align-items: center; justify-content: center; font-size: 42px; position: relative; }
        
        .cell.spinning { animation: fall 0.3s cubic-bezier(0.25, 0.46, 0.45, 0.94) both; }
        .cell.win-pulse { animation: pulse 0.6s infinite alternate; background: #fff9e6; z-index: 2; border: 2px solid var(--gold); border-radius: 8px; }
        .cell.sticky { border: 3px solid var(--gold) !important; background: #fffdf5; box-shadow: inset 0 0 15px rgba(240,195,109,0.3); }
        
        @keyframes fall { 0% { transform: translateY(-100%); opacity: 0; } 100% { transform: translateY(0); opacity: 1; } }
        @keyframes pulse { from { transform: scale(1); } to { transform: scale(1.08); } }

        .bet-box { background: var(--dark); color: #fff; border-radius: 15px; padding: 14px; text-align: center; font-size: 24px; font-weight: 800; margin: 12px 0; cursor: pointer; }
        .buy-btn { background: linear-gradient(135deg, #ff9500, #ff5e00); color: #fff; border: none; width: 100%; padding: 15px; border-radius: 15px; font-weight: 800; margin-bottom: 12px; cursor: pointer; font-size: 16px; }
        .main-btn { width: 100%; height: 65px; border-radius: 20px; border: none; background: linear-gradient(180deg, #007aff, #0056b3); cursor: pointer; display: flex; justify-content: center; align-items: center; z-index: 50; position: relative; }
        .main-btn svg { width: 32px; fill: #fff; }

        .settings { display: flex; justify-content: space-between; margin-top: 15px; }
        .toggle-box { display: flex; align-items: center; font-size: 13px; font-weight: 700; cursor: pointer; }
        .toggle-icon { width: 22px; height: 22px; border: 2px solid #ccc; border-radius: 6px; margin-right: 8px; position: relative; }
        .toggle-icon.active { background: var(--blue); border-color: var(--blue); }
        .toggle-icon.active::after { content: '✓'; color: #fff; position: absolute; left: 4px; top: -1px; font-size: 14px; }

        /* МОДАЛКИ (Новый дизайн) */
        .modal { position: fixed; inset: 0; background: rgba(0,0,0,0.8); display: none; align-items: center; justify-content: center; z-index: 100; backdrop-filter: blur(8px); }
        .card { width: 85%; background: #fff; border-radius: 25px; padding: 25px; text-align: center; border: 1px solid #eee; box-shadow: 0 10px 30px rgba(0,0,0,0.3); }
        .input-bet { width: 100%; padding: 15px; border-radius: 12px; border: 2px solid #eee; font-size: 24px; font-weight: 800; text-align: center; margin: 15px 0; outline: none; }
        
        .modal-btn-primary { background: var(--blue); color: #fff; padding: 15px; border-radius: 15px; border: none; font-weight: 800; font-size: 16px; cursor: pointer; width: 100%; margin-top: 10px; }
        .modal-btn-secondary { background: #eee; color: #000; padding: 15px; border-radius: 15px; border: none; font-weight: 800; font-size: 16px; cursor: pointer; width: 100%; }

        /* ПРАВИЛА */
        #rules-page { display: none; position: fixed; inset: 0; background: #fff; z-index: 200; padding: 20px; overflow-y: auto; }
        .rule-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; margin-top: 20px; }
        .rule-card { background: #f9f9f9; padding: 15px; border-radius: 15px; display: flex; flex-direction: column; align-items: center; text-align: center; border: 1px solid #eee; }
        .rule-emoji { font-size: 30px; margin-bottom: 5px; }
        .rule-txt { font-size: 12px; font-weight: 800; }
        .special-rule { grid-column: span 2; background: #fff9e6; border: 1px solid var(--gold); }
    </style>
</head>
<body>

<div id="particles-js"></div>

<div id="hub-page">
    <div class="hub-header">
        <h1 onclick="location.reload()">GSlots</h1>
        <div class="hub-balance">Баланс: $<span id="hub-bal-val">5,000,000</span></div>
    </div>
    <div class="game-card" onclick="openGame()">
        <div class="card-banner"><span class="card-emoji">💎</span></div>
        <div class="card-info">
            <div class="card-title">GSlots Palace</div>
            <div class="card-subtitle">5-IN-A-LINE • FULL VERSION</div>
        </div>
    </div>
</div>

<div id="slot-page">
    <div class="back-bar">
        <div class="logo-btn" onclick="backToHub()">GSlots</div>
        <div style="font-weight: 800; color: #8e8e93; font-size: 14px;">PALACE</div>
        <div onclick="openRules(true)" style="color:var(--blue); font-weight:800; cursor:pointer;">ИНФО</div>
    </div>

    <div class="app">
        <div class="win-display" id="win-text">ВЫИГРЫШ $0</div>
        <div class="fs-counter" id="fs-label">ФРИСПИНЫ: <span id="fs-count">0</span></div>

        <div class="slot-window">
            <div class="grid" id="grid"></div>
        </div>

        <div style="font-size:12px; color:#8e8e93; margin-top:10px; font-weight:700;">БАЛАНС: $<span id="bal-val">5,000,000</span></div>
        <div class="bet-box" id="bet-display" onclick="openBetModal()">$5,000</div>

        <button class="buy-btn" onclick="askBuyBonus()">КУПИТЬ БОНУС $<span id="buy-price">100,000</span></button>

        <button class="main-btn" onclick="handleSpin()" id="spin-btn">
            <svg id="svg-play" viewBox="0 0 24 24" width="32"><path d="M8 5v14l11-7z" fill="white"/></svg>
            <svg id="svg-stop" style="display:none" viewBox="0 0 24 24" width="32"><rect x="6" y="6" width="12" height="12" fill="white"/></svg>
        </button>

        <div class="settings">
            <div class="toggle-box" onclick="toggle('turbo')"><div class="toggle-icon" id="t-turbo"></div> ТУРБО</div>
            <div class="toggle-box" onclick="toggle('auto')"><div class="toggle-icon" id="t-auto"></div> АВТО</div>
        </div>
    </div>
</div>

<div class="modal" id="modal-bet">
    <div class="card">
        <h3>СТАВКА</h3>
        <input type="number" id="bet-input" class="input-bet" placeholder="0">
        <div style="display:flex; gap:10px;">
            <button class="modal-btn-secondary" onclick="closeBetModal()">ОТМЕНА</button>
            <button class="modal-btn-primary" onclick="saveBet()">ОК</button>
        </div>
    </div>
</div>

<div class="modal" id="modal-confirm">
    <div class="card">
        <h3>КУПИТЬ БОНУС?</h3>
        <p>13 игр за <b id="conf-price"></b></p>
        <div style="display:flex; gap:10px;">
            <button class="modal-btn-secondary" onclick="closeConfirm()">НЕТ</button>
            <button class="modal-btn-primary" onclick="confirmBuy()">ДА</button>
        </div>
    </div>
</div>

<div class="modal" id="modal-win">
    <div class="card">
        <h2 id="m-title" style="margin:0; font-size:26px;">БОНУС!</h2>
        <div id="m-sub" style="color:#8e8e93; font-weight:800; font-size:12px; margin-top:5px;">ВЫ ПОЛУЧИЛИ</div>
        <div id="m-num" style="color:var(--blue); font-size:50px; font-weight:900; margin:15px 0;">13</div>
        <div id="m-desc" style="font-weight:800; margin-bottom:15px;">ФРИСПИНОВ</div>
        <button class="modal-btn-primary" onclick="closeWinModal()">ОК</button>
    </div>
</div>

<div id="rules-page">
    <div onclick="openRules(false)" style="color:var(--blue); font-weight:900; padding:15px 0; cursor:pointer;">← ЗАКРЫТЬ</div>
    <h2>ТАБЛИЦА ВЫПЛАТ</h2>
    <div class="rule-grid" id="rules-list"></div>
</div>

<script src="https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js"></script>

<script>
    // ТОТ САМЫЙ ПРОШЛЫЙ ФОН (ЛОГИКА)
    particlesJS("particles-js", {
        "particles": {
            "number": { "value": 80, "density": { "enable": true, "value_area": 800 } },
            "color": { "value": "#000000" },
            "shape": { "type": "triangle", "stroke": { "width": 1, "color": "#000000" } },
            "opacity": { "value": 0.2 },
            "size": { "value": 3, "random": true },
            "line_linked": { "enable": true, "distance": 150, "color": "#000000", "opacity": 0.15, "width": 1 },
            "move": { "enable": true, "speed": 1.5, "direction": "none", "random": false, "straight": false, "out_mode": "out", "bounce": false }
        },
        "retina_detect": true
    });

    // Математика весов
    const SYMS_DATA = [
        { s: '🍭', v: 10,  w: 100 }, { s: '🍓', v: 10,  w: 100 }, { s: '🍔', v: 10,  w: 100 },
        { s: '🐯', v: 20,  w: 60 },  { s: '🦍', v: 30,  w: 50 },  { s: '🦋', v: 40,  w: 40 },
        { s: '🐷', v: 50,  w: 30 },  { s: '🤖', v: 100, w: 15 },  { s: '🥶', v: 200, w: 8 },
        { s: '😈', v: 300, w: 4 },   { s: '👹', v: 500, w: 2 }
    ];
    const LINES = [[0,1,2,3,4],[5,6,7,8,9],[10,11,12,13,14],[15,16,17,18,19],[0,6,12,18,14],[15,11,7,3,9],[0,6,10,16,14],[5,11,17,11,5],[0,5,10,15,10],[4,9,14,19,14],[1,6,11,16,11],[3,8,13,18,13],[0,1,7,13,14],[15,16,12,8,9],[5,0,1,2,7],[10,15,16,17,12],[0,6,2,8,4],[15,11,17,13,19],[5,1,7,3,9],[10,16,12,18,14]];

    let balance = 5000000, bet = 5000, fs = 0, isSpinning = false, isAuto = false, isTurbo = false, fsWin = 0;
    let stickies = new Map();

    function getRandomSymbol() {
        let total = SYMS_DATA.reduce((a, b) => a + b.w, 0);
        let r = Math.random() * total;
        for (let s of SYMS_DATA) { if (r < s.w) return s.s; r -= s.w; }
        return SYMS_DATA[0].s;
    }

    function openGame() {
        document.getElementById('hub-page').style.display = 'none';
        document.getElementById('slot-page').style.display = 'block';
        if(!document.querySelector('.cell')) initGame();
    }

    function backToHub() {
        if(isSpinning) return;
        isAuto = false; updateBtn();
        document.getElementById('slot-page').style.display = 'none';
        document.getElementById('hub-page').style.display = 'block';
    }

    function initGame() {
        const g = document.getElementById('grid'); g.innerHTML = '';
        for(let i=0; i<20; i++) g.innerHTML += `<div class="cell">${getRandomSymbol()}</div>`;
        const rl = document.getElementById('rules-list');
        SYMS_DATA.sort((a,b) => b.v - a.v).forEach(i => rl.innerHTML += `<div class="rule-card"><span class="rule-emoji">${i.s}</span><span class="rule-txt">x${i.v}</span></div>`);
        rl.innerHTML += `<div class="rule-card special-rule"><span class="rule-emoji">💰</span><span class="rule-txt">БОНУС (3+)</span></div>`;
        rl.innerHTML += `<div class="rule-card special-rule"><span class="rule-emoji">🥈/🥉</span><span class="rule-txt">WILD (x2/x3)</span></div>`;
        updateBetUI();
    }

    function updateBetUI() {
        document.getElementById('bet-display').innerText = "$"+bet.toLocaleString();
        document.getElementById('buy-price').innerText = (bet*20).toLocaleString();
        document.getElementById('conf-price').innerText = "$"+(bet*20).toLocaleString();
    }

    function openBetModal() { if(!isSpinning) document.getElementById('modal-bet').style.display = 'flex'; }
    function closeBetModal() { document.getElementById('modal-bet').style.display = 'none'; }
    function saveBet() {
        let v = parseInt(document.getElementById('bet-input').value);
        if(v > 0 && v <= balance) { bet = v; updateBetUI(); closeBetModal(); }
    }

    function handleSpin() { if(!isSpinning) startSpin(); else isAuto = false; }

    async function startSpin() {
        if(balance < bet && fs === 0) { isAuto = false; updateBtn(); return; }
        isSpinning = true; updateBtn();
        if(fs === 0) { balance -= bet; updateBal(); }
        document.getElementById('win-text').innerText = "...";

        const cells = document.querySelectorAll('.cell');
        cells.forEach(c => c.classList.remove('win-pulse', 'spinning'));

        for(let col=0; col<5; col++) {
            for(let row=0; row<4; row++) {
                let idx = col + row*5;
                if(!stickies.has(idx)) {
                    let r = Math.random(), s;
                    if (r > 0.997) s = '💰';
                    else if (r > 0.992) s = '🥉';
                    else if (r > 0.985) s = '🥈';
                    else s = getRandomSymbol();
                    cells[idx].innerText = s;
                    cells[idx].classList.add('spinning');
                }
            }
            if(!isTurbo) await new Promise(r => setTimeout(r, 60));
        }
        setTimeout(checkWins, isTurbo ? 100 : 300);
    }

    function checkWins() {
        const cells = document.querySelectorAll('.cell'), grid = Array.from(cells).map(c => c.innerText);
        let win = 0, winners = new Set();

        LINES.forEach(line => {
            let first = grid[line[0]];
            if(first === '💰') return;
            let ms = (first === '🥈' || first === '🥉') ? null : first;
            let count = 1, mult = (first === '🥈' ? 2 : (first === '🥉' ? 3 : 1));
            for(let i=1; i<5; i++){
                let cur = grid[line[i]];
                if(!ms && cur !== '🥈' && cur !== '🥉' && cur !== '💰') ms = cur;
                if(cur === ms || cur === '🥈' || cur === '🥉') {
                    count++;
                    if(cur === '🥈') mult *= 2; if(cur === '🥉') mult *= 3;
                } else break;
            }
            if(count === 5 && ms) {
                win += (bet/20) * SYMS_DATA.find(s => s.s === ms).v * mult;
                line.forEach(i => winners.add(i));
            }
        });

        if(win > 0) {
            winners.forEach(i => cells[i].classList.add('win-pulse'));
            document.getElementById('win-text').innerText = "$" + Math.floor(win).toLocaleString();
        } else document.getElementById('win-text').innerText = " ";

        if(fs > 0) {
            grid.forEach((s, i) => { if((s==='🥈' || s==='🥉') && !stickies.has(i)) { stickies.set(i, s); cells[i].classList.add('sticky'); } });
            fsWin += win;
        }
        balance += win; updateBal();

        if(grid.filter(x => x === '💰').length >= 3 && fs === 0) {
            setTimeout(() => { showWinModal("БОНУС!", 13, "ФРИСПИНОВ"); fs = 13; }, 500);
        } else if(fs > 0) {
            fs--; document.getElementById('fs-count').innerText = fs;
            if(fs === 0) setTimeout(() => { showWinModal("ИТОГ", fsWin, "ВЫИГРАНО"); fsWin=0; }, 600);
            else setTimeout(startSpin, isTurbo ? 200 : 1000);
        } else {
            isSpinning = false; updateBtn();
            if(isAuto) startSpin();
        }
    }

    function showWinModal(t, n, d) {
        document.getElementById('m-title').innerText = t;
        document.getElementById('m-num').innerText = n.toLocaleString();
        document.getElementById('m-desc').innerText = d;
        document.getElementById('modal-win').style.display = 'flex';
    }

    function closeWinModal() {
        document.getElementById('modal-win').style.display = 'none';
        if(fs > 0) { 
            document.getElementById('fs-label').style.visibility = 'visible'; 
            startSpin(); 
        } else { 
            document.getElementById('fs-label').style.visibility = 'hidden'; 
            
            // ИСПРАВЛЕНО: Удаляем желтые рамки Wild-символов после бонуса
            stickies.clear(); 
            document.querySelectorAll('.cell').forEach(c => c.classList.remove('sticky', 'win-pulse')); 
            
            isSpinning = false; 
            updateBtn(); 
            if(isAuto) startSpin(); 
        }
    }

    function updateBal() { let v = Math.floor(balance).toLocaleString(); document.getElementById('bal-val').innerText = v; document.getElementById('hub-bal-val').innerText = v; }
    function updateBtn() { document.getElementById('svg-play').style.display = (isSpinning || isAuto) ? 'none' : 'block'; document.getElementById('svg-stop').style.display = (isSpinning || isAuto) ? 'block' : 'none'; }
    function toggle(t) { if(t==='turbo') { isTurbo=!isTurbo; document.getElementById('t-turbo').classList.toggle('active'); } if(t==='auto') { isAuto=!isAuto; document.getElementById('t-auto').classList.toggle('active'); if(isAuto && !isSpinning) startSpin(); } }
    function askBuyBonus() { if(balance>=bet*20 && !isSpinning) document.getElementById('modal-confirm').style.display='flex'; }
    function closeConfirm() { document.getElementById('modal-confirm').style.display='none'; }
    function confirmBuy() { closeConfirm(); balance-=bet*20; updateBal(); showWinModal("БОНУС!", 13, "ФРИСПИНОВ"); fs=13; }
    function openRules(v) { document.getElementById('rules-page').style.display = v ? 'block' : 'none'; }
</script>
</body>
</html>
