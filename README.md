<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SA:MP Scripts Forum</title>
<link href="https://fonts.googleapis.com/css2?family=Oswald:wght@400;600;700&family=Share+Tech+Mono&family=Rajdhani:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  *{margin:0;padding:0;box-sizing:border-box}
  body{background:#0a0a0c;color:#c8c8c8;font-family:'Rajdhani',sans-serif;min-height:100vh}
  header{background:#0d0d10;border-bottom:2px solid #c8a84b;padding:0 2rem}
  .header-inner{max-width:1100px;margin:0 auto;display:flex;align-items:center;justify-content:space-between;height:64px}
  .logo{font-family:'Oswald',sans-serif;font-size:1.6rem;font-weight:700;letter-spacing:3px;color:#c8a84b;text-transform:uppercase}
  .logo span{color:#e8e8e8}
  .nav{display:flex;gap:1.5rem}
  .nav a{color:#888;font-size:.85rem;letter-spacing:1px;text-transform:uppercase;text-decoration:none;transition:color .2s}
  .nav a:hover{color:#c8a84b}
  .main{max-width:1100px;margin:0 auto;padding:2rem}
  .page-title{font-family:'Oswald',sans-serif;font-size:1.8rem;font-weight:600;color:#e0e0e0;letter-spacing:2px;text-transform:uppercase;margin-bottom:.3rem}
  .page-sub{color:#666;font-size:.85rem;letter-spacing:1px;margin-bottom:2rem;border-bottom:1px solid #1e1e24;padding-bottom:1rem}
  .section{margin-bottom:2rem}
  .section-header{display:flex;align-items:center;gap:.75rem;margin-bottom:.75rem}
  .section-icon{width:32px;height:32px;background:#c8a84b22;border:1px solid #c8a84b55;display:flex;align-items:center;justify-content:center;font-size:1rem}
  .section-title{font-family:'Oswald',sans-serif;font-size:1rem;font-weight:600;color:#c8a84b;letter-spacing:2px;text-transform:uppercase}
  .posts{display:flex;flex-direction:column;gap:2px}
  .post{background:#0f0f14;border:1px solid #1e1e28;padding:1rem 1.25rem;display:grid;grid-template-columns:1fr auto;gap:1rem;align-items:center;cursor:pointer;transition:border-color .2s,background .2s}
  .post:hover{background:#13131a;border-color:#c8a84b55}
  .post.pinned{border-left:3px solid #c8a84b}
  .post-left{display:flex;align-items:center;gap:1rem}
  .post-icon{width:40px;height:40px;background:#1a1a22;border:1px solid #2a2a35;display:flex;align-items:center;justify-content:center;font-size:1.2rem;flex-shrink:0}
  .post-title{font-family:'Rajdhani',sans-serif;font-weight:600;font-size:1rem;color:#e0e0e0;margin-bottom:.2rem}
  .post-meta{font-size:.78rem;color:#555;letter-spacing:.5px}
  .post-meta span{color:#777}
  .post-badge{font-family:'Share Tech Mono',monospace;font-size:.7rem;background:#c8a84b22;color:#c8a84b;border:1px solid #c8a84b44;padding:2px 8px;text-transform:uppercase;letter-spacing:1px}
  .post-badge.new{background:#1a3a2a;color:#4caf82;border-color:#4caf8244}
  .post-stats{text-align:right}
  .post-dl{font-family:'Share Tech Mono',monospace;font-size:1rem;color:#c8a84b;font-weight:600}
  .post-dl-label{font-size:.7rem;color:#555;letter-spacing:1px;text-transform:uppercase}
  .divider{height:1px;background:#2a2a35;margin:1.5rem 0}
  .featured{background:#0d0d12;border:1px solid #c8a84b33;padding:1.5rem;margin-bottom:2rem;display:grid;grid-template-columns:1fr 1fr;gap:1rem}
  .featured-title{font-family:'Oswald',sans-serif;font-size:.8rem;color:#c8a84b;letter-spacing:2px;text-transform:uppercase;margin-bottom:1rem;grid-column:1/-1;border-bottom:1px solid #1e1e28;padding-bottom:.5rem}
  .stat-card{background:#0a0a0d;border:1px solid #1e1e28;padding:.75rem 1rem;text-align:center}
  .stat-num{font-family:'Share Tech Mono',monospace;font-size:1.5rem;color:#c8a84b}
  .stat-label{font-size:.75rem;color:#555;text-transform:uppercase;letter-spacing:1px}
  .tag{display:inline-block;font-size:.7rem;background:#1a1a22;border:1px solid #2a2a35;color:#777;padding:2px 8px;margin-right:4px;margin-top:4px;letter-spacing:.5px}
  .upload-btn{background:#c8a84b;color:#0a0a0c;font-family:'Oswald',sans-serif;font-weight:600;letter-spacing:2px;text-transform:uppercase;border:none;padding:.5rem 1.5rem;cursor:pointer;font-size:.85rem;transition:background .2s}
  .upload-btn:hover{background:#dfc06a}
  footer{border-top:1px solid #1e1e28;margin-top:3rem;padding:1rem 2rem;text-align:center;font-size:.75rem;color:#444;letter-spacing:1px;text-transform:uppercase}
</style>
</head>
<body>

<header>
  <div class="header-inner">
    <div class="logo">SA<span>:</span>MP <span style="color:#666">|</span> SCRIPTS</div>
    <nav class="nav">
      <a href="#">Главная</a>
      <a href="#" style="color:#c8a84b">Скрипты</a>
      <a href="#">Гайды</a>
      <a href="#">О нас</a>
    </nav>
  </div>
</header>

<div class="main">
  <div class="page-title">Библиотека скриптов</div>
  <div class="page-sub">MoonLoader Lua — всё для SA-MP</div>

  <div class="featured">
    <div class="featured-title">📊 Статистика форума</div>
    <div class="stat-card"><div class="stat-num">48</div><div class="stat-label">Скриптов</div></div>
    <div class="stat-card"><div class="stat-num">1.2K</div><div class="stat-label">Загрузок</div></div>
    <div class="stat-card"><div class="stat-num">312</div><div class="stat-label">Участников</div></div>
    <div class="stat-card"><div class="stat-num">17</div><div class="stat-label">Новых за неделю</div></div>
  </div>

  <div class="section">
    <div class="section-header">
      <div class="section-icon">⭐</div>
      <div class="section-title">Популярные скрипты</div>
    </div>
    <div class="posts">
      <div class="post pinned">
        <div class="post-left">
          <div class="post-icon">📱</div>
          <div class="post-info">
            <div class="post-title">/me при звонке — авто РП действие</div>
            <div class="post-meta">Автор: <span>LuaDev_RU</span> · TrinityRP · MoonLoader 0.26+</div>
            <div style="margin-top:6px"><span class="tag">roleplay</span><span class="tag">phone</span><span class="tag">automation</span></div>
          </div>
        </div>
        <div class="post-stats">
          <div class="post-dl">247</div>
          <div class="post-dl-label">загрузок</div>
          <div style="margin-top:6px"><span class="post-badge">pinned</span></div>
        </div>
      </div>

      <div class="post">
        <div class="post-left">
          <div class="post-icon">🎯</div>
          <div class="post-info">
            <div class="post-title">HUD — здоровье, броня, деньги на экране</div>
            <div class="post-meta">Автор: <span>moonscript</span> · Все серверы · MoonLoader 0.25+</div>
            <div style="margin-top:6px"><span class="tag">hud</span><span class="tag">visual</span><span class="tag">stats</span></div>
          </div>
        </div>
        <div class="post-stats">
          <div class="post-dl">189</div>
          <div class="post-dl-label">загрузок</div>
          <div style="margin-top:6px"><span class="post-badge new">new</span></div>
        </div>
      </div>

      <div class="post">
        <div class="post-left">
          <div class="post-icon">💬</div>
          <div class="post-info">
            <div class="post-title">Автоответ в личку — /sms автоматический</div>
            <div class="post-meta">Автор: <span>SampCoder</span> · TrinityRP / Arizona · MoonLoader 0.26+</div>
            <div style="margin-top:6px"><span class="tag">chat</span><span class="tag">sms</span><span class="tag">auto</span></div>
          </div>
        </div>
        <div class="post-stats">
          <div class="post-dl">134</div>
          <div class="post-dl-label">загрузок</div>
        </div>
      </div>
    </div>
  </div>

  <div class="divider"></div>

  <div class="section">
    <div class="section-header">
      <div class="section-icon">🆕</div>
      <div class="section-title">Новые добавления</div>
    </div>
    <div class="posts">
      <div class="post">
        <div class="post-left">
          <div class="post-icon">🚗</div>
          <div class="post-info">
            <div class="post-title">Спидометр — скорость авто в реальном времени</div>
            <div class="post-meta">Автор: <span>v8_scripts</span> · 2 дня назад</div>
            <div style="margin-top:6px"><span class="tag">vehicle</span><span class="tag">speedometer</span></div>
          </div>
        </div>
        <div class="post-stats">
          <div class="post-dl">41</div>
          <div class="post-dl-label">загрузок</div>
          <div style="margin-top:6px"><span class="post-badge new">new</span></div>
        </div>
      </div>

      <div class="post">
        <div class="post-left">
          <div class="post-icon">🔔</div>
          <div class="post-info">
            <div class="post-title">Уведомления — всплывающие алерты в углу экрана</div>
            <div class="post-meta">Автор: <span>notifylua</span> · 5 дней назад</div>
            <div style="margin-top:6px"><span class="tag">ui</span><span class="tag">notifications</span></div>
          </div>
        </div>
        <div class="post-stats">
          <div class="post-dl">28</div>
          <div class="post-dl-label">загрузок</div>
          <div style="margin-top:6px"><span class="post-badge new">new</span></div>
        </div>
      </div>

      <div class="post">
        <div class="post-left">
          <div class="post-icon">🗺️</div>
          <div class="post-info">
            <div class="post-title">Кастомная миникарта — метки игроков рядом</div>
            <div class="post-meta">Автор: <span>mapdev_sa</span> · 1 неделю назад</div>
            <div style="margin-top:6px"><span class="tag">map</span><span class="tag">players</span><span class="tag">visual</span></div>
          </div>
        </div>
        <div class="post-stats">
          <div class="post-dl">76</div>
          <div class="post-dl-label">загрузок</div>
        </div>
      </div>
    </div>
  </div>

  <div style="margin-top:2rem;display:flex;align-items:center;justify-content:space-between">
    <div style="font-size:.8rem;color:#555;letter-spacing:1px">Хочешь добавить свой скрипт?</div>
    <button class="upload-btn">+ Загрузить скрипт</button>
  </div>
</div>

<footer>SA:MP Scripts Forum · MoonLoader Community · 2025</footer>
</body>
</html>
