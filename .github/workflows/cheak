<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1, user-scalable=no">
<title>Dhanavanshi E-Mobility</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@600;700;800&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
  :root{
    --navy-950:#060B1A;
    --navy-900:#0A1128;
    --navy-800:#101B3D;
    --navy-700:#182552;
    --gold:#D4A017;
    --gold-light:#F4C430;
    --teal:#2EC4B6;
    --teal-light:#5EEAD4;
    --white:#F5F7FA;
    --gray:#8B93A7;
    --danger:#E8574A;
    --success:#39C68C;
    --pending:#E8A93A;
    --radius:20px;
  }
  *{box-sizing:border-box; -webkit-tap-highlight-color:transparent;}
  html,body{margin:0;padding:0;}
  body{
    font-family:'Inter',sans-serif;
    background:
      radial-gradient(circle at 20% -10%, #1B2A5E 0%, transparent 45%),
      radial-gradient(circle at 100% 110%, #0E2E2A 0%, transparent 50%),
      var(--navy-950);
    min-height:100vh;
    display:flex;
    align-items:flex-start;
    justify-content:center;
    color:var(--white);
    padding:24px 12px 60px;
  }
  h1,h2,h3,.font-display{font-family:'Poppins',sans-serif;}
  #app{
    width:100%;
    max-width:420px;
    background:linear-gradient(160deg, var(--navy-900) 0%, var(--navy-950) 100%);
    border-radius:32px;
    border:1px solid rgba(255,255,255,0.06);
    box-shadow:
      0 30px 60px -20px rgba(0,0,0,0.7),
      0 0 0 1px rgba(255,255,255,0.02) inset,
      0 1px 0 rgba(255,255,255,0.08) inset;
    overflow:hidden;
    position:relative;
    min-height:640px;
  }
  .screen{ padding:28px 22px 32px; display:none; animation:fadeUp .35s ease; }
  .screen.active{ display:block; }
  @keyframes fadeUp{ from{opacity:0; transform:translateY(10px);} to{opacity:1; transform:translateY(0);} }

  .brand-row{ display:flex; align-items:center; gap:12px; margin-bottom:6px; }
  .bolt{
    width:46px;height:46px;border-radius:14px;
    background:linear-gradient(135deg, var(--teal) 0%, var(--gold) 130%);
    display:flex;align-items:center;justify-content:center;
    box-shadow:0 8px 20px -4px rgba(46,196,182,0.5), 0 0 0 1px rgba(255,255,255,0.15) inset;
    transform:perspective(300px) rotateX(6deg) rotateY(-6deg);
  }
  .bolt svg{width:24px;height:24px;}
  .brand-name{ font-size:15px; font-weight:800; letter-spacing:0.5px; line-height:1.15; }
  .brand-name span{ display:block; font-family:'Inter'; font-weight:600; font-size:10.5px; letter-spacing:2.5px; color:var(--teal-light); margin-top:2px; }

  .hero{ margin-top:36px; text-align:center; }
  .hero-badge{
    width:112px;height:112px;margin:0 auto 22px;
    border-radius:32px;
    background:radial-gradient(circle at 30% 20%, #234066, #0B1330 70%);
    display:flex;align-items:center;justify-content:center;
    box-shadow:0 20px 40px -12px rgba(212,160,23,0.35), 0 0 0 1px rgba(255,255,255,0.06) inset;
    transform:perspective(500px) rotateX(10deg);
    position:relative;
  }
  .hero-badge::after{
    content:'';position:absolute;inset:-2px;border-radius:34px;
    background:conic-gradient(from 180deg, var(--teal), var(--gold), var(--teal));
    z-index:-1; opacity:.55; filter:blur(10px);
  }
  .hero-badge svg{width:56px;height:56px;}
  .hero h1{ font-size:22px; margin:0 0 6px; font-weight:800; }
  .hero p{ color:var(--gray); font-size:13.5px; line-height:1.6; margin:0 auto 28px; max-width:280px; }

  .btn{
    width:100%; border:none; border-radius:16px; padding:15px 18px;
    font-family:'Inter'; font-weight:700; font-size:14.5px; cursor:pointer;
    display:flex; align-items:center; justify-content:center; gap:8px;
    transition:transform .15s ease, box-shadow .15s ease;
  }
  .btn:active{ transform:scale(0.97); }
  .btn:disabled{ opacity:.55; cursor:not-allowed; }
  .btn-primary{
    background:linear-gradient(135deg, var(--teal) 0%, #1FA396 100%);
    color:#04231F;
    box-shadow:0 14px 26px -10px rgba(46,196,182,0.55), 0 1px 0 rgba(255,255,255,0.3) inset;
  }
  .btn-gold{
    background:linear-gradient(135deg, var(--gold-light) 0%, var(--gold) 100%);
    color:#2B1D02;
    box-shadow:0 14px 26px -10px rgba(212,160,23,0.5), 0 1px 0 rgba(255,255,255,0.3) inset;
  }
  .btn-ghost{ background:rgba(255,255,255,0.05); color:var(--white); border:1px solid rgba(255,255,255,0.1); }
  .btn-danger{ background:rgba(232,87,74,0.12); color:#FF8A7A; border:1px solid rgba(232,87,74,0.3); }

  .top-row{ display:flex; align-items:center; gap:10px; margin-bottom:22px; }
  .icon-btn{
    width:36px;height:36px;border-radius:11px;
    background:rgba(255,255,255,0.05); border:1px solid rgba(255,255,255,0.08);
    display:flex;align-items:center;justify-content:center; cursor:pointer; flex-shrink:0;
  }
  .icon-btn svg{ width:16px;height:16px; }
  .top-title{ font-size:15px; font-weight:700; }

  .field{ margin-bottom:16px; }
  .field label{ display:block; font-size:11.5px; font-weight:600; color:var(--gray); margin-bottom:7px; letter-spacing:0.3px; text-transform:uppercase; }
  .field input, .field select{
    width:100%; background:var(--navy-800); border:1px solid rgba(255,255,255,0.08);
    border-radius:13px; padding:13px 14px; color:var(--white); font-size:14.5px; font-family:'Inter';
    outline:none; transition:border-color .15s;
  }
  .field input:focus{ border-color:var(--teal); }
  .field input::placeholder{ color:#5A6280; }
  .field-photo{ display:flex; align-items:center; gap:12px; }
  .photo-preview{ width:56px;height:56px;border-radius:14px;object-fit:cover; background:var(--navy-800); border:1px solid rgba(255,255,255,0.1); flex-shrink:0; }
  .upload-label{ flex:1; text-align:center; padding:12px; border-radius:13px; border:1.5px dashed rgba(255,255,255,0.15); font-size:12.5px; color:var(--gray); cursor:pointer; }
  .upload-label:hover{ border-color:var(--teal); color:var(--teal-light); }

  .upload-progress-wrap{ display:none; align-items:center; gap:8px; margin-top:8px; }
  .upload-progress-wrap.show{ display:flex; }
  .upload-progress-track{ flex:1; height:7px; border-radius:6px; background:rgba(255,255,255,0.08); overflow:hidden; }
  .upload-progress-fill{ height:100%; width:0%; border-radius:6px; background:linear-gradient(90deg, var(--teal), var(--teal-light)); transition:width .2s ease; }
  .upload-progress-pct{ font-size:11px; font-weight:700; color:var(--teal-light); min-width:36px; text-align:right; }
  .upload-progress-pct.done{ color:#7EE8B8; }

  .helper{ font-size:11.5px; color:var(--gray); margin-top:8px; text-align:center; line-height:1.5; }
  .msg{ font-size:12.5px; padding:10px 12px; border-radius:11px; margin-bottom:14px; display:none; }
  .msg.show{ display:block; }
  .msg.error{ background:rgba(232,87,74,0.12); color:#FF9A8C; border:1px solid rgba(232,87,74,0.25); }
  .msg.ok{ background:rgba(57,198,140,0.12); color:#7EE8B8; border:1px solid rgba(57,198,140,0.25); }
  .msg.info{ background:rgba(46,196,182,0.1); color:var(--teal-light); border:1px solid rgba(46,196,182,0.25); }

  .result-card{
    background:linear-gradient(160deg, var(--navy-800), var(--navy-900));
    border-radius:22px; padding:22px; border:1px solid rgba(255,255,255,0.06);
    box-shadow:0 20px 40px -20px rgba(0,0,0,0.6), 0 1px 0 rgba(255,255,255,0.05) inset;
    transform:perspective(600px) rotateX(2deg);
  }
  .cust-row{ display:flex; align-items:center; gap:14px; margin-bottom:18px; }
  .cust-photo{ width:64px;height:64px;border-radius:18px;object-fit:cover; border:2px solid var(--teal); box-shadow:0 0 0 4px rgba(46,196,182,0.12); }
  .cust-photo-fallback{ width:64px;height:64px;border-radius:18px; background:linear-gradient(135deg, var(--teal), var(--gold)); display:flex;align-items:center;justify-content:center; font-weight:800; font-size:22px; color:#04231F; }
  .cust-name{ font-size:17px; font-weight:800; }
  .cust-model{ font-size:12.5px; color:var(--teal-light); font-weight:600; margin-top:2px; }

  .info-grid{ display:grid; grid-template-columns:1fr 1fr; gap:10px; margin-bottom:18px; }
  .info-box{ background:rgba(255,255,255,0.04); border-radius:13px; padding:11px 13px; }
  .info-box .lbl{ font-size:10px; text-transform:uppercase; letter-spacing:0.5px; color:var(--gray); margin-bottom:4px; }
  .info-box .val{ font-size:13px; font-weight:700; word-break:break-all; }

  .bill-box{ background:rgba(212,160,23,0.08); border:1px solid rgba(212,160,23,0.25); border-radius:14px; padding:14px; display:flex; align-items:center; justify-content:space-between; margin-bottom:18px; }
  .bill-box .lbl{ font-size:11px; color:var(--gold-light); text-transform:uppercase; letter-spacing:0.5px; }
  .bill-box .amt{ font-size:19px; font-weight:800; color:var(--gold-light); margin-top:2px; }
  .bill-photo-btn{ font-size:11.5px; color:var(--teal-light); background:rgba(46,196,182,0.12); padding:8px 12px; border-radius:10px; border:1px solid rgba(46,196,182,0.3); cursor:pointer; }

  .service-title{ font-size:11.5px; text-transform:uppercase; letter-spacing:0.5px; color:var(--gray); margin:0 0 10px; }
  .service-item{ display:flex; align-items:center; justify-content:space-between; background:rgba(255,255,255,0.03); border-radius:13px; padding:12px 14px; margin-bottom:9px; }
  .service-item .svc-name{ font-size:13px; font-weight:700; }
  .service-item .svc-sub{ font-size:11px; color:var(--gray); margin-top:2px; }
  .pill{ font-size:11px; font-weight:800; padding:5px 12px; border-radius:20px; letter-spacing:0.3px; }
  .pill.paid{ background:rgba(57,198,140,0.15); color:var(--success); }
  .pill.pending{ background:rgba(232,169,58,0.15); color:var(--pending); }

  .hidden-gear{
    position:fixed; bottom:14px; right:calc(50% - 210px + 14px);
    width:30px;height:30px; border-radius:50%;
    background:rgba(255,255,255,0.03); border:1px solid rgba(255,255,255,0.05);
    display:flex;align-items:center;justify-content:center; cursor:pointer;
    opacity:0.18; transition:opacity .2s; z-index:50;
  }
  .hidden-gear:hover{ opacity:0.6; }
  .hidden-gear svg{ width:14px;height:14px; }
  @media (max-width:460px){ .hidden-gear{ right:14px; } }

  .admin-list-item{ background:var(--navy-800); border-radius:16px; padding:14px; margin-bottom:10px; display:flex; align-items:center; gap:12px; border:1px solid rgba(255,255,255,0.06); }
  .admin-list-item .ali-photo{ width:42px;height:42px;border-radius:12px;object-fit:cover; background:var(--navy-700); flex-shrink:0; }
  .admin-list-item .ali-info{ flex:1; min-width:0; }
  .admin-list-item .ali-name{ font-size:13.5px; font-weight:700; }
  .admin-list-item .ali-sub{ font-size:11px; color:var(--gray); margin-top:2px; overflow:hidden; text-overflow:ellipsis; white-space:nowrap; }
  .admin-actions{ display:flex; gap:6px; flex-shrink:0; }
  .admin-actions .icon-btn{ width:32px;height:32px; }

  .toggle-row{ display:flex; align-items:center; justify-content:space-between; background:var(--navy-800); border-radius:13px; padding:12px 14px; margin-bottom:10px; }
  .toggle-row .t-label{ font-size:12.5px; font-weight:600; }
  .switch{ position:relative; width:44px;height:25px; }
  .switch input{ opacity:0; width:0; height:0; }
  .slider{ position:absolute; inset:0; background:#2A3358; border-radius:20px; cursor:pointer; transition:.2s; }
  .slider::before{ content:''; position:absolute; width:19px;height:19px; left:3px; top:3px; background:#fff; border-radius:50%; transition:.2s; }
  input:checked + .slider{ background:var(--success); }
  input:checked + .slider::before{ transform:translateX(19px); }

  .empty-state{ text-align:center; padding:40px 10px; color:var(--gray); }
  .empty-state svg{ width:44px;height:44px; margin-bottom:12px; opacity:.5; }
  .empty-state p{ font-size:13px; }

  .loading-dot{ display:inline-block; width:6px;height:6px;border-radius:50%; background:var(--teal); animation:blink 1s infinite ease-in-out; }
  @keyframes blink{ 0%,100%{opacity:.2;} 50%{opacity:1;} }

  .scrollarea{ max-height:420px; overflow-y:auto; margin:0 -6px; padding:0 6px; }
  .scrollarea::-webkit-scrollbar{ width:5px; }
  .scrollarea::-webkit-scrollbar-thumb{ background:rgba(255,255,255,0.1); border-radius:10px; }

  .divider{ height:1px; background:rgba(255,255,255,0.07); margin:20px 0; }
  .footer-note{ text-align:center; font-size:10.5px; color:#4C5474; margin-top:18px; }

  .config-warn{
    background:rgba(232,169,58,0.1); border:1px solid rgba(232,169,58,0.3);
    border-radius:14px; padding:16px; font-size:12px; line-height:1.7; color:#F0C568;
  }
  .config-warn code{ background:rgba(0,0,0,0.3); padding:2px 6px; border-radius:5px; font-size:11px; }
</style>
</head>
<body>

<div id="app">

  <!-- CONFIG WARNING (shown only if firebaseConfig not filled in) -->
  <div class="screen" id="screen-config-warning">
    <div class="brand-row"><div class="bolt"><svg viewBox="0 0 24 24" fill="none"><path d="M13 2L4 14h6l-1 8 9-12h-6l1-8z" fill="#04231F"/></svg></div>
      <div class="brand-name">DHANAVANSHI<span>E-MOBILITY</span></div>
    </div>
    <div style="margin-top:24px;" class="config-warn">
      <b>⚠️ Firebase config baaki hai</b><br><br>
      Ye app real Firebase (Firestore + Storage) se juda hua hai, lekin abhi tak apna Firebase project connect nahi kiya gaya.<br><br>
      Neeche <code>&lt;script&gt;</code> section mein <code>firebaseConfig</code> object dhoondein aur apne Firebase project ki details bharein (Firebase Console → Project Settings → Your apps → SDK setup).<br><br>
      Config bharne ke baad ye warning apne aap gayab ho jayegi aur app normal chalne lagegi.
    </div>
  </div>

  <!-- ============ HOME / SPLASH ============ -->
  <div class="screen active" id="screen-home">
    <div class="brand-row">
      <div class="bolt"><svg viewBox="0 0 24 24" fill="none"><path d="M13 2L4 14h6l-1 8 9-12h-6l1-8z" fill="#04231F"/></svg></div>
      <div class="brand-name">DHANAVANSHI<span>E-MOBILITY</span></div>
    </div>

    <div class="hero">
      <div class="hero-badge">
        <svg viewBox="0 0 24 24" fill="none"><path d="M13 2L4 14h6l-1 8 9-12h-6l1-8z" stroke="url(#g1)" stroke-width="1.6" stroke-linejoin="round" fill="rgba(46,196,182,0.15)"/>
        <defs><linearGradient id="g1" x1="4" y1="2" x2="20" y2="22"><stop stop-color="#5EEAD4"/><stop offset="1" stop-color="#F4C430"/></linearGradient></defs></svg>
      </div>
      <h1>Apni Gaadi Check Karein</h1>
      <p>Chassis ya Battery Number daal kar apna bill, model aur free service status turant dekhein.</p>
      <button class="btn btn-primary" onclick="go('screen-search')">
        <svg viewBox="0 0 24 24" width="17" height="17" fill="none" stroke="#04231F" stroke-width="2.2"><circle cx="11" cy="11" r="7"/><path d="M21 21l-4.3-4.3"/></svg>
        Vehicle Check Karein
      </button>
    </div>
    <div class="divider"></div>
    <p class="footer-note">Dhanavanshi E-Mobility &copy; 2026 &middot; 2 Free Services Included</p>
  </div>

  <!-- ============ SEARCH ============ -->
  <div class="screen" id="screen-search">
    <div class="top-row">
      <div class="icon-btn" onclick="go('screen-home')"><svg viewBox="0 0 24 24" fill="none" stroke="#F5F7FA" stroke-width="2.2"><path d="M15 18l-6-6 6-6"/></svg></div>
      <div class="top-title">Vehicle Check</div>
    </div>
    <div id="search-msg" class="msg error"></div>
    <div class="field">
      <label>Chassis Number ya Battery Number</label>
      <input type="text" id="search-input" placeholder="Jaise: DHV12345678">
    </div>
    <button class="btn btn-primary" onclick="doSearch()"><span id="search-btn-label">Search Karein</span></button>
    <p class="helper">Number apni vehicle ki sale slip ya battery label par likha hota hai.</p>
  </div>

  <!-- ============ RESULT ============ -->
  <div class="screen" id="screen-result">
    <div class="top-row">
      <div class="icon-btn" onclick="go('screen-search')"><svg viewBox="0 0 24 24" fill="none" stroke="#F5F7FA" stroke-width="2.2"><path d="M15 18l-6-6 6-6"/></svg></div>
      <div class="top-title">Vehicle Details</div>
    </div>
    <div class="result-card" id="result-card"></div>
    <button class="btn btn-ghost" style="margin-top:16px;" onclick="go('screen-search')">Dusra Number Check Karein</button>
  </div>

  <!-- ============ HIDDEN GEAR -> ADMIN LOGIN ============ -->
  <div class="hidden-gear" onclick="go('screen-admin-login')" title="">
    <svg viewBox="0 0 24 24" fill="none" stroke="#8B93A7" stroke-width="1.8"><circle cx="12" cy="12" r="3"/><path d="M19.4 15a1.7 1.7 0 00.34 1.87l.06.06a2 2 0 11-2.83 2.83l-.06-.06a1.7 1.7 0 00-1.87-.34 1.7 1.7 0 00-1 1.55V21a2 2 0 11-4 0v-.09A1.7 1.7 0 009 19.4a1.7 1.7 0 00-1.87.34l-.06.06a2 2 0 11-2.83-2.83l.06-.06A1.7 1.7 0 004.6 15a1.7 1.7 0 00-1.55-1H3a2 2 0 110-4h.09A1.7 1.7 0 004.6 9a1.7 1.7 0 00-.34-1.87l-.06-.06a2 2 0 112.83-2.83l.06.06A1.7 1.7 0 009 4.6a1.7 1.7 0 001-1.55V3a2 2 0 114 0v.09a1.7 1.7 0 001 1.55 1.7 1.7 0 001.87-.34l.06-.06a2 2 0 112.83 2.83l-.06.06A1.7 1.7 0 0019.4 9a1.7 1.7 0 001.55 1H21a2 2 0 110 4h-.09a1.7 1.7 0 00-1.55 1z"/></svg>
  </div>

  <!-- ============ ADMIN LOGIN ============ -->
  <div class="screen" id="screen-admin-login">
    <div class="top-row">
      <div class="icon-btn" onclick="go('screen-home')"><svg viewBox="0 0 24 24" fill="none" stroke="#F5F7FA" stroke-width="2.2"><path d="M15 18l-6-6 6-6"/></svg></div>
      <div class="top-title">Admin Login</div>
    </div>
    <div id="login-msg" class="msg error"></div>
    <div class="field"><label>Username</label><input type="text" id="admin-user" placeholder="Username" autocomplete="off"></div>
    <div class="field"><label>Password</label><input type="password" id="admin-pass" placeholder="Password" autocomplete="off"></div>
    <button class="btn btn-gold" onclick="adminLogin()">Login</button>
  </div>

  <!-- ============ ADMIN DASHBOARD ============ -->
  <div class="screen" id="screen-admin-dash">
    <div class="top-row">
      <div class="icon-btn" onclick="adminLogout()"><svg viewBox="0 0 24 24" fill="none" stroke="#F5F7FA" stroke-width="2.2"><path d="M15 18l-6-6 6-6"/></svg></div>
      <div class="top-title" style="flex:1;">Admin Panel</div>
      <div class="icon-btn" onclick="openCustomerForm()"><svg viewBox="0 0 24 24" fill="none" stroke="#F5F7FA" stroke-width="2.2"><path d="M12 5v14M5 12h14"/></svg></div>
    </div>
    <div id="admin-list-wrap" class="scrollarea"></div>
  </div>

  <!-- ============ ADMIN CUSTOMER FORM ============ -->
  <div class="screen" id="screen-admin-form">
    <div class="top-row">
      <div class="icon-btn" onclick="go('screen-admin-dash'); renderAdminList();"><svg viewBox="0 0 24 24" fill="none" stroke="#F5F7FA" stroke-width="2.2"><path d="M15 18l-6-6 6-6"/></svg></div>
      <div class="top-title" id="form-title">Customer Add Karein</div>
    </div>
    <div id="form-msg" class="msg error"></div>
    <div class="scrollarea" style="max-height:520px;">
      <div class="field">
        <label>Customer Photo (Max 3MB)</label>
        <div class="field-photo">
          <img id="preview-customer-photo" class="photo-preview" src="" style="display:none;">
          <label class="upload-label" for="file-customer-photo">Photo Upload Karein</label>
          <input type="file" id="file-customer-photo" accept="image/*" style="display:none;" onchange="handlePhoto(this,'customer')">
        </div>
        <div class="upload-progress-wrap" id="progress-wrap-customer">
          <div class="upload-progress-track"><div class="upload-progress-fill" id="progress-fill-customer"></div></div>
          <span class="upload-progress-pct" id="progress-pct-customer">0%</span>
        </div>
      </div>
      <div class="field"><label>Customer Name</label><input type="text" id="f-name" placeholder="Jaise: Ramesh Kumar"></div>
      <div class="field"><label>Chassis Number</label><input type="text" id="f-chassis" placeholder="Jaise: DHV12345678"></div>
      <div class="field"><label>Battery Number</label><input type="text" id="f-battery" placeholder="Jaise: BAT98765"></div>
      <div class="field"><label>Model</label><input type="text" id="f-model" placeholder="Jaise: Dhanavanshi E-Rickshaw X1"></div>
      <div class="field"><label>Bill Amount (₹)</label><input type="text" inputmode="numeric" id="f-bill" placeholder="Jaise: 1,25,000" oninput="formatBillInput(this)"></div>
      <div class="field">
        <label>Bill (PDF Only, Max 3MB, Optional)</label>
        <div class="field-photo">
          <a id="preview-bill-photo" class="bill-photo-btn" href="#" target="_blank" style="display:none;">Bill PDF Dekhein</a>
          <label class="upload-label" for="file-bill-photo">Bill PDF Upload Karein</label>
          <input type="file" id="file-bill-photo" accept="application/pdf,.pdf" style="display:none;" onchange="handlePhoto(this,'bill')">
        </div>
        <div class="upload-progress-wrap" id="progress-wrap-bill">
          <div class="upload-progress-track"><div class="upload-progress-fill" id="progress-fill-bill"></div></div>
          <span class="upload-progress-pct" id="progress-pct-bill">0%</span>
        </div>
      </div>
      <div class="divider"></div>
      <p class="service-title">Free Service Status</p>
      <div class="toggle-row"><div class="t-label">Service 1 &middot; 1000 KM</div><label class="switch"><input type="checkbox" id="f-svc1"><span class="slider"></span></label></div>
      <div class="toggle-row"><div class="t-label">Service 2 &middot; 2000 KM</div><label class="switch"><input type="checkbox" id="f-svc2"><span class="slider"></span></label></div>
    </div>
    <button class="btn btn-gold" style="margin-top:16px;" id="save-btn" onclick="saveCustomer()">Save Karein</button>
    <button class="btn btn-danger" style="margin-top:10px; display:none;" id="delete-btn" onclick="deleteCustomer()">Customer Delete Karein</button>
  </div>

</div>

<!-- ===================== FIREBASE (compat SDK — works from a double-clicked local file too) ===================== -->
<script src="https://www.gstatic.com/firebasejs/10.13.0/firebase-app-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.13.0/firebase-firestore-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/10.13.0/firebase-storage-compat.js"></script>
<script>
/* ==================================================================
   1) YAHAN APNI FIREBASE PROJECT KI DETAILS DAALEIN
   Firebase Console -> Project Settings -> "Your apps" -> SDK setup and configuration
   Storage/Firestore chalane ke liye project Blaze (pay-as-you-go) plan par hona zaroori hai.
   ================================================================== */
const firebaseConfig = {
  apiKey: "AIzaSyCpI-pIeDZLUE4P-ZMHEOX9AVSDgtyCp5s",
  authDomain: "dhanavanshi-e-mobility-servies.firebaseapp.com",
  projectId: "dhanavanshi-e-mobility-servies",
  storageBucket: "dhanavanshi-e-mobility-servies.firebasestorage.app",
  messagingSenderId: "896745161315",
  appId: "1:896745161315:web:ffd89134f37fcfc94bee56"
};

const isConfigured = firebaseConfig.apiKey !== "YOUR_API_KEY" && firebaseConfig.projectId !== "YOUR_PROJECT_ID";

let db, storage, firebaseReady = false;
try{
  if (isConfigured && typeof firebase !== 'undefined') {
    firebase.initializeApp(firebaseConfig);
    db = firebase.firestore();
    storage = firebase.storage();
    firebaseReady = true;
  }
}catch(e){
  firebaseReady = false;
}

// ---------------- Navigation ----------------
function go(id){
  document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
  document.getElementById(id).classList.add('active');
  document.getElementById('app').scrollTop = 0;
}
// Home screen is already active by default in the HTML — app always opens normally,
// even if Firebase's CDN script is slow/blocked. Connection problems are only
// reported when an actual search/save is attempted (see below).

let editingChassis = null;
let selectedCustomerPhotoFile = null;
let selectedBillPhotoFile = null;

function safeKey(str){ return (str || '').trim().toLowerCase().replace(/\s+/g,''); }
function showMsg(elId, text, type){ const el=document.getElementById(elId); el.textContent=text; el.className='msg show '+type; }
function hideMsg(elId){ document.getElementById(elId).className='msg'; }
function escapeHtml(str){ return String(str).replace(/[&<>"']/g, m => ({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[m])); }

async function getAllCustomers(){
  const snap = await db.collection('customers').get();
  const out = [];
  snap.forEach(d => out.push(d.data()));
  return out;
}

// ---------------- Search ----------------
async function doSearch(){
  hideMsg('search-msg');
  if(!firebaseReady){ showMsg('search-msg','Internet connection check karein aur thodi der baad try karein.','error'); return; }
  const q = safeKey(document.getElementById('search-input').value);
  if(!q){ showMsg('search-msg','Kripya Chassis ya Battery Number daalein.','error'); return; }
  const label = document.getElementById('search-btn-label');
  label.innerHTML = 'Search ho raha hai <span class="loading-dot"></span>';

  let found = null;
  try{
    const dsnap = await db.collection('customers').doc(q).get();
    if(dsnap.exists) found = dsnap.data();
  }catch(e){}

  if(!found){
    try{
      const all = await getAllCustomers();
      found = all.find(c => safeKey(c.batteryNumber) === q || safeKey(c.chassisNumber) === q) || null;
    }catch(e){}
  }

  label.textContent = 'Search Karein';

  if(!found){ showMsg('search-msg','Koi record nahi mila. Number check karke dubara try karein.','error'); return; }
  renderResult(found);
  go('screen-result');
}

function renderResult(c){
  const svc1 = c.service1Paid ? '<span class="pill paid">PAID</span>' : '<span class="pill pending">PENDING</span>';
  const svc2 = c.service2Paid ? '<span class="pill paid">PAID</span>' : '<span class="pill pending">PENDING</span>';
  const photoHtml = c.customerPhotoUrl
    ? `<img class="cust-photo" src="${c.customerPhotoUrl}">`
    : `<div class="cust-photo-fallback">${(c.name||'?').charAt(0).toUpperCase()}</div>`;
  const billPhotoBtn = c.billPhotoUrl
    ? `<div class="bill-photo-btn" onclick="window.open('${c.billPhotoUrl}','_blank')">Bill Dekhein</div>` : '';

  document.getElementById('result-card').innerHTML = `
    <div class="cust-row">${photoHtml}
      <div><div class="cust-name">${escapeHtml(c.name||'-')}</div><div class="cust-model">${escapeHtml(c.model||'-')}</div></div>
    </div>
    <div class="info-grid">
      <div class="info-box"><div class="lbl">Chassis No.</div><div class="val">${escapeHtml(c.chassisNumber||'-')}</div></div>
      <div class="info-box"><div class="lbl">Battery No.</div><div class="val">${escapeHtml(c.batteryNumber||'-')}</div></div>
    </div>
    <div class="bill-box">
      <div><div class="lbl">Bill Amount</div><div class="amt">₹ ${c.billAmount ? Number(c.billAmount).toLocaleString('en-IN') : '-'}</div></div>
      ${billPhotoBtn}
    </div>
    <p class="service-title">Free Service Status</p>
    <div class="service-item"><div><div class="svc-name">Service 1</div><div class="svc-sub">1000 KM par</div></div>${svc1}</div>
    <div class="service-item"><div><div class="svc-name">Service 2</div><div class="svc-sub">2000 KM par</div></div>${svc2}</div>
  `;
}

// ---------------- Admin login (app-level gate, not Firebase Auth) ----------------
function adminLogin(){
  hideMsg('login-msg');
  const u = document.getElementById('admin-user').value.trim();
  const p = document.getElementById('admin-pass').value.trim();
  if(u === 'dhana' && p === 'dhana'){
    if(!firebaseReady){ showMsg('login-msg','Internet connection check karein aur thodi der baad try karein.','error'); return; }
    document.getElementById('admin-user').value=''; document.getElementById('admin-pass').value='';
    go('screen-admin-dash'); renderAdminList();
  }else{ showMsg('login-msg','Galat username ya password.','error'); }
}
function adminLogout(){ go('screen-home'); }

// ---------------- Admin list ----------------
async function renderAdminList(){
  const wrap = document.getElementById('admin-list-wrap');
  wrap.innerHTML = '<div class="empty-state"><p>Load ho raha hai...</p></div>';
  let all = [];
  try{ all = await getAllCustomers(); }catch(e){
    wrap.innerHTML = `<div class="empty-state"><p>Data load nahi ho paya: ${escapeHtml(e.message)}</p></div>`;
    return;
  }
  if(all.length === 0){
    wrap.innerHTML = `<div class="empty-state">
      <svg viewBox="0 0 24 24" fill="none" stroke="#8B93A7" stroke-width="1.6"><circle cx="12" cy="8" r="4"/><path d="M4 21c0-4 4-6 8-6s8 2 8 6"/></svg>
      <p>Abhi tak koi customer nahi joda gaya.<br>Upar + button se naya customer add karein.</p></div>`;
    return;
  }
  wrap.innerHTML = all.map(c => {
    const photo = c.customerPhotoUrl ? `<img class="ali-photo" src="${c.customerPhotoUrl}">` : `<div class="ali-photo" style="display:flex;align-items:center;justify-content:center;font-weight:800;">${(c.name||'?').charAt(0).toUpperCase()}</div>`;
    return `<div class="admin-list-item">${photo}
      <div class="ali-info"><div class="ali-name">${escapeHtml(c.name||'-')}</div><div class="ali-sub">${escapeHtml(c.chassisNumber||'-')} &middot; ${escapeHtml(c.model||'-')}</div></div>
      <div class="admin-actions"><div class="icon-btn" onclick='openCustomerForm(${JSON.stringify(c.chassisNumber)})'>
        <svg viewBox="0 0 24 24" fill="none" stroke="#5EEAD4" stroke-width="2"><path d="M12 20h9"/><path d="M16.5 3.5a2.1 2.1 0 013 3L7 19l-4 1 1-4 12.5-12.5z"/></svg></div></div>
    </div>`;
  }).join('');
}

// ---------------- Bill amount live comma formatting (Indian style) ----------------
function formatBillInput(input){
  let digits = input.value.replace(/[^0-9]/g, '');
  if(!digits){ input.value = ''; return; }
  input.value = Number(digits).toLocaleString('en-IN');
}

// ---------------- Photo/PDF select (preview only, upload happens on save) ----------------
const MAX_FILE_SIZE = 3 * 1024 * 1024; // 3MB

function handlePhoto(input, kind){
  const file = input.files[0];
  if(!file) return;
  hideMsg('form-msg');

  if(file.size > MAX_FILE_SIZE){
    showMsg('form-msg', (kind==='bill' ? 'Bill PDF' : 'Photo') + ' ka size 3MB se zyada nahi ho sakta.', 'error');
    input.value = '';
    return;
  }

  if(kind === 'bill'){
    if(file.type !== 'application/pdf'){
      showMsg('form-msg','Bill sirf PDF file honi chahiye.','error');
      input.value = '';
      return;
    }
    selectedBillPhotoFile = file;
    const link = document.getElementById('preview-bill-photo');
    link.href = URL.createObjectURL(file);
    link.textContent = 'Bill PDF Dekhein (' + file.name + ')';
    link.style.display = 'inline-block';
  } else {
    const reader = new FileReader();
    reader.onload = e => {
      const img = new Image();
      img.onload = () => {
        const maxDim = 1000;
        let { width, height } = img;
        if(width > maxDim || height > maxDim){
          if(width > height){ height = Math.round(height * maxDim / width); width = maxDim; }
          else { width = Math.round(width * maxDim / height); height = maxDim; }
        }
        const canvas = document.createElement('canvas');
        canvas.width = width; canvas.height = height;
        canvas.getContext('2d').drawImage(img, 0, 0, width, height);
        canvas.toBlob(blob => {
          selectedCustomerPhotoFile = blob || file; // compressed blob for fast upload, fallback to original
        }, 'image/jpeg', 0.75);
        const previewImg = document.getElementById('preview-customer-photo');
        previewImg.src = canvas.toDataURL('image/jpeg', 0.75);
        previewImg.style.display = 'block';
      };
      img.onerror = () => { selectedCustomerPhotoFile = file; };
      img.src = e.target.result;
    };
    reader.readAsDataURL(file);
  }
}

// ---------------- Admin form (add/edit) ----------------
async function openCustomerForm(chassisNumber){
  hideMsg('form-msg');
  editingChassis = chassisNumber || null;
  selectedCustomerPhotoFile = null; selectedBillPhotoFile = null;
  document.getElementById('form-title').textContent = editingChassis ? 'Customer Edit Karein' : 'Customer Add Karein';
  document.getElementById('delete-btn').style.display = editingChassis ? 'block' : 'none';

  ['name','chassis','battery','model','bill'].forEach(f => document.getElementById('f-'+f).value = '');
  document.getElementById('f-svc1').checked = false;
  document.getElementById('f-svc2').checked = false;
  const custImg = document.getElementById('preview-customer-photo');
  custImg.src = ''; custImg.style.display = 'none';
  const billLink = document.getElementById('preview-bill-photo');
  billLink.href = '#'; billLink.textContent = 'Bill PDF Dekhein'; billLink.style.display = 'none';
  resetProgressBar('customer');
  resetProgressBar('bill');

  if(editingChassis){
    try{
      const dsnap = await db.collection('customers').doc(safeKey(editingChassis)).get();
      if(dsnap.exists){
        const c = dsnap.data();
        document.getElementById('f-name').value = c.name || '';
        document.getElementById('f-chassis').value = c.chassisNumber || '';
        document.getElementById('f-battery').value = c.batteryNumber || '';
        document.getElementById('f-model').value = c.model || '';
        document.getElementById('f-bill').value = c.billAmount ? Number(c.billAmount).toLocaleString('en-IN') : '';
        document.getElementById('f-svc1').checked = !!c.service1Paid;
        document.getElementById('f-svc2').checked = !!c.service2Paid;
        if(c.customerPhotoUrl){ const img=document.getElementById('preview-customer-photo'); img.src=c.customerPhotoUrl; img.style.display='block'; }
        if(c.billPhotoUrl){ const link=document.getElementById('preview-bill-photo'); link.href=c.billPhotoUrl; link.textContent='Bill PDF Dekhein'; link.style.display='inline-block'; }
      }
    }catch(e){}
  }
  go('screen-admin-form');
}

function resetProgressBar(key){
  const wrap = document.getElementById('progress-wrap-'+key);
  const fill = document.getElementById('progress-fill-'+key);
  const pct = document.getElementById('progress-pct-'+key);
  wrap.classList.remove('show');
  fill.style.width = '0%';
  pct.textContent = '0%';
  pct.classList.remove('done');
}

function setProgressBar(key, percent){
  const wrap = document.getElementById('progress-wrap-'+key);
  const fill = document.getElementById('progress-fill-'+key);
  const pct = document.getElementById('progress-pct-'+key);
  wrap.classList.add('show');
  fill.style.width = percent + '%';
  if(percent >= 100){
    pct.textContent = 'Complete';
    pct.classList.add('done');
  } else {
    pct.textContent = percent + '%';
    pct.classList.remove('done');
  }
}

async function saveCustomer(){
  hideMsg('form-msg');
  const name = document.getElementById('f-name').value.trim();
  const chassisNumber = document.getElementById('f-chassis').value.trim();
  const batteryNumber = document.getElementById('f-battery').value.trim();
  const model = document.getElementById('f-model').value.trim();
  const billAmount = document.getElementById('f-bill').value.trim().replace(/,/g, '');

  if(!name || !chassisNumber){ showMsg('form-msg','Name aur Chassis Number zaroori hai.','error'); return; }
  if(!firebaseReady){ showMsg('form-msg','Internet connection check karein aur thodi der baad try karein.','error'); return; }

  const newKey = safeKey(chassisNumber);
  const saveBtn = document.getElementById('save-btn');
  saveBtn.disabled = true; saveBtn.textContent = 'Save ho raha hai...';

  try{
    // If chassis number changed while editing, move the doc + storage files
    if(editingChassis && safeKey(editingChassis) !== newKey){
      await db.collection('customers').doc(safeKey(editingChassis)).delete();
    }

    let customerPhotoUrl = document.getElementById('preview-customer-photo').src.startsWith('http')
      ? document.getElementById('preview-customer-photo').src : '';
    let billPhotoUrl = document.getElementById('preview-bill-photo').href.startsWith('http')
      ? document.getElementById('preview-bill-photo').href : '';

    const progress = { customer: 0, bill: 0 };
    const updateBtnProgress = () => {
      const parts = [];
      if(selectedCustomerPhotoFile) parts.push('Photo ' + progress.customer + '%');
      if(selectedBillPhotoFile) parts.push('Bill ' + progress.bill + '%');
      saveBtn.textContent = parts.length ? ('Upload ho raha hai...') : 'Save ho raha hai...';
    };

    function uploadWithProgress(ref, file, contentType, key){
      setProgressBar(key, 0);
      return new Promise((resolve, reject) => {
        const task = ref.put(file, {contentType});
        task.on('state_changed',
          snap => {
            progress[key] = Math.round((snap.bytesTransferred / snap.totalBytes) * 100);
            setProgressBar(key, progress[key]);
            updateBtnProgress();
          },
          reject,
          () => { setProgressBar(key, 100); resolve(); }
        );
      });
    }

    const uploadJobs = [];
    if(selectedCustomerPhotoFile){
      const r = storage.ref(`customers/${newKey}/customer-photo.jpg`);
      uploadJobs.push(
        uploadWithProgress(r, selectedCustomerPhotoFile, 'image/jpeg', 'customer')
          .then(() => r.getDownloadURL())
          .then(url => { customerPhotoUrl = url; })
      );
    }
    if(selectedBillPhotoFile){
      const r = storage.ref(`customers/${newKey}/bill-photo.pdf`);
      uploadJobs.push(
        uploadWithProgress(r, selectedBillPhotoFile, 'application/pdf', 'bill')
          .then(() => r.getDownloadURL())
          .then(url => { billPhotoUrl = url; })
      );
    }
    await Promise.all(uploadJobs);
    saveBtn.textContent = 'Save ho raha hai...';

    const data = {
      name, chassisNumber, batteryNumber, model,
      billAmount: billAmount ? Number(billAmount) : null,
      customerPhotoUrl, billPhotoUrl,
      service1Paid: document.getElementById('f-svc1').checked,
      service2Paid: document.getElementById('f-svc2').checked,
      updatedAt: Date.now()
    };

    await db.collection('customers').doc(newKey).set(data);
    go('screen-admin-dash');
    renderAdminList();
  }catch(e){
    showMsg('form-msg', 'Save nahi ho paya: ' + e.message, 'error');
  }finally{
    saveBtn.disabled = false; saveBtn.textContent = 'Save Karein';
  }
}

async function deleteCustomer(){
  if(!editingChassis) return;
  if(!confirm('Kya aap sach mein is customer ko delete karna chahte hain?')) return;
  const key = safeKey(editingChassis);
  try{
    await db.collection('customers').doc(key).delete();
    try{ await storage.ref(`customers/${key}/customer-photo.jpg`).delete(); }catch(e){}
    try{ await storage.ref(`customers/${key}/bill-photo.pdf`).delete(); }catch(e){}
  }catch(e){}
  go('screen-admin-dash');
  renderAdminList();
}
</script>

</body>
</html>
