<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1.0,maximum-scale=1.0,user-scalable=no">
<title>ZapZone ⚡</title>
<script src="https://www.gstatic.com/firebasejs/10.12.0/firebase-app-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.12.0/firebase-auth-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.12.0/firebase-database-compat.js"></script>
<script src="https://checkout.razorpay.com/v1/checkout.js"></script>
<style>
*{margin:0;padding:0;box-sizing:border-box;-webkit-tap-highlight-color:transparent}
body{font-family:'Segoe UI',system-ui,sans-serif;background:#0d0d1a;color:#f0f0f0;max-width:440px;margin:0 auto;min-height:100vh;overflow-x:hidden}
.page{display:none;min-height:100vh;flex-direction:column}.page.active{display:flex}
button{font-family:inherit;cursor:pointer;border:none;outline:none}
input,textarea{font-family:inherit;outline:none}
.btn{width:100%;padding:13px;border-radius:13px;font-weight:800;font-size:15px;color:#fff;border:none;cursor:pointer;margin-bottom:10px}
.btn-p{background:linear-gradient(135deg,#a855f7,#4361ee)}
.btn-g{background:linear-gradient(135deg,#06d6a0,#4361ee)}
.btn-r{background:linear-gradient(135deg,#ff6b6b,#fb8500)}
.btn-y{background:linear-gradient(135deg,#ffe66d,#fb8500);color:#1a1a35}
.btn-out{background:none;border:2px solid #2a2a50;color:#7070a0;border-radius:13px;padding:12px;font-weight:700;font-size:14px;width:100%;margin-bottom:10px}
.inp{width:100%;background:#0d0d1a;border:2px solid #2a2a50;border-radius:12px;padding:11px 15px;color:#f0f0f0;font-size:15px;font-family:inherit;transition:border-color 0.2s;display:block;margin-bottom:13px}
.inp:focus{border-color:#a855f7}
.lbl{font-size:11px;color:#7070a0;font-weight:700;text-transform:uppercase;letter-spacing:1px;margin-bottom:5px;display:block}
.err{background:rgba(255,107,107,0.1);color:#ff6b6b;border-radius:10px;padding:8px 12px;font-size:13px;text-align:center;margin-bottom:10px;display:none}
.card{background:#1a1a35;border-radius:18px;padding:16px}
/* SPLASH */
#splash{background:linear-gradient(135deg,#0d0d1a,#1a1a35);align-items:center;justify-content:center;text-align:center}
.sp-icon{font-size:72px;animation:zap 0.8s ease-in-out infinite alternate}
@keyframes zap{from{transform:scale(1) rotate(-5deg)}to{transform:scale(1.15) rotate(5deg)}}
@keyframes ld{from{width:0}to{width:100%}}
@keyframes spin{to{transform:rotate(360deg)}}
@keyframes slideUp{from{transform:translateY(20px);opacity:0}to{transform:translateY(0);opacity:1}}
@keyframes pop{0%{transform:scale(0)}50%{transform:scale(1.2)}100%{transform:scale(1)}}
@keyframes shine{0%,100%{opacity:1}50%{opacity:0.6}}
/* AUTH */
#login,#register{background:#0d0d1a;align-items:center;justify-content:center;padding:20px;overflow-y:auto}
.auth-box{width:100%;max-width:380px}
.auth-logo{text-align:center;margin-bottom:20px}
.auth-card{background:#1a1a35;border-radius:22px;padding:26px 22px;box-shadow:0 16px 48px rgba(0,0,0,0.3)}
/* NAV */
.nav{position:fixed;bottom:0;left:50%;transform:translateX(-50%);width:100%;max-width:440px;background:#111128;border-top:1px solid #2a2a50;display:flex;justify-content:space-around;padding:8px 0;z-index:100}
.nb{background:none;border:none;color:#7070a0;display:flex;flex-direction:column;align-items:center;gap:1px;padding:3px 10px;font-size:9px;font-weight:500;transition:color 0.2s;font-family:inherit}
.nb.on{color:#a855f7;font-weight:800}
.nb .ni{font-size:20px}
/* CHAT */
.ch-hdr{background:#111128;border-bottom:1px solid #2a2a50;padding:10px 14px;display:flex;align-items:center;justify-content:space-between}
.ch-msgs{flex:1;overflow-y:auto;padding:10px 12px;display:flex;flex-direction:column;gap:8px;background:#0a0a18;min-height:0}
.msg-row{display:flex;gap:6px;align-items:flex-end}
.msg-row.me{justify-content:flex-end}
.msg-bbl{border-radius:18px 18px 18px 4px;padding:9px 13px;font-size:14px;line-height:1.5;background:#1a1a35;color:#f0f0f0;position:relative}
.msg-row.me .msg-bbl{border-radius:18px 18px 4px 18px;background:linear-gradient(135deg,#a855f7,#4361ee);color:#fff}
.msg-reactions{display:flex;gap:4px;margin-top:4px;flex-wrap:wrap}
.rxn-btn{background:rgba(255,255,255,0.1);border:1px solid rgba(255,255,255,0.2);border-radius:20px;padding:2px 8px;font-size:12px;cursor:pointer;display:flex;align-items:center;gap:3px;color:#f0f0f0}
.rxn-btn.active{background:rgba(168,85,247,0.3);border-color:#a855f7}
.add-rxn{background:none;border:1px solid #2a2a50;border-radius:20px;padding:2px 8px;font-size:12px;cursor:pointer;color:#7070a0}
.rxn-picker{display:none;gap:4px;margin-top:4px}
.rxn-picker.open{display:flex}
.rxn-pick-btn{background:#1a1a35;border:1px solid #2a2a50;border-radius:8px;padding:4px 8px;font-size:16px;cursor:pointer}
.emoji-bar{display:flex;gap:5px;padding:6px 12px;overflow-x:auto;background:#0a0a18}
.eb{background:none;border:1px solid #2a2a50;border-radius:10px;padding:4px 7px;font-size:15px;flex-shrink:0}
.ch-inp-row{display:flex;gap:8px;padding:8px 12px;background:#111128;border-top:1px solid #2a2a50}
.ch-inp{flex:1;background:#0a0a18;border:2px solid #2a2a50;border-radius:22px;padding:9px 14px;color:#f0f0f0;font-size:14px;font-family:inherit}
.ch-inp:focus{border-color:#a855f7;outline:none}
.send-btn{background:linear-gradient(135deg,#a855f7,#4361ee);border:none;border-radius:50%;width:42px;height:42px;font-size:18px;flex-shrink:0}
/* QUIZ */
.pp{padding:14px}
.ptitle{font-size:20px;font-weight:900}
.psub{color:#7070a0;font-size:12px;margin-top:2px}
.cat-grid{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-top:14px}
.cat-card{background:#1a1a35;border:2px solid #2a2a50;border-radius:16px;padding:16px 12px;cursor:pointer;text-align:center;font-family:inherit;transition:all 0.2s}
.cat-card:active{transform:scale(0.97)}
.q-hdr{display:flex;align-items:center;justify-content:space-between;margin-bottom:12px}
.q-back{background:none;border:none;color:#7070a0;font-size:22px;cursor:pointer}
.q-prog{background:#1a1a35;border-radius:8px;height:6px;margin-bottom:5px;overflow:hidden}
.q-pf{height:100%;border-radius:8px;transition:width 0.4s}
.q-card{background:#1a1a35;border-radius:18px;padding:20px 16px;margin-bottom:14px;border-left:4px solid #06d6a0}
.q-opts{display:flex;flex-direction:column;gap:8px}
.q-opt{background:#1a1a35;border:2px solid #2a2a50;border-radius:13px;padding:12px 14px;color:#f0f0f0;font-size:14px;font-weight:600;text-align:left;cursor:pointer;font-family:inherit;transition:all 0.2s}
.q-opt.correct{background:#0a2e1e;border-color:#06d6a0}
.q-opt.wrong{background:#2e0a0a;border-color:#ff6b6b}
.timer-ring{display:flex;align-items:center;justify-content:center;width:40px;height:40px;border-radius:50%;font-weight:900;font-size:16px;border:3px solid #a855f7;color:#a855f7}
.timer-ring.warn{border-color:#ff6b6b;color:#ff6b6b;animation:shine 0.5s infinite}
/* ROOMS */
.room-code{font-size:32px;font-weight:900;letter-spacing:6px;color:#ffe66d;text-align:center;padding:16px;background:#1a1a35;border-radius:14px;margin:10px 0}
.room-list{display:flex;flex-direction:column;gap:10px}
.room-item{background:#1a1a35;border:2px solid #2a2a50;border-radius:14px;padding:14px;cursor:pointer;display:flex;align-items:center;gap:12px}
/* SHOP */
.shop-grid{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-top:10px}
.shop-item{background:#1a1a35;border:2px solid #2a2a50;border-radius:14px;padding:14px;text-align:center}
.shop-item.owned{border-color:#06d6a0}
.spin-wheel{width:200px;height:200px;border-radius:50%;margin:0 auto;position:relative;overflow:hidden;border:4px solid #a855f7}
.spin-result{font-size:24px;font-weight:900;text-align:center;margin:12px 0;min-height:36px}
/* PROFILE / BADGES */
.badge-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;margin-top:10px}
.badge-item{background:#1a1a35;border-radius:14px;padding:12px 8px;text-align:center;border:2px solid #2a2a50}
.badge-item.earned{border-color:#ffe66d;background:rgba(255,230,109,0.08)}
.badge-icon{font-size:28px;margin-bottom:4px}
.badge-name{font-size:10px;font-weight:700;color:#7070a0}
.badge-item.earned .badge-name{color:#ffe66d}
/* DAILY CHALLENGE */
.daily-card{background:linear-gradient(135deg,#1a1a35,#0f0f28);border:2px solid #ffe66d;border-radius:16px;padding:16px;margin-bottom:14px;position:relative;overflow:hidden}
.daily-glow{position:absolute;top:-20px;right:-20px;width:80px;height:80px;background:rgba(255,230,109,0.15);border-radius:50%}
/* LEADERBOARD */
.lb-row{display:flex;align-items:center;gap:10px;background:#1a1a35;border:2px solid #2a2a50;border-radius:14px;padding:10px 12px;margin-bottom:8px}
.lb-row.me{border-color:#a855f7;background:rgba(168,85,247,0.08)}
/* ANNOUNCEMENT */
.announce-banner{background:linear-gradient(135deg,#a855f7,#4361ee);border-radius:14px;padding:12px 16px;margin-bottom:12px;display:none}
/* SWATCH */
.sw-wrap{display:flex;gap:6px;flex-wrap:wrap}
.sw-btn{border:2px solid transparent;border-radius:10px;background:none;padding:3px;cursor:pointer}
.sw-btn.sel{border-color:#ffe66d}
.sw-dot{width:22px;height:22px;border-radius:50%}
.txt-opts{display:flex;gap:6px;flex-wrap:wrap}
.txt-opt{border:2px solid #2a2a50;border-radius:10px;background:#1a1a35;padding:5px 10px;cursor:pointer;color:#f0f0f0;font-size:11px;font-family:inherit}
.txt-opt.sel{border-color:#a855f7;background:rgba(168,85,247,0.2)}
.g-row{display:flex;gap:8px;margin-bottom:4px}
.g-btn{flex:1;background:#1a1a35;border:2px solid #2a2a50;border-radius:10px;padding:9px;color:#f0f0f0;font-weight:700;cursor:pointer;font-family:inherit}
.g-btn.sel{border-color:#a855f7;background:rgba(168,85,247,0.2)}
/* VIP */
.vip-card{background:linear-gradient(135deg,#1a1035,#0d0820);border:2px solid #ffe66d;border-radius:18px;padding:18px;margin-bottom:14px;position:relative;overflow:hidden}
.vip-glow{position:absolute;top:-30px;right:-30px;width:100px;height:100px;background:rgba(255,230,109,0.12);border-radius:50%}
.vip-badge{display:inline-block;background:linear-gradient(135deg,#ffe66d,#fb8500);border-radius:20px;padding:3px 12px;font-size:11px;font-weight:900;color:#1a1a35;margin-bottom:8px}
.vip-active{background:linear-gradient(135deg,#064e3b,#065f46);border-color:#06d6a0}
.coin-pack{background:#1a1a35;border:2px solid #2a2a50;border-radius:14px;padding:14px;text-align:center;cursor:pointer;transition:all 0.2s}
.coin-pack:active{transform:scale(0.97)}
.coin-pack.popular{border-color:#a855f7;position:relative}
.coin-pack .pop-tag{position:absolute;top:-8px;left:50%;transform:translateX(-50%);background:#a855f7;border-radius:10px;padding:2px 10px;font-size:10px;font-weight:800;color:#fff;white-space:nowrap}
.ad-card{background:linear-gradient(135deg,#0f1f3d,#0d0d1a);border:2px solid #4361ee;border-radius:16px;padding:16px;margin-bottom:14px}
.ad-timer{font-size:32px;font-weight:900;color:#4361ee;text-align:center;margin:8px 0}
.ad-progress{background:#0d0d1a;border-radius:8px;height:8px;overflow:hidden;margin:8px 0}
.ad-prog-fill{height:100%;background:linear-gradient(90deg,#4361ee,#a855f7);border-radius:8px;transition:width 0.5s}
/* MODAL */
.modal-bg{display:none;position:fixed;inset:0;background:rgba(0,0,0,0.7);z-index:200;align-items:center;justify-content:center}
.modal-bg.open{display:flex}
.modal{background:#1a1a35;border-radius:22px;padding:24px 20px;width:90%;max-width:360px;animation:slideUp 0.3s ease}
.modal-title{font-size:18px;font-weight:900;margin-bottom:16px;text-align:center}
</style>
</head>
<body>

<!-- SPLASH -->
<div id="splash" class="page active">
  <div class="sp-icon">⚡</div>
  <div style="font-size:34px;font-weight:900;color:#ffe66d;margin-top:10px">ZapZone</div>
  <div style="color:rgba(255,255,255,0.6);font-size:11px;letter-spacing:3px;text-transform:uppercase;margin-top:4px">Quiz · Chat · Dominate</div>
  <div style="width:180px;height:5px;background:rgba(255,255,255,0.15);border-radius:5px;overflow:hidden;margin-top:24px">
    <div style="width:0;height:100%;background:#ffe66d;border-radius:5px;animation:ld 1.8s ease-out forwards"></div>
  </div>
</div>

<!-- LOGIN -->
<div id="login" class="page">
  <div class="auth-box">
    <div class="auth-logo"><div style="font-size:46px">⚡</div><div style="font-size:26px;font-weight:900;color:#ffe66d">ZapZone</div><div style="color:#7070a0;font-size:11px;letter-spacing:2px;text-transform:uppercase">Quiz · Chat · Dominate</div></div>
    <div class="auth-card">
      <div style="font-size:18px;font-weight:900;text-align:center;margin-bottom:16px">🔑 Login</div>
      <label class="lbl">Username</label><input id="l-user" class="inp" placeholder="your username">
      <label class="lbl">Password</label><input id="l-pass" class="inp" type="password" placeholder="password">
      <div id="l-err" class="err"></div>
      <button class="btn btn-p" onclick="doLogin()">⚡ Enter ZapZone</button>
      <button class="btn-out" onclick="showPage('register')">✨ Create Account</button>
    </div>
  </div>
</div>

<!-- REGISTER -->
<div id="register" class="page">
  <div class="auth-box" style="padding:16px;width:100%;max-width:380px;margin:0 auto">
    <div class="auth-logo" style="margin-bottom:12px"><div style="font-size:36px">✨</div><div style="font-size:20px;font-weight:900;color:#ffe66d">Join ZapZone!</div><div style="color:#7070a0;font-size:12px">Get 100 🪙 free coins!</div></div>
    <div style="text-align:center;margin-bottom:12px"><div style="display:inline-block;background:#1a1a35;border-radius:18px;padding:12px 20px"><div id="reg-av"></div><div id="reg-av-name" style="font-weight:800;margin-top:4px;font-size:13px">Your Name</div></div></div>
    <div class="auth-card">
      <label class="lbl">Display Name</label><input id="r-name" class="inp" placeholder="e.g. Alex, Priya..." oninput="updRegAv()">
      <label class="lbl">Username</label><input id="r-user" class="inp" placeholder="min 3 chars">
      <label class="lbl">Password</label><input id="r-pass" class="inp" type="password" placeholder="min 4 chars">
      <label class="lbl">Confirm Password</label><input id="r-pass2" class="inp" type="password" placeholder="same again">
      <div style="border-top:1px solid #2a2a50;padding-top:12px;margin-bottom:12px">
        <div class="lbl" style="margin-bottom:8px">Quick Avatar</div>
        <div style="margin-bottom:8px"><div class="lbl">Gender</div><div class="g-row"><button class="g-btn sel" id="g-boy" onclick="setRG('Boy')">👦 Boy</button><button class="g-btn" id="g-girl" onclick="setRG('Girl')">👧 Girl</button></div></div>
        <div style="margin-bottom:8px"><div class="lbl">Skin</div><div class="sw-wrap" id="r-skin"></div></div>
        <div style="margin-bottom:8px"><div class="lbl">Expression</div><div class="txt-opts" id="r-expr"></div></div>
        <div><div class="lbl">Accessory</div><div class="txt-opts" id="r-acc"></div></div>
      </div>
      <div id="r-err" class="err"></div>
      <button class="btn btn-g" onclick="doRegister()">🎉 Join Now!</button>
      <button class="btn-out" onclick="showPage('login')">← Back</button>
    </div>
  </div>
</div>

<!-- APP -->
<div id="app" class="page">
  <div id="ac" style="flex:1;overflow-y:auto;padding-bottom:62px">

    <!-- ANNOUNCEMENT BANNER -->
    <div class="announce-banner" id="ann-banner">
      <div style="font-weight:800;font-size:13px">📢 <span id="ann-text"></span></div>
    </div>

    <!-- CHAT TAB -->
    <div id="t-chat" style="display:flex;flex-direction:column;height:calc(100vh - 62px)">
      <div class="ch-hdr">
        <div><div style="font-weight:900;font-size:16px">⚡ ZapZone Chat</div><div id="online-c" style="color:#06d6a0;font-size:11px">● Loading...</div></div>
        <div style="display:flex;align-items:center;gap:6px">
          <button style="background:#1a1a35;border:1px solid #2a2a50;border-radius:16px;padding:4px 10px;color:#f0f0f0;font-size:13px" onclick="toggleTheme()">☀️</button>
          <div id="hdr-av"></div>
        </div>
      </div>
      <div class="ch-msgs" id="ch-msgs">
        <div style="text-align:center;padding-top:50px;color:#7070a0"><div style="font-size:40px;margin-bottom:10px">⚡</div><div style="font-weight:700">Be the first to say something!</div></div>
      </div>
      <div class="emoji-bar">
        <button class="eb" onclick="addE('👋')">👋</button><button class="eb" onclick="addE('😂')">😂</button><button class="eb" onclick="addE('🔥')">🔥</button><button class="eb" onclick="addE('🎉')">🎉</button><button class="eb" onclick="addE('❤️')">❤️</button><button class="eb" onclick="addE('💯')">💯</button><button class="eb" onclick="addE('⚡')">⚡</button><button class="eb" onclick="addE('😎')">😎</button>
      </div>
      <div class="ch-inp-row">
        <input id="ch-inp" class="ch-inp" placeholder="Say something..." onkeydown="if(event.key==='Enter')sendMsg()">
        <button class="send-btn" onclick="sendMsg()">⚡</button>
      </div>
    </div>

    <!-- QUIZ TAB -->
    <div id="t-quiz" class="pp" style="display:none">
      <!-- Daily Challenge Card -->
      <div class="daily-card" id="daily-card">
        <div class="daily-glow"></div>
        <div style="display:flex;align-items:center;justify-content:space-between">
          <div><div style="font-size:11px;color:#ffe66d;font-weight:700;text-transform:uppercase;letter-spacing:1px">🌟 Daily Challenge</div><div style="font-weight:900;font-size:16px;margin-top:2px" id="daily-title">Today's Quiz</div><div style="font-size:12px;color:#7070a0;margin-top:2px">Bonus: +100 🪙 coins!</div></div>
          <button id="daily-btn" class="btn btn-y" style="width:auto;padding:10px 16px;margin:0;font-size:13px" onclick="startDaily()">Play!</button>
        </div>
      </div>
      <!-- Categories -->
      <div id="qz-cats">
        <div style="display:flex;justify-content:space-between;align-items:center"><div><div class="ptitle">🎯 Quiz Arena</div><div class="psub">Pick a category!</div></div><div id="qz-coins" style="background:#1a1a35;border-radius:10px;padding:5px 12px;color:#ffe66d;font-weight:700">🪙 0</div></div>
        <div class="cat-grid" id="cat-grid"></div>
        <!-- Mode toggle -->
        <div style="margin-top:12px;background:#1a1a35;border-radius:14px;padding:12px">
          <div style="font-weight:800;margin-bottom:8px;font-size:13px">⚙️ Quiz Mode</div>
          <div style="display:flex;gap:8px">
            <button id="mode-normal" class="g-btn sel" onclick="setMode('normal')" style="font-size:12px;padding:8px">Normal</button>
            <button id="mode-timer" class="g-btn" onclick="setMode('timer')" style="font-size:12px;padding:8px">⏱️ Timer (10s)</button>
          </div>
        </div>
        <!-- Leaderboard mini -->
        <div style="margin-top:12px"><div style="font-weight:800;margin-bottom:8px">🏆 Top Players</div><div id="mini-lb"></div></div>
      </div>
      <!-- Game -->
      <div id="qz-game" style="display:none">
        <div class="q-hdr">
          <button class="q-back" onclick="backCats()">←</button>
          <div id="q-cat-lbl" style="font-weight:800;font-size:15px"></div>
          <div style="display:flex;align-items:center;gap:6px">
            <div id="q-timer" class="timer-ring" style="display:none">10</div>
            <div id="q-streak" style="background:#ff6b6b;border-radius:8px;padding:3px 8px;color:#fff;font-weight:700;font-size:12px;display:none">🔥x0</div>
          </div>
        </div>
        <div class="q-prog"><div class="q-pf" id="q-pf"></div></div>
        <div id="q-cnt" style="color:#7070a0;font-size:11px;text-align:right;margin-bottom:12px"></div>
        <div class="q-card" id="q-card"><div id="q-txt" style="font-size:15px;font-weight:700;line-height:1.5;text-align:center"></div></div>
        <div class="q-opts" id="q-opts"></div>
      </div>
      <!-- Done -->
      <div id="qz-done" style="display:none;text-align:center;padding-top:16px">
        <div id="done-icon" style="font-size:60px;margin-bottom:8px"></div>
        <div id="done-title" style="font-size:24px;font-weight:900;margin-bottom:4px"></div>
        <div id="done-sub" style="color:#7070a0;font-size:15px;margin-bottom:16px"></div>
        <div id="done-av" style="display:inline-block"></div>
        <div id="done-reward" style="color:#06d6a0;font-weight:800;margin:10px 0 20px;font-size:14px"></div>
        <div id="done-badge" style="display:none;background:rgba(255,230,109,0.1);border:1px solid #ffe66d;border-radius:12px;padding:10px;margin-bottom:16px;font-size:13px">🏅 New Badge Earned!</div>
        <button class="btn btn-p" onclick="playAgain()">🔄 Play Again</button>
        <button class="btn btn-r" onclick="backCats()">📚 Change Category</button>
      </div>
    </div>

    <!-- ROOMS TAB -->
    <div id="t-rooms" class="pp" style="display:none">
      <div class="ptitle">🏠 Private Rooms</div>
      <div class="psub" style="margin-bottom:14px">Create or join a room with friends</div>
      <!-- Create room -->
      <div class="card" style="margin-bottom:12px">
        <div style="font-weight:800;margin-bottom:10px">➕ Create Room</div>
        <label class="lbl">Room Name</label>
        <input id="room-name" class="inp" placeholder="e.g. My Squad Room">
        <button class="btn btn-p" style="margin-bottom:0" onclick="createRoom()">Create Room</button>
      </div>
      <!-- Join room -->
      <div class="card" style="margin-bottom:14px">
        <div style="font-weight:800;margin-bottom:10px">🔑 Join Room</div>
        <label class="lbl">Enter Room Code</label>
        <div style="display:flex;gap:8px">
          <input id="join-code" class="inp" style="margin-bottom:0;flex:1" placeholder="6-digit code" maxlength="6">
          <button class="btn btn-g" style="width:auto;padding:0 16px;margin:0" onclick="joinRoom()">Join</button>
        </div>
      </div>
      <!-- My rooms -->
      <div><div style="font-weight:800;margin-bottom:10px">📋 My Rooms</div><div id="my-rooms"><div style="color:#7070a0;font-size:13px">No rooms yet — create one!</div></div></div>
    </div>

    <!-- ROOM CHAT -->
    <div id="t-roomchat" style="display:none;flex-direction:column;height:calc(100vh - 62px)">
      <div class="ch-hdr">
        <div style="display:flex;align-items:center;gap:8px">
          <button class="q-back" onclick="leaveRoomChat()">←</button>
          <div><div id="rc-name" style="font-weight:900;font-size:15px"></div><div id="rc-code" style="color:#7070a0;font-size:11px"></div></div>
        </div>
        <div id="rc-members" style="color:#06d6a0;font-size:11px"></div>
      </div>
      <div class="ch-msgs" id="rc-msgs">
        <div style="text-align:center;padding-top:40px;color:#7070a0"><div style="font-size:36px">🏠</div><div style="margin-top:8px">Welcome to the room!</div></div>
      </div>
      <div class="ch-inp-row">
        <input id="rc-inp" class="ch-inp" placeholder="Say something..." onkeydown="if(event.key==='Enter')sendRoomMsg()">
        <button class="send-btn" onclick="sendRoomMsg()">⚡</button>
      </div>
    </div>

    <!-- SHOP TAB -->
    <div id="t-shop" class="pp" style="display:none">
      <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:14px">
        <div><div class="ptitle">🛒 ZapZone Shop</div><div class="psub">Coins, VIP & more!</div></div>
        <div id="shop-coins" style="background:#1a1a35;border-radius:10px;padding:5px 12px;color:#ffe66d;font-weight:700">🪙 0</div>
      </div>

      <!-- VIP MEMBERSHIP -->
      <div class="vip-card" id="vip-card">
        <div class="vip-glow"></div>
        <div class="vip-badge" id="vip-badge-lbl">👑 VIP MEMBERSHIP</div>
        <div style="font-weight:900;font-size:18px;margin-bottom:4px" id="vip-title">Unlock ZapZone VIP!</div>
        <div style="color:#7070a0;font-size:12px;margin-bottom:10px" id="vip-desc">Get premium perks every month</div>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:6px;margin-bottom:12px">
          <div style="background:rgba(255,230,109,0.08);border-radius:10px;padding:8px;font-size:12px">⚡ 2x Quiz Coins</div>
          <div style="background:rgba(255,230,109,0.08);border-radius:10px;padding:8px;font-size:12px">🎰 Unlimited Spins</div>
          <div style="background:rgba(255,230,109,0.08);border-radius:10px;padding:8px;font-size:12px">👑 VIP Badge</div>
          <div style="background:rgba(255,230,109,0.08);border-radius:10px;padding:8px;font-size:12px">🎨 Exclusive Avatars</div>
          <div style="background:rgba(255,230,109,0.08);border-radius:10px;padding:8px;font-size:12px">🏆 VIP Leaderboard</div>
          <div style="background:rgba(255,230,109,0.08);border-radius:10px;padding:8px;font-size:12px">💬 Private Rooms ∞</div>
        </div>
        <div id="vip-btn-wrap">
          <button class="btn btn-y" style="font-size:16px" onclick="buyVIP()">👑 Get VIP — ₹199/month</button>
        </div>
        <div id="vip-active-msg" style="display:none;text-align:center;color:#06d6a0;font-weight:800;font-size:14px">✅ You are VIP! Expires: <span id="vip-exp"></span></div>
      </div>

      <!-- REWARDED ADS -->
      <div class="ad-card" id="ad-card">
        <div style="font-weight:900;font-size:15px;margin-bottom:4px">📺 Watch Ad — Earn Coins!</div>
        <div style="color:#7070a0;font-size:12px;margin-bottom:10px">Watch a short ad to earn <span style="color:#ffe66d;font-weight:700">25 🪙 coins</span>. Available 5x per day.</div>
        <div id="ad-count-disp" style="font-size:12px;color:#4361ee;margin-bottom:10px;font-weight:700">✅ <span id="ad-left">5</span> watches remaining today</div>
        <div id="ad-watching" style="display:none">
          <div style="text-align:center;font-size:12px;color:#7070a0;margin-bottom:4px">Ad playing... don't close!</div>
          <div class="ad-timer" id="ad-timer">30</div>
          <div class="ad-progress"><div class="ad-prog-fill" id="ad-pf" style="width:0%"></div></div>
        </div>
        <button class="btn" id="ad-btn" onclick="watchAd()" style="background:linear-gradient(135deg,#4361ee,#a855f7);margin-bottom:0">📺 Watch Ad (+25 🪙)</button>
      </div>

      <!-- COIN PACKS -->
      <div style="margin-bottom:14px">
        <div style="font-weight:900;font-size:16px;margin-bottom:10px">🪙 Coin Packs</div>
        <div style="display:flex;flex-direction:column;gap:10px">
          <div class="coin-pack" onclick="buyCoins('starter')">
            <div style="display:flex;align-items:center;justify-content:space-between">
              <div style="display:flex;align-items:center;gap:12px">
                <div style="font-size:32px">🪙</div>
                <div><div style="font-weight:900;font-size:16px">500 Coins</div><div style="color:#7070a0;font-size:12px">Starter Pack</div></div>
              </div>
              <button style="background:linear-gradient(135deg,#06d6a0,#4361ee);border:none;border-radius:12px;padding:8px 16px;color:#fff;font-weight:800;font-size:14px;cursor:pointer">₹49</button>
            </div>
          </div>
          <div class="coin-pack popular" onclick="buyCoins('popular')" style="position:relative">
            <div class="pop-tag">🔥 MOST POPULAR</div>
            <div style="display:flex;align-items:center;justify-content:space-between;margin-top:4px">
              <div style="display:flex;align-items:center;gap:12px">
                <div style="font-size:32px">💰</div>
                <div><div style="font-weight:900;font-size:16px">1,200 Coins</div><div style="color:#7070a0;font-size:12px">Value Pack • +200 Bonus!</div></div>
              </div>
              <button style="background:linear-gradient(135deg,#a855f7,#4361ee);border:none;border-radius:12px;padding:8px 16px;color:#fff;font-weight:800;font-size:14px;cursor:pointer">₹99</button>
            </div>
          </div>
          <div class="coin-pack" onclick="buyCoins('mega')">
            <div style="display:flex;align-items:center;justify-content:space-between">
              <div style="display:flex;align-items:center;gap:12px">
                <div style="font-size:32px">💎</div>
                <div><div style="font-weight:900;font-size:16px">2,500 Coins</div><div style="color:#7070a0;font-size:12px">Mega Pack • Best Value!</div></div>
              </div>
              <button style="background:linear-gradient(135deg,#ff6b6b,#a855f7);border:none;border-radius:12px;padding:8px 16px;color:#fff;font-weight:800;font-size:14px;cursor:pointer">₹199</button>
            </div>
          </div>
        </div>
      </div>

      <!-- SPIN TO WIN -->
      <div class="card" style="margin-bottom:14px;text-align:center">
        <div style="font-weight:900;font-size:16px;margin-bottom:4px">🎰 Spin to Win!</div>
        <div style="color:#7070a0;font-size:12px;margin-bottom:12px" id="spin-cost-lbl">Cost: 50 🪙 per spin <span id="vip-spin-tag" style="display:none;color:#ffe66d;font-weight:700">(VIP: FREE!)</span></div>
        <div id="spin-wheel" style="width:160px;height:160px;border-radius:50%;margin:0 auto 12px;border:4px solid #a855f7;display:flex;align-items:center;justify-content:center;font-size:36px;transition:transform 1.5s cubic-bezier(0.17,0.67,0.12,0.99)">🎰</div>
        <div id="spin-result" class="spin-result"></div>
        <button class="btn btn-p" onclick="doSpin()">🎰 Spin Now</button>
      </div>

      <!-- AVATAR SHOP -->
      <div><div style="font-weight:900;font-size:16px;margin-bottom:10px">🎨 Avatar Shop</div>
      <div class="shop-grid" id="shop-grid"></div></div>
    </div>

    <!-- PROFILE TAB -->
    <div id="t-me" style="display:none">
      <div id="prof-view" class="pp">
        <!-- Profile card -->
        <div class="card" style="text-align:center;margin-bottom:14px">
          <div id="prof-av" style="display:inline-block"></div>
          <div id="prof-name" style="font-weight:900;font-size:19px;margin-top:6px"></div>
          <div id="prof-user" style="color:#7070a0;font-size:12px"></div>
          <div style="margin-top:10px;background:#0a0a18;border-radius:8px;height:7px;overflow:hidden"><div id="xp-bar" style="height:100%;background:linear-gradient(90deg,#a855f7,#ffe66d);transition:width 0.5s"></div></div>
          <div id="xp-lbl" style="font-size:11px;color:#7070a0;margin-top:3px"></div>
        </div>
        <!-- Stats -->
        <div style="display:flex;gap:8px;justify-content:center;margin-bottom:14px">
          <div class="card" style="min-width:70px;text-align:center;padding:10px"><div style="font-size:16px">🪙</div><div id="s-coins" style="font-weight:900;font-size:18px;color:#ffe66d">0</div><div style="font-size:10px;color:#7070a0">Coins</div></div>
          <div class="card" style="min-width:70px;text-align:center;padding:10px"><div style="font-size:16px">⚡</div><div id="s-xp" style="font-weight:900;font-size:18px;color:#a855f7">0</div><div style="font-size:10px;color:#7070a0">XP</div></div>
          <div class="card" style="min-width:70px;text-align:center;padding:10px"><div style="font-size:16px">🏆</div><div id="s-lv" style="font-weight:900;font-size:18px;color:#4ecdc4">1</div><div style="font-size:10px;color:#7070a0">Level</div></div>
        </div>
        <!-- Badges -->
        <div class="card" style="margin-bottom:14px">
          <div style="font-weight:800;margin-bottom:10px">🏅 Badges</div>
          <div class="badge-grid" id="badge-grid"></div>
        </div>
        <!-- Records -->
        <div class="card" style="margin-bottom:14px">
          <div style="font-weight:800;margin-bottom:10px">🎯 Quiz Records</div>
          <div id="rec-list"></div>
        </div>
        <!-- Actions -->
        <div style="display:flex;gap:8px;margin-bottom:10px">
          <button class="btn btn-p" style="margin:0;flex:1" onclick="showAvEd()">🎨 Edit Avatar</button>
          <button style="background:none;border:2px solid #2a2a50;border-radius:13px;padding:13px 16px;color:#7070a0;font-weight:700;font-size:13px;cursor:pointer;font-family:inherit" onclick="doLogout()">🚪 Logout</button>
        </div>
      </div>
      <!-- Avatar Editor -->
      <div id="av-ed" class="pp" style="display:none">
        <div style="display:flex;align-items:center;gap:8px;margin-bottom:14px">
          <button class="q-back" onclick="hideAvEd()">←</button>
          <div style="font-weight:900;font-size:18px">🎨 Edit Avatar</div>
        </div>
        <div style="text-align:center;margin-bottom:16px"><div style="display:inline-block;background:#1a1a35;border-radius:18px;padding:14px 22px"><div id="ed-av"></div></div></div>
        <div style="margin-bottom:8px"><div class="lbl">Gender</div><div class="g-row"><button class="g-btn" id="e-boy" onclick="setEG('Boy')">👦 Boy</button><button class="g-btn" id="e-girl" onclick="setEG('Girl')">👧 Girl</button></div></div>
        <div style="margin-bottom:8px"><div class="lbl">Skin</div><div class="sw-wrap" id="e-skin"></div></div>
        <div style="margin-bottom:8px"><div class="lbl">Hair Color</div><div class="sw-wrap" id="e-hc"></div></div>
        <div style="margin-bottom:8px"><div class="lbl">Shirt Color</div><div class="sw-wrap" id="e-sh"></div></div>
        <div style="margin-bottom:8px"><div class="lbl">Hair Style</div><div class="txt-opts" id="e-hair"></div></div>
        <div style="margin-bottom:8px"><div class="lbl">Expression</div><div class="txt-opts" id="e-expr"></div></div>
        <div style="margin-bottom:16px"><div class="lbl">Accessory</div><div class="txt-opts" id="e-acc"></div></div>
        <button class="btn btn-g" onclick="saveAv()">✅ Save Avatar</button>
      </div>
    </div>

  </div>

  <!-- NAV -->
  <div class="nav">
    <button class="nb on" id="n-chat" onclick="sw('chat')"><span class="ni">⚡</span>Chat</button>
    <button class="nb" id="n-quiz" onclick="sw('quiz')"><span class="ni">🎯</span>Quiz</button>
    <button class="nb" id="n-rooms" onclick="sw('rooms')"><span class="ni">🏠</span>Rooms</button>
    <button class="nb" id="n-shop" onclick="sw('shop')"><span class="ni">🛒</span>Shop</button>
    <button class="nb" id="n-me" onclick="sw('me')"><span class="ni">👤</span>Me</button>
  </div>
</div>

<!-- BADGE MODAL -->
<div class="modal-bg" id="badge-modal">
  <div class="modal" style="text-align:center">
    <div style="font-size:56px;margin-bottom:8px;animation:pop 0.5s ease" id="bm-icon"></div>
    <div style="font-size:20px;font-weight:900;color:#ffe66d;margin-bottom:4px" id="bm-title"></div>
    <div style="color:#7070a0;font-size:13px;margin-bottom:16px" id="bm-desc"></div>
    <button class="btn btn-y" onclick="document.getElementById('badge-modal').classList.remove('open')">🎉 Awesome!</button>
  </div>
</div>

<script>
// ─── FIREBASE ────────────────────────────────────────────────────────────────
const FC = {
  apiKey:"AIzaSyDy7Cip2itCD8gsQIuk-fHjQkGQDzTxdPc",
  authDomain:"zapzone-98727.firebaseapp.com",
  databaseURL:"https://zapzone-98727-default-rtdb.firebaseio.com",
  projectId:"zapzone-98727",
  storageBucket:"zapzone-98727.firebasestorage.app",
  messagingSenderId:"884845281907",
  appId:"1:884845281907:web:6be3cd071feb6a058f2006"
};
firebase.initializeApp(FC);
const auth = firebase.auth();
const db = firebase.database();

// ─── CONSTANTS ────────────────────────────────────────────────────────────────
const SKINS=["#FDBCB4","#F1C27D","#E0AC69","#C68642","#8D5524","#FFDBAC"];
const HCS=["#1a0a00","#4A2C2A","#C9A06A","#ffe66d","#E63946","#a855f7","#00B4D8","#06D6A0"];
const BH=["spiky","messy","short","curly","mohawk","bald"];
const GH=["ponytail","pigtails","long","bun","curly-long","bob"];
const EXPRS=["happy","wink","cool","silly","surprised","smug"];
const ACCS=["none","party-hat","sunglasses","crown","cat-ears","headphones"];
const SHIRTS=["#ff6b6b","#4361ee","#06d6a0","#fb8500","#a855f7","#4ecdc4","#f72585","#ffe66d"];
const DEF={gender:"Boy",skin:SKINS[0],hairCol:HCS[0],hair:"short",expr:"happy",acc:"none",shirt:SHIRTS[0],name:"Player"};

const BADGES=[
  {id:"firstLogin",icon:"🌟",name:"First Login",desc:"Welcome to ZapZone!"},
  {id:"quizMaster",icon:"🎓",name:"Quiz Master",desc:"Complete all 4 categories"},
  {id:"chatKing",icon:"💬",name:"Chat King",desc:"Send 20 messages"},
  {id:"streakHero",icon:"🔥",name:"Streak Hero",desc:"Get 5 correct in a row"},
  {id:"richKid",icon:"🪙",name:"Rich Kid",desc:"Earn 500+ coins"},
  {id:"dailyHero",icon:"📅",name:"Daily Hero",desc:"Complete daily challenge"},
  {id:"speedster",icon:"⚡",name:"Speedster",desc:"Win in timer mode"},
  {id:"socialite",icon:"🏠",name:"Socialite",desc:"Join a private room"},
  {id:"shopper",icon:"🛒",name:"Shopper",desc:"Buy from the shop"},
];

const SHOP_ITEMS=[
  {id:"rainbow-hair",name:"Rainbow Hair",icon:"🌈",cost:200,type:"hairCol",value:"linear",desc:"Special rainbow effect"},
  {id:"gold-crown",name:"Gold Crown",icon:"👑",cost:300,type:"acc",value:"crown",desc:"You are royalty!"},
  {id:"neon-shirt",name:"Neon Green Shirt",icon:"💚",cost:100,type:"shirt",value:"#39ff14",desc:"Glow in the dark!"},
  {id:"wizard-acc",name:"Party Hat",icon:"🎉",cost:150,type:"acc",value:"party-hat",desc:"Always festive!"},
  {id:"cool-shades",name:"Sunglasses",icon:"😎",cost:120,type:"acc",value:"sunglasses",desc:"Stay cool!"},
  {id:"pink-hair",name:"Bubblegum Hair",icon:"🩷",cost:180,type:"hairCol",value:"#ff69b4",desc:"Sweet & fun!"},
];

const QUIZ={
  Science:{icon:"🔬",color:"#06d6a0",questions:[
    {q:"Chemical symbol for water?",o:["H2O","CO2","O2","H2SO4"],a:0},
    {q:"Bones in adult human body?",o:["156","186","206","226"],a:2},
    {q:"The Red Planet?",o:["Venus","Mars","Jupiter","Saturn"],a:1},
    {q:"Gas plants use for photosynthesis?",o:["Oxygen","Nitrogen","Carbon Dioxide","Hydrogen"],a:2},
    {q:"Hardest natural substance?",o:["Gold","Iron","Diamond","Ruby"],a:2},
    {q:"Organ that pumps blood?",o:["Brain","Lung","Liver","Heart"],a:3},
    {q:"How many legs does a spider have?",o:["6","8","10","12"],a:1},
    {q:"Powerhouse of the cell?",o:["Nucleus","Ribosome","Mitochondria","Vacuole"],a:2},
    {q:"Speed of light approx?",o:["300 km/s","3,000 km/s","300,000 km/s","30,000 km/s"],a:2},
    {q:"What is H2O?",o:["Oxygen","Hydrogen","Water","Salt"],a:2},
    {q:"How many colors in a rainbow?",o:["5","6","7","8"],a:2},
    {q:"Which planet is largest?",o:["Saturn","Neptune","Jupiter","Uranus"],a:2},
    {q:"What do plants produce in photosynthesis?",o:["CO2","Oxygen","Nitrogen","Water"],a:1},
    {q:"Human body temperature (Celsius)?",o:["35°C","37°C","39°C","40°C"],a:1},
    {q:"Sound travels fastest through?",o:["Air","Water","Vacuum","Steel"],a:3},
  ]},
  Maths:{icon:"🔢",color:"#4361ee",questions:[
    {q:"What is 12 × 12?",o:["124","132","144","148"],a:2},
    {q:"What is √196?",o:["12","13","14","15"],a:2},
    {q:"25% of 200?",o:["25","40","50","75"],a:2},
    {q:"2 to the power of 10?",o:["512","1024","2048","256"],a:1},
    {q:"Angles in a triangle sum to?",o:["90°","120°","180°","360°"],a:2},
    {q:"What is 17 × 8?",o:["126","130","136","142"],a:2},
    {q:"What is 1000 ÷ 8?",o:["115","120","125","130"],a:2},
    {q:"Sides in a hexagon?",o:["5","6","7","8"],a:1},
    {q:"What is 15²?",o:["175","205","225","250"],a:2},
    {q:"What is 7! (7 factorial)?",o:["2040","5040","4050","3024"],a:1},
    {q:"Prime number between 10-15?",o:["11","12","14","15"],a:0},
    {q:"What is 3/4 as a percentage?",o:["65%","70%","75%","80%"],a:2},
    {q:"Area of circle with r=7? (π≈22/7)",o:["154","144","164","174"],a:0},
    {q:"What is 999 + 111?",o:["1000","1010","1100","1110"],a:3},
    {q:"What is 0.5 × 0.5?",o:["0.1","0.25","0.5","1.0"],a:1},
  ]},
  Geography:{icon:"🌍",color:"#fb8500",questions:[
    {q:"Capital of Australia?",o:["Sydney","Melbourne","Brisbane","Canberra"],a:3},
    {q:"Longest river in the world?",o:["Amazon","Mississippi","Nile","Yangtze"],a:2},
    {q:"Largest continent?",o:["Africa","North America","Asia","Europe"],a:2},
    {q:"Smallest country?",o:["Monaco","San Marino","Vatican City","Liechtenstein"],a:2},
    {q:"Largest ocean?",o:["Atlantic","Indian","Arctic","Pacific"],a:3},
    {q:"Capital of Japan?",o:["Osaka","Kyoto","Tokyo","Hiroshima"],a:2},
    {q:"Largest desert?",o:["Arabian","Gobi","Sahara","Antarctic"],a:3},
    {q:"How many continents?",o:["5","6","7","8"],a:2},
    {q:"Capital of Brazil?",o:["São Paulo","Rio de Janeiro","Brasília","Salvador"],a:2},
    {q:"Tallest mountain?",o:["K2","Kangchenjunga","Mount Everest","Lhotse"],a:2},
    {q:"Capital of India?",o:["Mumbai","Kolkata","New Delhi","Chennai"],a:2},
    {q:"Which country has most population?",o:["USA","China","India","Russia"],a:2},
    {q:"Amazon river is in?",o:["Africa","Asia","South America","Australia"],a:2},
    {q:"Capital of France?",o:["London","Berlin","Madrid","Paris"],a:3},
    {q:"Great Wall is in?",o:["Japan","Korea","China","Vietnam"],a:2},
  ]},
  History:{icon:"📜",color:"#ff6b6b",questions:[
    {q:"Who invented the telephone?",o:["Thomas Edison","Nikola Tesla","Alexander Graham Bell","Marconi"],a:2},
    {q:"Year WW2 ended?",o:["1943","1944","1945","1946"],a:2},
    {q:"First US President?",o:["Abraham Lincoln","John Adams","Thomas Jefferson","George Washington"],a:3},
    {q:"Who painted the Mona Lisa?",o:["Michelangelo","Raphael","Leonardo da Vinci","Donatello"],a:2},
    {q:"India's independence year?",o:["1945","1946","1947","1948"],a:2},
    {q:"Who discovered America in 1492?",o:["Vasco da Gama","Ferdinand Magellan","Christopher Columbus","John Cabot"],a:2},
    {q:"Who invented the light bulb?",o:["Nikola Tesla","Thomas Edison","Alexander Fleming","James Watt"],a:1},
    {q:"City of the Eiffel Tower?",o:["London","Berlin","Rome","Paris"],a:3},
    {q:"Who built the Pyramids?",o:["Romans","Greeks","Ancient Egyptians","Persians"],a:2},
    {q:"Who wrote Romeo and Juliet?",o:["Charles Dickens","Jane Austen","William Shakespeare","Mark Twain"],a:2},
    {q:"First man on the Moon?",o:["Buzz Aldrin","Neil Armstrong","Yuri Gagarin","John Glenn"],a:1},
    {q:"WW1 started in?",o:["1912","1914","1916","1918"],a:1},
    {q:"Who was Napoleon Bonaparte?",o:["British King","French Emperor","Spanish Admiral","Russian Tsar"],a:1},
    {q:"Mahatma Gandhi's birthday?",o:["Oct 2","Nov 14","Jan 26","Aug 15"],a:0},
    {q:"Which country gifted Statue of Liberty to USA?",o:["UK","Germany","France","Italy"],a:2},
  ]},
};

// ─── STATE ────────────────────────────────────────────────────────────────────
let CU=null, UD=null;
let rCfg=Object.assign({},DEF), eCfg=Object.assign({},DEF);
let isDark=true;
let qCat=null, qi=0, qSc=0, qCh=null, qStr=0, qQs=[], qMode='normal', timerInt=null, timerVal=10;
let chatInited=false, msgCount=0, curRoom=null, roomLsn=null;
let onInt=null;

// ─── AVATAR ───────────────────────────────────────────────────────────────────
function mkAv(cfg,sz){
  sz=sz||80;
  var c=cfg||DEF;
  var sk=c.skin||SKINS[0],hc=c.hairCol||HCS[0],hr=c.hair||'short',ex=c.expr||'happy',ac=c.acc||'none',sh=c.shirt||SHIRTS[0],gd=c.gender||'Boy';
  var h='';
  if(hr==='spiky')h='<rect x="26" y="20" width="68" height="20" rx="6" fill="'+hc+'"/><polygon points="30,22 35,8 40,22" fill="'+hc+'"/><polygon points="40,22 45,8 50,22" fill="'+hc+'"/><polygon points="50,22 55,8 60,22" fill="'+hc+'"/><polygon points="60,22 65,8 70,22" fill="'+hc+'"/><polygon points="70,22 75,8 80,22" fill="'+hc+'"/>';
  else if(hr==='messy')h='<ellipse cx="60" cy="28" rx="36" ry="16" fill="'+hc+'"/><ellipse cx="32" cy="36" rx="10" ry="8" fill="'+hc+'"/><ellipse cx="88" cy="36" rx="10" ry="8" fill="'+hc+'"/>';
  else if(hr==='short')h='<rect x="26" y="20" width="68" height="20" rx="10" fill="'+hc+'"/>';
  else if(hr==='curly')h='<ellipse cx="60" cy="26" rx="36" ry="14" fill="'+hc+'"/><circle cx="34" cy="34" r="9" fill="'+hc+'"/><circle cx="46" cy="34" r="9" fill="'+hc+'"/><circle cx="60" cy="34" r="9" fill="'+hc+'"/><circle cx="74" cy="34" r="9" fill="'+hc+'"/><circle cx="86" cy="34" r="9" fill="'+hc+'"/>';
  else if(hr==='mohawk')h='<rect x="26" y="26" width="14" height="14" rx="4" fill="'+hc+'"/><rect x="80" y="26" width="14" height="14" rx="4" fill="'+hc+'"/><rect x="50" y="4" width="20" height="36" rx="8" fill="'+hc+'"/>';
  else if(hr==='ponytail')h='<rect x="26" y="20" width="68" height="18" rx="9" fill="'+hc+'"/><ellipse cx="92" cy="40" rx="10" ry="22" fill="'+hc+'"/><circle cx="92" cy="24" r="6" fill="'+hc+'"/>';
  else if(hr==='pigtails')h='<rect x="26" y="20" width="68" height="18" rx="9" fill="'+hc+'"/><ellipse cx="20" cy="52" rx="10" ry="20" fill="'+hc+'"/><ellipse cx="100" cy="52" rx="10" ry="20" fill="'+hc+'"/>';
  else if(hr==='long')h='<rect x="26" y="20" width="68" height="18" rx="9" fill="'+hc+'"/><rect x="18" y="30" width="14" height="60" rx="7" fill="'+hc+'"/><rect x="88" y="30" width="14" height="60" rx="7" fill="'+hc+'"/>';
  else if(hr==='bun')h='<rect x="26" y="26" width="68" height="14" rx="7" fill="'+hc+'"/><circle cx="60" cy="16" r="14" fill="'+hc+'"/><circle cx="60" cy="16" r="8" fill="'+hc+'" opacity="0.6"/>';
  else if(hr==='curly-long')h='<ellipse cx="60" cy="26" rx="36" ry="14" fill="'+hc+'"/><ellipse cx="22" cy="60" rx="12" ry="30" fill="'+hc+'"/><ellipse cx="98" cy="60" rx="12" ry="30" fill="'+hc+'"/>';
  else if(hr==='bob')h='<rect x="26" y="20" width="68" height="18" rx="9" fill="'+hc+'"/><rect x="18" y="30" width="12" height="30" rx="6" fill="'+hc+'"/><rect x="90" y="30" width="12" height="30" rx="6" fill="'+hc+'"/>';
  var e='';
  if(ex==='happy')e='<circle cx="47" cy="57" r="7" fill="white"/><circle cx="73" cy="57" r="7" fill="white"/><circle cx="48" cy="58" r="4" fill="#222"/><circle cx="74" cy="58" r="4" fill="#222"/><path d="M50 74 Q60 82 70 74" stroke="#c0706b" stroke-width="2" fill="none" stroke-linecap="round"/>';
  else if(ex==='wink')e='<circle cx="47" cy="57" r="7" fill="white"/><circle cx="48" cy="58" r="4" fill="#222"/><path d="M67 54 Q73 62 79 54" stroke="#222" stroke-width="2.5" fill="none" stroke-linecap="round"/><path d="M50 74 Q60 82 70 74" stroke="#c0706b" stroke-width="2" fill="none" stroke-linecap="round"/>';
  else if(ex==='cool')e='<rect x="38" y="52" width="20" height="11" rx="5" fill="#1a1a2e"/><rect x="62" y="52" width="20" height="11" rx="5" fill="#1a1a2e"/><line x1="58" y1="57" x2="62" y2="57" stroke="#333" stroke-width="2"/><path d="M50 74 Q60 82 70 74" stroke="#c0706b" stroke-width="2" fill="none" stroke-linecap="round"/>';
  else if(ex==='silly')e='<circle cx="47" cy="57" r="7" fill="white"/><circle cx="73" cy="57" r="7" fill="white"/><circle cx="49" cy="55" r="4" fill="#222"/><circle cx="71" cy="59" r="4" fill="#222"/><ellipse cx="60" cy="76" rx="10" ry="7" fill="#E63946"/><ellipse cx="60" cy="79" rx="6" ry="4" fill="#ff9999"/>';
  else if(ex==='surprised')e='<circle cx="47" cy="57" r="8" fill="white"/><circle cx="73" cy="57" r="8" fill="white"/><circle cx="47" cy="57" r="5" fill="#222"/><circle cx="73" cy="57" r="5" fill="#222"/><ellipse cx="60" cy="76" rx="9" ry="8" fill="#222"/>';
  else if(ex==='smug')e='<circle cx="47" cy="57" r="7" fill="white"/><circle cx="73" cy="57" r="7" fill="white"/><circle cx="48" cy="58" r="4" fill="#222"/><circle cx="74" cy="58" r="4" fill="#222"/><path d="M52 74 Q63 78 70 72" stroke="#c0706b" stroke-width="2" fill="none" stroke-linecap="round"/>';
  var a='';
  if(ac==='party-hat')a='<polygon points="60,2 38,30 82,30" fill="#a855f7" opacity="0.9"/><rect x="38" y="28" width="44" height="6" rx="3" fill="#ffe66d"/><circle cx="42" cy="28" r="3" fill="#ff6b6b"/><circle cx="52" cy="30" r="3" fill="#4361ee"/><circle cx="62" cy="28" r="3" fill="#06d6a0"/>';
  else if(ac==='sunglasses')a='<rect x="36" y="50" width="24" height="14" rx="6" fill="#1a1a1a" opacity="0.9"/><rect x="60" y="50" width="24" height="14" rx="6" fill="#1a1a1a" opacity="0.9"/><rect x="34" y="55" width="4" height="3" rx="2" fill="#1a1a1a"/><rect x="82" y="55" width="4" height="3" rx="2" fill="#1a1a1a"/>';
  else if(ac==='crown')a='<polygon points="28,32 38,14 50,26 60,10 70,26 82,14 92,32" fill="#ffe66d"/><rect x="28" y="30" width="64" height="8" rx="2" fill="#ffe66d"/><circle cx="60" cy="16" r="5" fill="#ff6b6b"/><circle cx="38" cy="22" r="4" fill="#4361ee"/><circle cx="82" cy="22" r="4" fill="#06d6a0"/>';
  else if(ac==='cat-ears')a='<polygon points="26,32 20,8 42,26" fill="'+hc+'"/><polygon points="94,32 100,8 78,26" fill="'+hc+'"/><polygon points="28,30 22,12 40,26" fill="'+sk+'" opacity="0.5"/>';
  else if(ac==='headphones')a='<rect x="18" y="46" width="12" height="18" rx="6" fill="#333"/><rect x="90" y="46" width="12" height="18" rx="6" fill="#333"/><path d="M22 52 Q60 26 98 52" fill="none" stroke="#333" stroke-width="5"/>';
  var gx=gd==='Girl'?'<circle cx="20" cy="64" r="3" fill="#ffe66d"/><circle cx="100" cy="64" r="3" fill="#ffe66d"/><ellipse cx="38" cy="68" rx="8" ry="5" fill="#ffb3c1" opacity="0.45"/><ellipse cx="82" cy="68" rx="8" ry="5" fill="#ffb3c1" opacity="0.45"/>':'';
  return '<svg width="'+sz+'" height="'+sz+'" viewBox="0 0 120 120" xmlns="http://www.w3.org/2000/svg"><rect x="28" y="98" width="64" height="28" rx="14" fill="'+sh+'"/><rect x="50" y="88" width="20" height="16" rx="6" fill="'+sk+'"/><ellipse cx="60" cy="62" rx="34" ry="34" fill="'+sk+'"/>'+h+'<ellipse cx="26" cy="62" rx="6" ry="8" fill="'+sk+'"/><ellipse cx="94" cy="62" rx="6" ry="8" fill="'+sk+'"/>'+gx+e+'<ellipse cx="60" cy="70" rx="4" ry="3" fill="'+sk+'" style="filter:brightness(0.85)"/>'+a+'</svg>';
}

// ─── THEME ────────────────────────────────────────────────────────────────────
function toggleTheme(){isDark=!isDark;document.body.style.background=isDark?'#0d0d1a':'#f0f4ff';document.body.style.color=isDark?'#f0f0f0':'#1a1a35';}

// ─── PAGE ─────────────────────────────────────────────────────────────────────
function showPage(id){document.querySelectorAll('.page').forEach(function(p){p.classList.remove('active');});document.getElementById(id).classList.add('active');}

// ─── AUTH ─────────────────────────────────────────────────────────────────────
function sE(id,msg){var e=document.getElementById(id);e.style.display='block';e.textContent=msg;}
function hE(id){document.getElementById(id).style.display='none';}
function eh(s){return String(s).replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;');}

async function doLogin(){
  var u=document.getElementById('l-user').value.trim().toLowerCase();
  var p=document.getElementById('l-pass').value;
  if(!u||!p){sE('l-err','Fill in username and password!');return;}
  hE('l-err');
  try{
    var snap=await db.ref('usernames/'+u).once('value');
    if(!snap.exists()){sE('l-err','Account not found — register first!');return;}
    await auth.signInWithEmailAndPassword(snap.val(),p);
  }catch(e){sE('l-err',e.code==='auth/wrong-password'?'Wrong password! 🔐':'Error: '+e.message);}
}

async function doRegister(){
  var name=document.getElementById('r-name').value.trim();
  var u=document.getElementById('r-user').value.trim().toLowerCase();
  var p=document.getElementById('r-pass').value;
  var p2=document.getElementById('r-pass2').value;
  if(!name||!u||!p){sE('r-err','Fill in all fields!');return;}
  if(p!==p2){sE('r-err',"Passwords don't match!");return;}
  if(p.length<4){sE('r-err','Password needs 4+ chars!');return;}
  if(u.length<3){sE('r-err','Username needs 3+ chars!');return;}
  hE('r-err');
  try{
    var ex=await db.ref('usernames/'+u).once('value');
    if(ex.exists()){sE('r-err','Username taken! Try another 😅');return;}
    var email=u+'@zapzone.app';
    var cr=await auth.createUserWithEmailAndPassword(email,p);
    var uid=cr.user.uid;
    var cfg=Object.assign({},rCfg,{name:name});
    var data={name:name,username:u,avatar:cfg,coins:100,xp:0,scores:{},badges:{firstLogin:true},msgCount:0,shopOwned:{}};
    await db.ref('users/'+uid).set(data);
    await db.ref('usernames/'+u).set(email);
    await db.ref('messages').push({uid:uid,name:name,avatar:cfg,text:'🌟 '+name+' just joined ZapZone! Say hi! 👋',ts:Date.now(),system:true});
    showBadge('firstLogin');
  }catch(e){sE('r-err','Error: '+e.message);}
}

function doLogout(){
  if(roomLsn){db.ref('rooms/'+curRoom+'/messages').off();roomLsn=null;}
  auth.signOut();
  chatInited=false;msgCount=0;curRoom=null;
  if(onInt)clearInterval(onInt);
}

auth.onAuthStateChanged(async function(user){
  if(user){
    CU=user;
    var snap=await db.ref('users/'+user.uid).once('value');
    UD=snap.val()||{};UD.uid=user.uid;
    enterApp();
  }else{CU=null;UD=null;showPage('login');}
});

// ─── APP INIT ─────────────────────────────────────────────────────────────────
function enterApp(){
  showPage('app');sw('chat');
  updHdrAv();initChat();startOnline();buildCats();updProf();buildBadges();buildShop();loadAnn();loadMiniLb();checkDaily();
  updVIPUI();updAdUI();
}

function updHdrAv(){if(!UD)return;document.getElementById('hdr-av').innerHTML=mkAv(UD.avatar||DEF,38);}

// ─── CHAT ─────────────────────────────────────────────────────────────────────
function initChat(){
  if(chatInited)return;chatInited=true;
  var el=document.getElementById('ch-msgs');var first=true;
  db.ref('messages').limitToLast(60).on('child_added',function(snap){
    var m=snap.val();if(!m)return;
    if(first){el.innerHTML='';first=false;}
    renderMsg(m,snap.key,el);
    el.scrollTop=el.scrollHeight;
    msgCount++;
    if(msgCount>=20&&UD&&!(UD.badges&&UD.badges.chatKing)){awardBadge('chatKing');}
  });
}

function renderMsg(m,key,container){
  if(!m)return;
  var isMe=CU&&m.uid===CU.uid;
  if(m.system){var d=document.createElement('div');d.style.cssText='text-align:center;color:#7070a0;font-size:12px;padding:4px 0';d.textContent=m.text;container.appendChild(d);return;}
  var row=document.createElement('div');row.className='msg-row'+(isMe?' me':'');
  var av=mkAv(m.avatar||DEF,34);
  var time=new Date(m.ts).toLocaleTimeString([],{hour:'2-digit',minute:'2-digit'});
  var rxnHtml='<div class="msg-reactions" id="rxn-'+key+'"><button class="add-rxn" onclick="toggleRxnPicker(\''+key+'\')">+😊</button></div><div class="rxn-picker" id="rp-'+key+'"><button class="rxn-pick-btn" onclick="addRxn(\''+key+'\',\'👍\')">👍</button><button class="rxn-pick-btn" onclick="addRxn(\''+key+'\',\'❤️\')">❤️</button><button class="rxn-pick-btn" onclick="addRxn(\''+key+'\',\'😂\')">😂</button><button class="rxn-pick-btn" onclick="addRxn(\''+key+'\',\'🔥\')">🔥</button><button class="rxn-pick-btn" onclick="addRxn(\''+key+'\',\'⚡\')">⚡</button></div>';
  if(isMe){row.innerHTML='<div class="msg-body" style="max-width:72%"><div class="msg-bbl">'+eh(m.text)+'</div>'+rxnHtml+'<div style="font-size:10px;color:#7070a0;margin-top:2px;text-align:right">'+time+'</div></div><div>'+av+'</div>';}
  else{row.innerHTML='<div>'+av+'</div><div class="msg-body" style="max-width:72%"><div style="font-size:11px;color:#7070a0;margin-bottom:2px;margin-left:2px">'+eh(m.name||'')+'</div><div class="msg-bbl">'+eh(m.text)+'</div>'+rxnHtml+'<div style="font-size:10px;color:#7070a0;margin-top:2px;margin-left:2px">'+time+'</div></div>';}
  container.appendChild(row);
  // Listen for reactions
  db.ref('messages/'+key+'/reactions').on('value',function(rsnap){updRxnDisplay(key,rsnap.val());});
}

function toggleRxnPicker(key){var rp=document.getElementById('rp-'+key);if(rp)rp.classList.toggle('open');}

async function addRxn(key,emoji){
  if(!CU)return;
  await db.ref('messages/'+key+'/reactions/'+emoji+'/'+CU.uid).transaction(function(v){return v?null:true;});
  var rp=document.getElementById('rp-'+key);if(rp)rp.classList.remove('open');
}

function updRxnDisplay(key,rxns){
  var el=document.getElementById('rxn-'+key);if(!el)return;
  var html='';
  if(rxns){
    Object.keys(rxns).forEach(function(emoji){
      var users=rxns[emoji];var cnt=Object.keys(users).length;var mine=CU&&users[CU.uid];
      if(cnt>0)html+='<button class="rxn-btn'+(mine?' active':'')+'" onclick="addRxn(\''+key+'\',\''+emoji+'\')">'+emoji+' '+cnt+'</button>';
    });
  }
  html+='<button class="add-rxn" onclick="toggleRxnPicker(\''+key+'\')">+😊</button>';
  el.innerHTML=html;
}

async function sendMsg(){
  var inp=document.getElementById('ch-inp');var t=inp.value.trim();
  if(!t||!CU||!UD)return;inp.value='';
  await db.ref('messages').push({uid:CU.uid,name:UD.name||'Player',avatar:UD.avatar||DEF,text:t,ts:Date.now()});
}
function addE(e){var i=document.getElementById('ch-inp');i.value+=e;i.focus();}

// ─── ONLINE ───────────────────────────────────────────────────────────────────
function startOnline(){
  if(!CU)return;
  function hb(){db.ref('online/'+CU.uid).set({ts:Date.now(),name:UD&&UD.name||'Player'});}
  hb();onInt=setInterval(hb,30000);
  db.ref('online').on('value',function(snap){
    var now=Date.now(),cnt=0;
    snap.forEach(function(c){var d=c.val();if(d&&now-d.ts<90000)cnt++;});
    var el=document.getElementById('online-c');if(el)el.textContent='● '+cnt+' online';
  });
}

// ─── TABS ─────────────────────────────────────────────────────────────────────
function sw(name){
  var tabs=['chat','quiz','rooms','roomchat','shop','me'];
  tabs.forEach(function(t){var el=document.getElementById('t-'+t);if(el)el.style.display='none';});
  var navs=['chat','quiz','rooms','shop','me'];
  navs.forEach(function(n){var el=document.getElementById('n-'+n);if(el)el.classList.remove('on');});
  var el=document.getElementById('t-'+name);
  if(el)el.style.display=name==='chat'||name==='roomchat'?'flex':'block';
  var nb=document.getElementById('n-'+name);if(nb)nb.classList.add('on');
  if(name==='chat'){var m=document.getElementById('ch-msgs');if(m)setTimeout(function(){m.scrollTop=m.scrollHeight;},100);}
  if(name==='me'){updProf();buildBadges();}
  if(name==='shop'){updShopCoins();}
  if(name==='quiz'){updQCoins();}
  if(name==='rooms'){loadMyRooms();}
}

// ─── QUIZ ─────────────────────────────────────────────────────────────────────
function setMode(m){
  qMode=m;
  document.getElementById('mode-normal').classList.toggle('sel',m==='normal');
  document.getElementById('mode-timer').classList.toggle('sel',m==='timer');
}

function buildCats(){
  var g=document.getElementById('cat-grid');if(!g)return;g.innerHTML='';
  Object.keys(QUIZ).forEach(function(cat){
    var info=QUIZ[cat];var best=UD&&UD.scores&&UD.scores[cat]?UD.scores[cat]:0;
    var d=document.createElement('button');d.className='cat-card';
    d.innerHTML='<div style="font-size:32px;margin-bottom:6px">'+info.icon+'</div><div style="font-weight:800;font-size:15px;color:#f0f0f0">'+cat+'</div><div style="color:#7070a0;font-size:11px;margin-top:2px">15 questions</div>'+(best>0?'<div style="color:'+info.color+';font-size:11px;font-weight:700;margin-top:3px">Best: '+best+'/10 ⭐</div>':'');
    d.onclick=function(){startQuiz(cat);};
    g.appendChild(d);
  });
  updQCoins();
}

function updQCoins(){
  var c=UD?UD.coins||0:0;
  var el=document.getElementById('qz-coins');if(el)el.textContent='🪙 '+c;
  var el2=document.getElementById('shop-coins');if(el2)el2.textContent='🪙 '+c;
}

function startQuiz(cat){
  qCat=cat;qi=0;qSc=0;qCh=null;qStr=0;
  qQs=QUIZ[cat].questions.slice().sort(function(){return Math.random()-0.5;}).slice(0,10);
  document.getElementById('qz-cats').style.display='none';
  document.getElementById('qz-done').style.display='none';
  document.getElementById('qz-game').style.display='block';
  var info=QUIZ[cat];
  document.getElementById('q-cat-lbl').textContent=info.icon+' '+cat;
  document.getElementById('q-cat-lbl').style.color=info.color;
  document.getElementById('q-card').style.borderColor=info.color;
  document.getElementById('q-pf').style.background=info.color;
  document.getElementById('q-streak').style.display='none';
  renderQ();
}

function renderQ(){
  var q=qQs[qi];
  document.getElementById('q-pf').style.width=(qi/qQs.length*100)+'%';
  document.getElementById('q-cnt').textContent=(qi+1)+'/'+qQs.length;
  document.getElementById('q-txt').textContent=q.q;
  var opts=document.getElementById('q-opts');opts.innerHTML='';
  q.o.forEach(function(opt,i){
    var b=document.createElement('button');b.className='q-opt';
    b.innerHTML='<span style="color:#7070a0;margin-right:6px;font-weight:800">'+['A','B','C','D'][i]+'.</span>'+eh(opt);
    b.onclick=function(){ansQ(i);};opts.appendChild(b);
  });
  qCh=null;
  // Timer mode
  if(qMode==='timer'){
    timerVal=10;
    var tr=document.getElementById('q-timer');tr.style.display='flex';tr.textContent=timerVal;tr.className='timer-ring';
    if(timerInt)clearInterval(timerInt);
    timerInt=setInterval(function(){
      timerVal--;
      var tr2=document.getElementById('q-timer');if(tr2){tr2.textContent=timerVal;if(timerVal<=3)tr2.className='timer-ring warn';}
      if(timerVal<=0){clearInterval(timerInt);if(qCh===null)ansQ(-1);}
    },1000);
  } else {
    document.getElementById('q-timer').style.display='none';
    if(timerInt)clearInterval(timerInt);
  }
}

async function ansQ(idx){
  if(qCh!==null)return;qCh=idx;
  if(timerInt)clearInterval(timerInt);
  var q=qQs[qi];
  var opts=document.getElementById('q-opts').children;
  if(opts[q.a])opts[q.a].classList.add('correct');
  if(idx>=0&&idx!==q.a&&opts[idx])opts[idx].classList.add('wrong');
  for(var i=0;i<opts.length;i++)opts[i].onclick=null;
  if(idx===q.a){
    var bonus=qStr>=2?2:1;qSc++;qStr++;
    var addC=15*bonus,addX=20;
    if(UD){UD.coins=(UD.coins||0)+addC;UD.xp=(UD.xp||0)+addX;}
    await db.ref('users/'+CU.uid+'/coins').set(UD.coins);
    await db.ref('users/'+CU.uid+'/xp').set(UD.xp);
    updQCoins();
    if(qStr>=5&&!(UD.badges&&UD.badges.streakHero))awardBadge('streakHero');
    if(qMode==='timer'&&!(UD.badges&&UD.badges.speedster))awardBadge('speedster');
    var ss=document.getElementById('q-streak');ss.style.display='block';ss.textContent='🔥x'+qStr;
  } else {qStr=0;document.getElementById('q-streak').style.display='none';}
  setTimeout(function(){if(qi+1>=qQs.length)showDone();else{qi++;renderQ();}},900);
}

async function showDone(){
  document.getElementById('qz-game').style.display='none';
  document.getElementById('qz-done').style.display='block';
  var icons=['😅','😅','😅','😊','😊','🌟','🌟','🌟','🏆','🏆','🏆'];
  document.getElementById('done-icon').textContent=icons[qSc]||'🏆';
  var titles={0:'Keep Zapping!',1:'Keep Zapping!',2:'Keep Zapping!',3:'Good Try!',4:'Good Try!',5:'Well Played!',6:'Well Played!',7:'Well Played!',8:'You Dominated!',9:'Almost Perfect!',10:'PERFECT! 🎉'};
  document.getElementById('done-title').textContent=titles[qSc]||'Done!';
  document.getElementById('done-sub').textContent=qSc+'/'+qQs.length+' correct • '+QUIZ[qCat].icon+' '+qCat;
  document.getElementById('done-av').innerHTML=mkAv(UD&&UD.avatar||DEF,80);
  document.getElementById('done-reward').textContent='+'+qSc*15+' coins • +'+qSc*20+' XP saved!';
  var prev=UD&&UD.scores&&UD.scores[qCat]?UD.scores[qCat]:0;
  if(qSc>prev){
    if(!UD.scores)UD.scores={};UD.scores[qCat]=qSc;
    await db.ref('users/'+CU.uid+'/scores/'+qCat).set(qSc);
    var total=Object.values(UD.scores).reduce(function(a,b){return a+b;},0);
    await db.ref('leaderboard/'+CU.uid).set({name:UD.name||'Player',username:UD.username||'',avatar:UD.avatar||DEF,scores:UD.scores,total:total});
  }
  // Quiz master badge
  var cats=Object.keys(QUIZ);var allDone=cats.every(function(c){return UD.scores&&UD.scores[c];});
  if(allDone&&!(UD.badges&&UD.badges.quizMaster))awardBadge('quizMaster');
  // Coin badge
  if((UD.coins||0)>=500&&!(UD.badges&&UD.badges.richKid))awardBadge('richKid');
  updProf();buildCats();loadMiniLb();
}

function playAgain(){startQuiz(qCat);}
function backCats(){
  document.getElementById('qz-game').style.display='none';
  document.getElementById('qz-done').style.display='none';
  document.getElementById('qz-cats').style.display='block';
  if(timerInt)clearInterval(timerInt);qCat=null;
}

// ─── DAILY CHALLENGE ─────────────────────────────────────────────────────────
function checkDaily(){
  var today=new Date().toDateString();
  var done=UD&&UD.lastDaily===today;
  var btn=document.getElementById('daily-btn');
  if(done){btn.textContent='✅ Done!';btn.disabled=true;btn.style.opacity='0.5';}
  else{btn.textContent='Play!';btn.disabled=false;btn.style.opacity='1';}
}

async function startDaily(){
  var today=new Date().toDateString();
  if(UD&&UD.lastDaily===today){alert('Already done today! Come back tomorrow! 🌟');return;}
  // Pick random category based on day
  var cats=Object.keys(QUIZ);var idx=new Date().getDate()%cats.length;
  var cat=cats[idx];
  qCat=cat;qi=0;qSc=0;qCh=null;qStr=0;
  qQs=QUIZ[cat].questions.slice(0,8);// Fixed daily questions
  sw('quiz');
  document.getElementById('qz-cats').style.display='none';
  document.getElementById('qz-done').style.display='none';
  document.getElementById('qz-game').style.display='block';
  var info=QUIZ[cat];
  document.getElementById('q-cat-lbl').textContent='🌟 Daily: '+info.icon+' '+cat;
  document.getElementById('q-cat-lbl').style.color='#ffe66d';
  document.getElementById('q-card').style.borderColor='#ffe66d';
  document.getElementById('q-pf').style.background='#ffe66d';
  renderQ();
  // Override showDone for daily bonus
  var origShowDone=showDone;
  window._dailyMode=true;
  // Mark done and give bonus
  if(UD){UD.lastDaily=today;await db.ref('users/'+CU.uid+'/lastDaily').set(today);}
  if(!(UD.badges&&UD.badges.dailyHero))awardBadge('dailyHero');
  // Give 100 bonus coins
  UD.coins=(UD.coins||0)+100;
  await db.ref('users/'+CU.uid+'/coins').set(UD.coins);
  updQCoins();checkDaily();
}

// ─── PRIVATE ROOMS ────────────────────────────────────────────────────────────
function genCode(){return Math.random().toString(36).substr(2,6).toUpperCase();}

async function createRoom(){
  var name=document.getElementById('room-name').value.trim();
  if(!name||!CU)return;
  var code=genCode();
  await db.ref('rooms/'+code).set({name:name,code:code,createdBy:CU.uid,createdByName:UD&&UD.name||'Player',ts:Date.now(),members:{}});
  await db.ref('rooms/'+code+'/members/'+CU.uid).set(UD&&UD.name||'Player');
  if(UD&&!(UD.badges&&UD.badges.socialite))awardBadge('socialite');
  document.getElementById('room-name').value='';
  alert('Room created! Code: '+code+'\n\nShare this code with friends!');
  loadMyRooms();openRoom(code,name);
}

async function joinRoom(){
  var code=document.getElementById('join-code').value.trim().toUpperCase();
  if(!code||code.length!==6){alert('Enter a valid 6-digit room code!');return;}
  var snap=await db.ref('rooms/'+code).once('value');
  if(!snap.exists()){alert('Room not found! Check the code.');return;}
  await db.ref('rooms/'+code+'/members/'+CU.uid).set(UD&&UD.name||'Player');
  if(UD&&!(UD.badges&&UD.badges.socialite))awardBadge('socialite');
  document.getElementById('join-code').value='';
  var room=snap.val();
  openRoom(code,room.name);
}

async function loadMyRooms(){
  var el=document.getElementById('my-rooms');if(!el)return;
  el.innerHTML='<div style="color:#7070a0;font-size:13px">Loading...</div>';
  var snap=await db.ref('rooms').orderByChild('createdBy').equalTo(CU&&CU.uid).once('value');
  var rooms=[];snap.forEach(function(c){rooms.push(Object.assign({code:c.key},c.val()));});
  // Also get rooms we're member of
  if(rooms.length===0){el.innerHTML='<div style="color:#7070a0;font-size:13px">No rooms yet!</div>';return;}
  el.innerHTML='';
  rooms.forEach(function(r){
    var div=document.createElement('div');div.className='room-item';
    div.innerHTML='<div style="font-size:28px">🏠</div><div style="flex:1"><div style="font-weight:800;font-size:15px">'+eh(r.name)+'</div><div style="color:#7070a0;font-size:12px">Code: <span style="color:#ffe66d;font-weight:700;letter-spacing:2px">'+r.code+'</span></div></div><button style="background:#a855f7;border:none;border-radius:10px;padding:6px 12px;color:#fff;font-size:12px;cursor:pointer" onclick="openRoom(\''+r.code+'\',\''+eh(r.name)+'\')">Open</button>';
    el.appendChild(div);
  });
}

function openRoom(code,name){
  curRoom=code;
  document.getElementById('rc-name').textContent=name;
  document.getElementById('rc-code').textContent='Code: '+code;
  var el=document.getElementById('rc-msgs');el.innerHTML='';
  sw('roomchat');
  if(roomLsn){db.ref('rooms/'+curRoom+'/messages').off();}
  var first=true;
  roomLsn=db.ref('rooms/'+code+'/messages').limitToLast(50).on('child_added',function(snap){
    var m=snap.val();if(!m)return;
    if(first){el.innerHTML='';first=false;}
    var isMe=CU&&m.uid===CU.uid;
    if(m.system){var d=document.createElement('div');d.style.cssText='text-align:center;color:#7070a0;font-size:12px;padding:4px 0';d.textContent=m.text;el.appendChild(d);}
    else{
      var row=document.createElement('div');row.className='msg-row'+(isMe?' me':'');
      var time=new Date(m.ts).toLocaleTimeString([],{hour:'2-digit',minute:'2-digit'});
      if(isMe)row.innerHTML='<div style="max-width:72%"><div class="msg-bbl">'+eh(m.text)+'</div><div style="font-size:10px;color:#7070a0;margin-top:2px;text-align:right">'+time+'</div></div><div>'+mkAv(m.avatar||DEF,34)+'</div>';
      else row.innerHTML='<div>'+mkAv(m.avatar||DEF,34)+'</div><div style="max-width:72%"><div style="font-size:11px;color:#7070a0;margin-bottom:2px;margin-left:2px">'+eh(m.name||'')+'</div><div class="msg-bbl">'+eh(m.text)+'</div><div style="font-size:10px;color:#7070a0;margin-top:2px;margin-left:2px">'+time+'</div></div>';
      el.appendChild(row);
    }
    el.scrollTop=el.scrollHeight;
  });
  // Member count
  db.ref('rooms/'+code+'/members').on('value',function(snap){
    var cnt=snap.numChildren();
    document.getElementById('rc-members').textContent='👥 '+cnt+' members';
  });
}

async function sendRoomMsg(){
  var inp=document.getElementById('rc-inp');var t=inp.value.trim();
  if(!t||!CU||!curRoom)return;inp.value='';
  await db.ref('rooms/'+curRoom+'/messages').push({uid:CU.uid,name:UD&&UD.name||'Player',avatar:UD&&UD.avatar||DEF,text:t,ts:Date.now()});
}

function leaveRoomChat(){
  if(roomLsn){db.ref('rooms/'+curRoom+'/messages').off();roomLsn=null;}
  curRoom=null;sw('rooms');
}

// ─── SHOP ─────────────────────────────────────────────────────────────────────
function buildShop(){
  var g=document.getElementById('shop-grid');if(!g)return;g.innerHTML='';
  SHOP_ITEMS.forEach(function(item){
    var owned=UD&&UD.shopOwned&&UD.shopOwned[item.id];
    var d=document.createElement('div');d.className='shop-item'+(owned?' owned':'');
    d.innerHTML='<div style="font-size:32px;margin-bottom:6px">'+item.icon+'</div><div style="font-weight:800;font-size:13px;margin-bottom:2px">'+item.name+'</div><div style="color:#7070a0;font-size:11px;margin-bottom:8px">'+item.desc+'</div>'+(owned?'<div style="color:#06d6a0;font-weight:700;font-size:12px">✅ Owned</div>':'<button style="background:linear-gradient(135deg,#a855f7,#4361ee);border:none;border-radius:10px;padding:6px 12px;color:#fff;font-size:12px;cursor:pointer;font-family:inherit;width:100%" onclick="buyItem(\''+item.id+'\')">'+item.cost+' 🪙</button>');
    g.appendChild(d);
  });
  updShopCoins();
}

async function buyItem(itemId){
  var item=SHOP_ITEMS.find(function(i){return i.id===itemId;});
  if(!item||!CU||!UD)return;
  if(UD.shopOwned&&UD.shopOwned[itemId]){alert('Already owned!');return;}
  if((UD.coins||0)<item.cost){alert('Not enough coins! Need '+item.cost+' 🪙');return;}
  UD.coins=(UD.coins||0)-item.cost;
  if(!UD.shopOwned)UD.shopOwned={};UD.shopOwned[itemId]=true;
  await db.ref('users/'+CU.uid+'/coins').set(UD.coins);
  await db.ref('users/'+CU.uid+'/shopOwned/'+itemId).set(true);
  // Apply item to avatar
  if(!UD.avatar)UD.avatar=Object.assign({},DEF);
  if(item.type==='acc')UD.avatar.acc=item.value;
  else if(item.type==='hairCol')UD.avatar.hairCol=item.value;
  else if(item.type==='shirt')UD.avatar.shirt=item.value;
  await db.ref('users/'+CU.uid+'/avatar').set(UD.avatar);
  if(!(UD.badges&&UD.badges.shopper))awardBadge('shopper');
  alert('🎉 Purchased '+item.name+'! Applied to your avatar!');
  buildShop();updShopCoins();updHdrAv();updProf();
}

function updShopCoins(){
  var c=UD?UD.coins||0:0;
  var el=document.getElementById('shop-coins');if(el)el.textContent='🪙 '+c;
}

// ─── SPIN TO WIN — see monetization section below ─────────────────────────────

// ─── BADGES ───────────────────────────────────────────────────────────────────
function buildBadges(){
  var g=document.getElementById('badge-grid');if(!g)return;g.innerHTML='';
  BADGES.forEach(function(b){
    var earned=UD&&UD.badges&&UD.badges[b.id];
    var d=document.createElement('div');d.className='badge-item'+(earned?' earned':'');
    d.innerHTML='<div class="badge-icon" style="opacity:'+(earned?'1':'0.3')+'">'+b.icon+'</div><div class="badge-name">'+b.name+'</div>';
    d.title=b.desc;g.appendChild(d);
  });
}

async function awardBadge(id){
  var badge=BADGES.find(function(b){return b.id===id;});if(!badge||!CU)return;
  if(!UD.badges)UD.badges={};UD.badges[id]=true;
  await db.ref('users/'+CU.uid+'/badges/'+id).set(true);
  showBadge(id);buildBadges();
}

function showBadge(id){
  var badge=BADGES.find(function(b){return b.id===id;});if(!badge)return;
  document.getElementById('bm-icon').textContent=badge.icon;
  document.getElementById('bm-title').textContent='New Badge: '+badge.name;
  document.getElementById('bm-desc').textContent=badge.desc;
  document.getElementById('badge-modal').classList.add('open');
}

// ─── PROFILE ─────────────────────────────────────────────────────────────────
function updProf(){
  if(!UD)return;
  var xp=UD.xp||0,lv=Math.floor(xp/150)+1,bar=(xp%150)/150*100;
  document.getElementById('prof-av').innerHTML=mkAv(UD.avatar||DEF,110);
  document.getElementById('prof-name').textContent=UD.name||'Player';
  document.getElementById('prof-user').textContent='@'+(UD.username||'')+' • Level '+lv;
  document.getElementById('xp-bar').style.width=bar+'%';
  document.getElementById('xp-lbl').textContent=(xp%150)+'/150 XP to next level';
  document.getElementById('s-coins').textContent=UD.coins||0;
  document.getElementById('s-xp').textContent=xp;
  document.getElementById('s-lv').textContent=lv;
  var rl=document.getElementById('rec-list');if(rl){rl.innerHTML='';
    Object.keys(QUIZ).forEach(function(cat){
      var sc=UD.scores&&UD.scores[cat]?UD.scores[cat]:0;var info=QUIZ[cat];
      var row=document.createElement('div');row.style.cssText='display:flex;align-items:center;gap:10px;margin-bottom:8px';
      row.innerHTML='<span style="font-size:18px">'+info.icon+'</span><div style="flex:1"><div style="display:flex;justify-content:space-between;margin-bottom:2px"><span style="font-size:13px;font-weight:600">'+cat+'</span><span style="font-size:13px;font-weight:700;color:'+info.color+'">'+sc+'/10</span></div><div style="background:#0a0a18;border-radius:4px;height:5px;overflow:hidden"><div style="width:'+(sc/10*100)+'%;height:100%;background:'+info.color+';border-radius:4px"></div></div></div>';
      rl.appendChild(row);
    });
  }
}

// ─── AVATAR EDITOR ────────────────────────────────────────────────────────────
function showAvEd(){
  eCfg=Object.assign({},UD&&UD.avatar||DEF);
  document.getElementById('prof-view').style.display='none';
  document.getElementById('av-ed').style.display='block';
  initEdPickers();
}
function hideAvEd(){document.getElementById('av-ed').style.display='none';document.getElementById('prof-view').style.display='block';}

function initEdPickers(){
  function mkSw(cid,arr,key,isCol){
    var el=document.getElementById(cid);if(!el)return;el.innerHTML='';
    arr.forEach(function(v){
      var b=document.createElement('button');
      if(isCol){b.className='sw-btn'+(eCfg[key]===v?' sel':'');b.innerHTML='<div class="sw-dot" style="background:'+v+'"></div>';}
      else{b.className='txt-opt'+(eCfg[key]===v?' sel':'');b.textContent=v;}
      b.onclick=function(){eCfg[key]=v;updEdAv();el.querySelectorAll(isCol?'.sw-btn':'.txt-opt').forEach(function(x){x.classList.remove('sel');});b.classList.add('sel');};
      el.appendChild(b);
    });
  }
  mkSw('e-skin',SKINS,'skin',true);mkSw('e-hc',HCS,'hairCol',true);mkSw('e-sh',SHIRTS,'shirt',true);
  mkSw('e-hair',eCfg.gender==='Boy'?BH:GH,'hair',false);
  mkSw('e-expr',EXPRS,'expr',false);mkSw('e-acc',ACCS,'acc',false);
  document.getElementById('e-boy').classList.toggle('sel',eCfg.gender==='Boy');
  document.getElementById('e-girl').classList.toggle('sel',eCfg.gender==='Girl');
  updEdAv();
}
function setEG(g){eCfg.gender=g;eCfg.hair=g==='Boy'?'short':'ponytail';initEdPickers();}
function updEdAv(){document.getElementById('ed-av').innerHTML=mkAv(eCfg,100);}
async function saveAv(){
  if(!CU)return;UD.avatar=Object.assign({},eCfg);
  await db.ref('users/'+CU.uid+'/avatar').set(UD.avatar);
  updProf();updHdrAv();hideAvEd();
}

// ─── REG PICKERS ──────────────────────────────────────────────────────────────
function initRegPickers(){
  function mkSw(cid,arr,key,isCol){
    var el=document.getElementById(cid);if(!el)return;el.innerHTML='';
    arr.forEach(function(v,i){
      var b=document.createElement('button');
      if(isCol){b.className='sw-btn'+(i===0?' sel':'');b.innerHTML='<div class="sw-dot" style="background:'+v+'"></div>';}
      else{b.className='txt-opt'+(i===0?' sel':'');b.textContent=v;}
      b.onclick=function(){rCfg[key]=v;updRegAv();el.querySelectorAll(isCol?'.sw-btn':'.txt-opt').forEach(function(x){x.classList.remove('sel');});b.classList.add('sel');};
      el.appendChild(b);
    });
  }
  mkSw('r-skin',SKINS,'skin',true);mkSw('r-expr',EXPRS,'expr',false);mkSw('r-acc',ACCS,'acc',false);
  updRegAv();
}
function setRG(g){rCfg.gender=g;rCfg.hair=g==='Boy'?'short':'ponytail';document.getElementById('g-boy').classList.toggle('sel',g==='Boy');document.getElementById('g-girl').classList.toggle('sel',g==='Girl');updRegAv();}
function updRegAv(){var n=document.getElementById('r-name').value.trim()||'You';rCfg.name=n;document.getElementById('reg-av').innerHTML=mkAv(rCfg,80);document.getElementById('reg-av-name').textContent=n;}

// ─── LEADERBOARD (MINI) ───────────────────────────────────────────────────────
async function loadMiniLb(){
  var el=document.getElementById('mini-lb');if(!el)return;
  el.innerHTML='<div style="color:#7070a0;font-size:12px">Loading...</div>';
  try{
    var snap=await db.ref('leaderboard').orderByChild('total').limitToLast(5).once('value');
    var entries=[];snap.forEach(function(c){entries.push(Object.assign({uid:c.key},c.val()));});
    entries.sort(function(a,b){return(b.total||0)-(a.total||0);});
    if(!entries.length){el.innerHTML='<div style="color:#7070a0;font-size:12px">No scores yet — play quiz first!</div>';return;}
    el.innerHTML='';
    entries.forEach(function(e,i){
      var med=['🥇','🥈','🥉','4️⃣','5️⃣'][i]||'';var isMe=CU&&e.uid===CU.uid;
      var row=document.createElement('div');row.className='lb-row'+(isMe?' me':'');
      row.innerHTML='<div style="font-size:18px;min-width:26px">'+med+'</div><div>'+mkAv(e.avatar||DEF,36)+'</div><div style="flex:1"><div style="font-weight:800;font-size:13px">'+eh(e.name||'')+'</div><div style="color:#7070a0;font-size:11px">@'+eh(e.username||'')+'</div></div><div style="text-align:right"><div style="font-weight:900;color:#ffe66d;font-size:18px">'+(e.total||0)+'</div><div style="color:#7070a0;font-size:10px">pts</div></div>';
      el.appendChild(row);
    });
  }catch(err){el.innerHTML='<div style="color:#7070a0;font-size:12px">Could not load.</div>';}
}

// ─── ANNOUNCEMENTS ────────────────────────────────────────────────────────────
function loadAnn(){
  db.ref('announcement').on('value',function(snap){
    var d=snap.val();var b=document.getElementById('ann-banner');
    if(d&&d.text&&d.active){b.style.display='block';document.getElementById('ann-text').textContent=d.text;}
    else{b.style.display='none';}
  });
}

// ─── MONETIZATION ────────────────────────────────────────────────────────────

// !! RAZORPAY KEY — Replace with your actual key from razorpay.com !!
var RZP_KEY = 'rzp_test_YOUR_KEY_HERE';

var COIN_PACKS = {
  starter:  { coins:500,  amount:4900,  label:'500 Coins',  price:'₹49'  },
  popular:  { coins:1200, amount:9900,  label:'1200 Coins', price:'₹99'  },
  mega:     { coins:2500, amount:19900, label:'2500 Coins', price:'₹199' },
};

// ─── VIP ─────────────────────────────────────────────────────────────────────
function checkVIP(){
  if(!UD)return false;
  var vip=UD.vip;
  if(!vip||!vip.active)return false;
  if(vip.expiresAt<Date.now()){// Expired
    db.ref('users/'+CU.uid+'/vip/active').set(false);return false;
  }
  return true;
}

function updVIPUI(){
  var isVIP=checkVIP();
  var vc=document.getElementById('vip-card');if(vc){vc.classList.toggle('vip-active',isVIP);}
  var vt=document.getElementById('vip-title');if(vt)vt.textContent=isVIP?'You are VIP! 👑':'Unlock ZapZone VIP!';
  var vd=document.getElementById('vip-desc');if(vd)vd.textContent=isVIP?'All premium perks unlocked!':'Get premium perks every month';
  var vbw=document.getElementById('vip-btn-wrap');if(vbw)vbw.style.display=isVIP?'none':'block';
  var vam=document.getElementById('vip-active-msg');if(vam)vam.style.display=isVIP?'block':'none';
  if(isVIP){
    var vbadge=document.getElementById('vip-badge-lbl');if(vbadge)vbadge.textContent='👑 VIP ACTIVE ✅';
    var vexp=document.getElementById('vip-exp');
    if(vexp&&UD.vip)vexp.textContent=new Date(UD.vip.expiresAt).toLocaleDateString('en-IN');
    var vst=document.getElementById('vip-spin-tag');if(vst)vst.style.display='inline';
  }
}

async function buyVIP(){
  if(!CU||!UD){alert('Please login first!');return;}
  if(checkVIP()){alert('You already have active VIP! ✅');return;}
  if(RZP_KEY==='rzp_test_YOUR_KEY_HERE'){
    // Demo mode - simulate purchase
    var confirmed=confirm('DEMO MODE\n\nIn real app, Razorpay payment of ₹199 will open.\n\nSimulate VIP activation for testing?');
    if(!confirmed)return;
    await activateVIP();return;
  }
  var options={
    key: RZP_KEY,
    amount: 19900,// ₹199 in paise
    currency: 'INR',
    name: 'ZapZone',
    description: 'VIP Membership - 1 Month',
    image: 'https://mahapatraswapnajit-prog.github.io/ZapZone/zapzone.html',
    prefill:{name:UD.name||'Player',email:(UD.username||'user')+'@zapzone.app'},
    theme:{color:'#a855f7'},
    handler: async function(response){
      // Payment successful
      await activateVIP();
      await db.ref('payments/'+CU.uid+'/vip').push({
        paymentId:response.razorpay_payment_id,ts:Date.now(),amount:199
      });
    }
  };
  var rzp=new Razorpay(options);rzp.open();
}

async function activateVIP(){
  var now=Date.now();
  var expiry=now+(30*24*60*60*1000);// 30 days
  if(!UD.vip)UD.vip={};
  UD.vip={active:true,activatedAt:now,expiresAt:expiry};
  await db.ref('users/'+CU.uid+'/vip').set(UD.vip);
  if(!UD.badges)UD.badges={};
  UD.badges.vipMember=true;
  await db.ref('users/'+CU.uid+'/badges/vipMember').set(true);
  updVIPUI();buildBadges();
  alert('🎉 Welcome to VIP! Enjoy your premium perks for 30 days! 👑');
}

// ─── COIN PACKS ───────────────────────────────────────────────────────────────
async function buyCoins(packId){
  if(!CU||!UD){alert('Please login first!');return;}
  var pack=COIN_PACKS[packId];if(!pack)return;
  if(RZP_KEY==='rzp_test_YOUR_KEY_HERE'){
    var confirmed=confirm('DEMO MODE\n\nIn real app, Razorpay payment of '+pack.price+' will open.\n\nSimulate adding '+pack.coins+' coins for testing?');
    if(!confirmed)return;
    await addCoins(pack.coins,'Coin Pack: '+pack.label);return;
  }
  var options={
    key:RZP_KEY,
    amount:pack.amount,
    currency:'INR',
    name:'ZapZone',
    description:pack.label,
    prefill:{name:UD.name||'Player',email:(UD.username||'user')+'@zapzone.app'},
    theme:{color:'#a855f7'},
    handler:async function(response){
      await addCoins(pack.coins,'Coin Pack: '+pack.label);
      await db.ref('payments/'+CU.uid+'/coins').push({
        paymentId:response.razorpay_payment_id,ts:Date.now(),
        amount:pack.amount/100,coins:pack.coins,pack:packId
      });
    }
  };
  var rzp=new Razorpay(options);rzp.open();
}

async function addCoins(amount, reason){
  if(!UD)return;
  UD.coins=(UD.coins||0)+amount;
  await db.ref('users/'+CU.uid+'/coins').set(UD.coins);
  updShopCoins();updQCoins();updProf();
  alert('🎉 '+amount+' coins added!\n'+reason+'\nTotal: '+UD.coins+' 🪙');
  if(UD.coins>=500&&!(UD.badges&&UD.badges.richKid))awardBadge('richKid');
}

// ─── REWARDED ADS ─────────────────────────────────────────────────────────────
var adInterval=null;var adWatching=false;

function getAdCount(){
  var today=new Date().toDateString();
  var stored=localStorage?localStorage.getItem('zz_ads_'+today):null;
  return stored?parseInt(stored):0;
}
function setAdCount(n){
  var today=new Date().toDateString();
  if(localStorage)localStorage.setItem('zz_ads_'+today,n);
}
function updAdUI(){
  var used=getAdCount();var left=5-used;
  var el=document.getElementById('ad-left');if(el)el.textContent=left;
  var btn=document.getElementById('ad-btn');
  if(btn){btn.disabled=left<=0;btn.style.opacity=left<=0?'0.5':'1';btn.textContent=left<=0?'✅ Done for today!':'📺 Watch Ad (+25 🪙)';}
  var cnt=document.getElementById('ad-count-disp');
  if(cnt)cnt.style.color=left<=0?'#7070a0':'#4361ee';
}

async function watchAd(){
  if(adWatching)return;
  var used=getAdCount();
  if(used>=5){alert('You have watched 5 ads today! Come back tomorrow 😊');return;}
  if(!CU||!UD){alert('Please login first!');return;}
  adWatching=true;
  var btn=document.getElementById('ad-btn');if(btn){btn.disabled=true;btn.textContent='📺 Watching...';}
  var watching=document.getElementById('ad-watching');if(watching)watching.style.display='block';
  var timerEl=document.getElementById('ad-timer');
  var pfEl=document.getElementById('ad-pf');
  var t=30;
  adInterval=setInterval(async function(){
    t--;
    if(timerEl)timerEl.textContent=t;
    if(pfEl)pfEl.style.width=((30-t)/30*100)+'%';
    if(t<=0){
      clearInterval(adInterval);
      adWatching=false;
      if(watching)watching.style.display='none';
      setAdCount(used+1);
      await addCoins(25,'Rewarded Ad');
      updAdUI();
    }
  },1000);
}

// ─── UPDATE SPIN FOR VIP ──────────────────────────────────────────────────────
var spinPrizes=[
  {label:'10 🪙',coins:10},{label:'25 🪙',coins:25},{label:'Try Again',coins:0},
  {label:'50 🪙',coins:50},{label:'Try Again',coins:0},{label:'100 🪙',coins:100},
  {label:'Try Again',coins:0},{label:'200 🪙',coins:200}
];
var spinning=false;

async function doSpin(){
  if(spinning)return;
  var isVIP=checkVIP();
  var cost=isVIP?0:50;
  if(!isVIP&&(!UD||(UD.coins||0)<50)){alert('Need 50 🪙 coins to spin!\nOr get VIP for FREE spins! 👑');return;}
  spinning=true;
  if(cost>0){UD.coins=(UD.coins||0)-cost;await db.ref('users/'+CU.uid+'/coins').set(UD.coins);updShopCoins();updQCoins();}
  var result=document.getElementById('spin-result');result.textContent='';
  var wheel=document.getElementById('spin-wheel');
  var deg=1440+Math.random()*360;
  wheel.style.transform='rotate('+deg+'deg)';wheel.textContent='🎰';
  setTimeout(async function(){
    var idx=Math.floor(Math.random()*spinPrizes.length);var prize=spinPrizes[idx];
    wheel.textContent=prize.coins>0?'🪙':'😅';
    if(prize.coins>0){
      await addCoins(prize.coins,'Spin to Win!');
      result.textContent='🎉 You won '+prize.label+'!';result.style.color='#06d6a0';
    }else{result.textContent='😅 Try again!';result.style.color='#ff6b6b';}
    spinning=false;
  },1600);
}

// ─── INIT ─────────────────────────────────────────────────────────────────────
window.onload=function(){initRegPickers();setTimeout(function(){showPage('login');},1800);};
</script>
</body>
</html>
