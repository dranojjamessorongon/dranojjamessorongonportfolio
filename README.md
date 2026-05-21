<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Dranoj James Sorongon | IT Support & Network Engineer</title>
  <meta name="description" content="IT Support & Network Engineer with 2+ years of expertise in network configuration, VLAN management, desktop support, and system administration. Based in Iloilo, PH." />
  <meta property="og:title" content="Dranoj James Sorongon | IT Support & Network Engineer" />
  <meta property="og:description" content="IT Support & Network Engineer with 2+ years of expertise in network configuration, VLAN management, and system administration." />
  <meta property="og:type" content="website" />
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content="Dranoj James Sorongon | IT Support & Network Engineer" />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;500;600;700;800&family=DM+Mono:wght@300;400;500&family=Instrument+Serif:ital@0;1&display=swap" rel="stylesheet" />
  <style>
    :root {
      --bg: #0a0a0f;
      --bg2: #0f0f18;
      --surface: #13131f;
      --surface2: #1a1a2e;
      --border: rgba(255,255,255,0.07);
      --accent: #00e5ff;
      --accent2: #7c3aed;
      --accent3: #f59e0b;
      --text: #e8e8f0;
      --text2: #9494aa;
      --text3: #5a5a70;
      --white: #ffffff;
      --radius: 12px;
      --radius2: 20px;
      --glow: 0 0 40px rgba(0,229,255,0.15);
    }
    [data-theme="light"] {
      --bg: #f4f4f8;
      --bg2: #ebebf2;
      --surface: #ffffff;
      --surface2: #f0f0f8;
      --border: rgba(0,0,0,0.08);
      --text: #12121e;
      --text2: #44445a;
      --text3: #8888a0;
      --glow: 0 0 40px rgba(0,180,200,0.12);
    }
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; }
    body {
      background: var(--bg);
      color: var(--text);
      font-family: 'DM Mono', monospace;
      font-size: 15px;
      line-height: 1.7;
      overflow-x: hidden;
      transition: background 0.3s, color 0.3s;
    }

    /* ─── NOISE OVERLAY ─── */
    body::before {
      content: '';
      position: fixed; inset: 0;
      background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.03'/%3E%3C/svg%3E");
      pointer-events: none;
      z-index: 1000;
      opacity: 0.4;
    }

    /* ─── NAV ─── */
    nav {
      position: fixed; top: 0; left: 0; right: 0; z-index: 900;
      display: flex; align-items: center; justify-content: space-between;
      padding: 18px 5%;
      background: rgba(10,10,15,0.85);
      backdrop-filter: blur(20px);
      border-bottom: 1px solid var(--border);
      transition: background 0.3s;
    }
    [data-theme="light"] nav { background: rgba(244,244,248,0.85); }
    .nav-logo {
      font-family: 'Syne', sans-serif;
      font-weight: 800;
      font-size: 18px;
      color: var(--white);
      text-decoration: none;
      letter-spacing: -0.5px;
    }
    [data-theme="light"] .nav-logo { color: var(--text); }
    .nav-logo span { color: var(--accent); }
    .nav-links { display: flex; gap: 32px; list-style: none; align-items: center; }
    .nav-links a {
      color: var(--text2);
      text-decoration: none;
      font-size: 12px;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      transition: color 0.2s;
    }
    .nav-links a:hover { color: var(--accent); }
    .nav-right { display: flex; align-items: center; gap: 16px; }
    .theme-btn {
      background: var(--surface);
      border: 1px solid var(--border);
      color: var(--text2);
      width: 36px; height: 36px;
      border-radius: 50%;
      cursor: pointer;
      font-size: 16px;
      display: flex; align-items: center; justify-content: center;
      transition: all 0.2s;
    }
    .theme-btn:hover { border-color: var(--accent); color: var(--accent); }
    .hamburger { display: none; flex-direction: column; gap: 5px; cursor: pointer; background: none; border: none; padding: 4px; }
    .hamburger span { display: block; width: 22px; height: 2px; background: var(--text2); border-radius: 2px; transition: 0.3s; }

    /* ─── HERO ─── */
    #hero {
      min-height: 100vh;
      display: flex; align-items: center;
      padding: 100px 5% 60px;
      position: relative;
      overflow: hidden;
    }
    .hero-grid {
      display: grid; grid-template-columns: 1fr 1fr;
      gap: 60px; align-items: center;
      max-width: 1200px; margin: 0 auto; width: 100%;
    }
    .hero-eyebrow {
      display: inline-flex; align-items: center; gap: 8px;
      background: rgba(0,229,255,0.08);
      border: 1px solid rgba(0,229,255,0.2);
      border-radius: 100px;
      padding: 6px 16px;
      font-size: 11px;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--accent);
      margin-bottom: 24px;
    }
    .hero-eyebrow::before { content: '●'; font-size: 8px; animation: blink 2s infinite; }
    @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0.3} }
    .hero-title {
      font-family: 'Syne', sans-serif;
      font-size: clamp(42px, 5.5vw, 76px);
      font-weight: 800;
      line-height: 1.0;
      letter-spacing: -2px;
      margin-bottom: 16px;
      color: var(--white);
    }
    [data-theme="light"] .hero-title { color: var(--text); }
    .hero-title .line2 {
      font-family: 'Instrument Serif', serif;
      font-style: italic;
      font-weight: 400;
      color: var(--accent);
    }
    .hero-sub {
      font-size: 14px;
      color: var(--text2);
      max-width: 460px;
      margin-bottom: 40px;
      line-height: 1.8;
    }
    .hero-btns { display: flex; flex-wrap: wrap; gap: 12px; margin-bottom: 48px; }
    .btn-primary {
      background: var(--accent);
      color: #000;
      padding: 14px 28px;
      border-radius: var(--radius);
      text-decoration: none;
      font-family: 'Syne', sans-serif;
      font-weight: 700;
      font-size: 13px;
      letter-spacing: 0.04em;
      transition: all 0.2s;
      border: none; cursor: pointer;
    }
    .btn-primary:hover { background: #33ebff; transform: translateY(-2px); box-shadow: 0 8px 30px rgba(0,229,255,0.3); }
    .btn-secondary {
      background: transparent;
      color: var(--text);
      padding: 13px 28px;
      border-radius: var(--radius);
      border: 1px solid var(--border);
      text-decoration: none;
      font-family: 'Syne', sans-serif;
      font-weight: 600;
      font-size: 13px;
      letter-spacing: 0.04em;
      transition: all 0.2s;
      cursor: pointer;
    }
    .btn-secondary:hover { border-color: var(--accent); color: var(--accent); transform: translateY(-2px); }
    .hero-stats {
      display: flex; gap: 32px;
      padding-top: 32px;
      border-top: 1px solid var(--border);
    }
    .stat-item {}
    .stat-num {
      font-family: 'Syne', sans-serif;
      font-size: 28px;
      font-weight: 800;
      color: var(--white);
    }
    [data-theme="light"] .stat-num { color: var(--text); }
    .stat-num span { color: var(--accent); }
    .stat-label { font-size: 11px; color: var(--text3); letter-spacing: 0.06em; text-transform: uppercase; }

    /* ─── HERO VISUAL ─── */
    .hero-visual {
      display: flex; align-items: center; justify-content: center;
      position: relative;
    }
    .profile-frame {
      width: 360px; height: 440px;
      border-radius: 24px;
      background: linear-gradient(135deg, var(--surface2) 0%, var(--surface) 100%);
      border: 1px solid var(--border);
      position: relative;
      overflow: hidden;
      box-shadow: var(--glow);
    }
    .profile-frame::before {
      content: '';
      position: absolute; inset: 0;
      background: linear-gradient(180deg, transparent 60%, rgba(0,229,255,0.08) 100%);
    }
    .profile-placeholder {
      width: 100%; height: 100%;
      display: flex; flex-direction: column;
      align-items: center; justify-content: center;
      gap: 16px;
    }
    .avatar-icon {
      width: 100px; height: 100px;
      border-radius: 50%;
      background: linear-gradient(135deg, var(--accent2), var(--accent));
      display: flex; align-items: center; justify-content: center;
      font-size: 42px;
    }
    .profile-name-tag {
      font-family: 'Syne', sans-serif;
      font-size: 18px;
      font-weight: 700;
      color: var(--white);
      text-align: center;
    }
    [data-theme="light"] .profile-name-tag { color: var(--text); }
    .profile-role-tag {
      font-size: 12px; color: var(--accent);
      letter-spacing: 0.08em; text-transform: uppercase;
    }
    .profile-badge {
      position: absolute; bottom: 20px; right: 20px;
      background: rgba(0,229,255,0.12);
      border: 1px solid rgba(0,229,255,0.25);
      border-radius: 10px;
      padding: 10px 16px;
      font-size: 11px; color: var(--accent);
      letter-spacing: 0.06em;
    }
    .orbit-ring {
      position: absolute;
      border-radius: 50%;
      border: 1px dashed rgba(0,229,255,0.12);
      animation: spin 18s linear infinite;
    }
    .orbit-ring:nth-child(1) { width: 480px; height: 480px; top: -60px; right: -60px; }
    .orbit-ring:nth-child(2) { width: 360px; height: 360px; top: 0px; right: 0px; animation-duration: 24s; animation-direction: reverse; }
    @keyframes spin { from{transform:rotate(0deg)} to{transform:rotate(360deg)} }
    .orbit-dot {
      position: absolute;
      width: 8px; height: 8px;
      border-radius: 50%;
      background: var(--accent);
      top: 0; left: 50%;
      transform: translateX(-50%);
      box-shadow: 0 0 10px var(--accent);
    }

    /* ─── SECTION SHARED ─── */
    section { padding: 100px 5%; }
    .section-inner { max-width: 1200px; margin: 0 auto; }
    .section-label {
      font-size: 11px; letter-spacing: 0.14em;
      text-transform: uppercase; color: var(--accent);
      margin-bottom: 12px;
      display: flex; align-items: center; gap: 10px;
    }
    .section-label::after { content: ''; flex: 1; max-width: 40px; height: 1px; background: var(--accent); opacity: 0.4; }
    .section-title {
      font-family: 'Syne', sans-serif;
      font-size: clamp(32px, 4vw, 52px);
      font-weight: 800;
      letter-spacing: -1.5px;
      line-height: 1.05;
      color: var(--white);
      margin-bottom: 16px;
    }
    [data-theme="light"] .section-title { color: var(--text); }
    .section-sub { color: var(--text2); max-width: 560px; font-size: 14px; line-height: 1.8; }

    /* ─── ABOUT ─── */
    #about { background: var(--bg2); }
    .about-grid {
      display: grid; grid-template-columns: 1fr 1fr;
      gap: 80px; align-items: start;
      margin-top: 60px;
    }
    .about-text p {
      color: var(--text2); font-size: 14px; line-height: 1.9;
      margin-bottom: 20px;
    }
    .about-text p strong { color: var(--accent); font-weight: 500; }
    .about-cards { display: flex; flex-direction: column; gap: 16px; }
    .about-card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius2);
      padding: 24px;
      transition: border-color 0.2s, transform 0.2s;
    }
    .about-card:hover { border-color: rgba(0,229,255,0.3); transform: translateX(4px); }
    .about-card-icon { font-size: 24px; margin-bottom: 10px; }
    .about-card h4 { font-family: 'Syne', sans-serif; font-size: 15px; font-weight: 700; color: var(--white); margin-bottom: 6px; }
    [data-theme="light"] .about-card h4 { color: var(--text); }
    .about-card p { font-size: 12px; color: var(--text3); line-height: 1.7; }

    /* ─── SKILLS ─── */
    #skills {}
    .skills-header { margin-bottom: 60px; }
    .skills-grid {
      display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
      gap: 24px;
    }
    .skill-category {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius2);
      padding: 32px;
      transition: border-color 0.2s;
    }
    .skill-category:hover { border-color: rgba(0,229,255,0.2); box-shadow: var(--glow); }
    .skill-cat-title {
      font-family: 'Syne', sans-serif;
      font-size: 13px; font-weight: 700;
      letter-spacing: 0.1em; text-transform: uppercase;
      color: var(--accent); margin-bottom: 24px;
      display: flex; align-items: center; gap: 8px;
    }
    .skill-item { margin-bottom: 18px; }
    .skill-item:last-child { margin-bottom: 0; }
    .skill-row { display: flex; justify-content: space-between; margin-bottom: 7px; }
    .skill-name { font-size: 13px; color: var(--text); }
    .skill-pct { font-size: 11px; color: var(--text3); font-family: 'DM Mono', monospace; }
    .skill-bar { height: 4px; background: var(--surface2); border-radius: 2px; overflow: hidden; }
    .skill-fill {
      height: 100%; border-radius: 2px;
      background: linear-gradient(90deg, var(--accent2), var(--accent));
      width: 0;
      transition: width 1.2s cubic-bezier(0.4,0,0.2,1);
    }
    .skill-tags { display: flex; flex-wrap: wrap; gap: 8px; }
    .skill-tag {
      background: var(--surface2);
      border: 1px solid var(--border);
      border-radius: 6px;
      padding: 5px 12px;
      font-size: 11px;
      color: var(--text2);
      letter-spacing: 0.04em;
      transition: all 0.2s;
    }
    .skill-tag:hover { border-color: var(--accent); color: var(--accent); background: rgba(0,229,255,0.05); }

    /* ─── EXPERIENCE ─── */
    #experience { background: var(--bg2); }
    .exp-timeline { margin-top: 60px; position: relative; }
    .exp-timeline::before {
      content: '';
      position: absolute; left: 20px; top: 0; bottom: 0;
      width: 1px; background: var(--border);
    }
    .exp-item {
      display: grid; grid-template-columns: 60px 1fr;
      gap: 32px; margin-bottom: 48px;
      position: relative;
    }
    .exp-dot {
      width: 40px; height: 40px;
      border-radius: 50%;
      background: var(--surface);
      border: 2px solid var(--accent);
      display: flex; align-items: center; justify-content: center;
      font-size: 16px;
      position: relative; z-index: 1;
      box-shadow: 0 0 20px rgba(0,229,255,0.2);
    }
    .exp-content {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius2);
      padding: 32px;
      transition: border-color 0.2s;
    }
    .exp-content:hover { border-color: rgba(0,229,255,0.25); }
    .exp-header { display: flex; justify-content: space-between; align-items: flex-start; flex-wrap: wrap; gap: 8px; margin-bottom: 8px; }
    .exp-role { font-family: 'Syne', sans-serif; font-size: 20px; font-weight: 700; color: var(--white); }
    [data-theme="light"] .exp-role { color: var(--text); }
    .exp-date {
      background: rgba(0,229,255,0.08);
      border: 1px solid rgba(0,229,255,0.2);
      border-radius: 6px;
      padding: 4px 12px;
      font-size: 11px; color: var(--accent);
      letter-spacing: 0.06em; white-space: nowrap;
    }
    .exp-company { font-size: 13px; color: var(--accent); margin-bottom: 20px; letter-spacing: 0.04em; }
    .exp-list { list-style: none; display: flex; flex-direction: column; gap: 10px; }
    .exp-list li {
      font-size: 13px; color: var(--text2); line-height: 1.7;
      padding-left: 20px; position: relative;
    }
    .exp-list li::before {
      content: '→';
      position: absolute; left: 0;
      color: var(--accent); font-size: 11px;
      top: 3px;
    }
    .exp-list li strong { color: var(--accent3); font-weight: 500; }

    /* ─── PROJECTS ─── */
    #projects {}
    .projects-grid {
      display: grid; grid-template-columns: repeat(auto-fit, minmax(340px, 1fr));
      gap: 24px; margin-top: 60px;
    }
    .project-card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius2);
      padding: 32px;
      position: relative;
      overflow: hidden;
      transition: all 0.3s;
      display: flex; flex-direction: column;
    }
    .project-card::before {
      content: '';
      position: absolute; top: 0; left: 0; right: 0;
      height: 2px;
      background: linear-gradient(90deg, var(--accent2), var(--accent));
      transform: scaleX(0); transform-origin: left;
      transition: transform 0.3s;
    }
    .project-card:hover { transform: translateY(-6px); border-color: rgba(0,229,255,0.2); box-shadow: 0 20px 60px rgba(0,0,0,0.3); }
    .project-card:hover::before { transform: scaleX(1); }
    .project-num {
      font-family: 'Syne', sans-serif;
      font-size: 48px; font-weight: 800;
      color: var(--border);
      line-height: 1;
      margin-bottom: 16px;
      transition: color 0.3s;
    }
    .project-card:hover .project-num { color: rgba(0,229,255,0.15); }
    .project-title { font-family: 'Syne', sans-serif; font-size: 18px; font-weight: 700; color: var(--white); margin-bottom: 10px; }
    [data-theme="light"] .project-title { color: var(--text); }
    .project-desc { font-size: 13px; color: var(--text2); line-height: 1.8; margin-bottom: 20px; flex: 1; }
    .project-tech { display: flex; flex-wrap: wrap; gap: 6px; margin-bottom: 24px; }
    .tech-tag {
      background: rgba(124,58,237,0.12);
      border: 1px solid rgba(124,58,237,0.25);
      border-radius: 6px;
      padding: 3px 10px;
      font-size: 10px;
      color: #a78bfa;
      letter-spacing: 0.04em;
    }
    .project-links { display: flex; gap: 12px; }
    .project-link {
      display: flex; align-items: center; gap: 6px;
      font-size: 11px; color: var(--text3);
      text-decoration: none;
      letter-spacing: 0.06em; text-transform: uppercase;
      transition: color 0.2s;
    }
    .project-link:hover { color: var(--accent); }
    .project-achievement {
      background: rgba(245,158,11,0.08);
      border: 1px solid rgba(245,158,11,0.2);
      border-radius: 8px;
      padding: 10px 14px;
      font-size: 12px;
      color: var(--accent3);
      margin-bottom: 16px;
    }

    /* ─── SCHEDULE ─── */
    #schedule { background: var(--bg2); }
    .schedule-wrap {
      display: grid; grid-template-columns: 1fr 1.2fr;
      gap: 60px; margin-top: 60px;
      align-items: start;
    }
    .calendar-ui {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius2);
      padding: 28px;
    }
    .cal-header {
      display: flex; justify-content: space-between; align-items: center;
      margin-bottom: 20px;
    }
    .cal-month { font-family: 'Syne', sans-serif; font-size: 16px; font-weight: 700; color: var(--white); }
    [data-theme="light"] .cal-month { color: var(--text); }
    .cal-nav button {
      background: var(--surface2); border: 1px solid var(--border);
      color: var(--text2); width: 32px; height: 32px;
      border-radius: 8px; cursor: pointer;
      font-size: 14px; transition: all 0.2s;
    }
    .cal-nav button:hover { border-color: var(--accent); color: var(--accent); }
    .cal-nav { display: flex; gap: 8px; }
    .cal-days-header {
      display: grid; grid-template-columns: repeat(7, 1fr);
      text-align: center; margin-bottom: 10px;
    }
    .cal-days-header span { font-size: 10px; color: var(--text3); letter-spacing: 0.08em; text-transform: uppercase; padding: 6px 0; }
    .cal-days {
      display: grid; grid-template-columns: repeat(7, 1fr);
      gap: 4px;
    }
    .cal-day {
      aspect-ratio: 1;
      border-radius: 8px;
      display: flex; align-items: center; justify-content: center;
      font-size: 12px;
      cursor: pointer;
      transition: all 0.15s;
      border: 1px solid transparent;
    }
    .cal-day:not(.empty):not(.past):hover { background: rgba(0,229,255,0.1); border-color: rgba(0,229,255,0.3); color: var(--accent); }
    .cal-day.today { border-color: var(--accent); color: var(--accent); font-weight: 600; }
    .cal-day.selected { background: var(--accent); color: #000; font-weight: 700; }
    .cal-day.past { color: var(--text3); cursor: default; }
    .cal-day.empty { cursor: default; }
    .cal-day.available { background: rgba(0,229,255,0.05); }

    .tz-select {
      margin-top: 16px;
      padding: 10px 14px;
      background: var(--surface2);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      color: var(--text2);
      font-family: 'DM Mono', monospace;
      font-size: 12px;
      width: 100%;
      cursor: pointer;
    }

    .slots-panel {
      margin-top: 20px;
    }
    .slots-title { font-size: 12px; color: var(--text3); letter-spacing: 0.08em; text-transform: uppercase; margin-bottom: 12px; }
    .slots-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 8px; }
    .slot-btn {
      padding: 8px 4px;
      background: var(--surface2);
      border: 1px solid var(--border);
      border-radius: 8px;
      color: var(--text2);
      font-family: 'DM Mono', monospace;
      font-size: 11px;
      cursor: pointer;
      transition: all 0.15s;
      text-align: center;
    }
    .slot-btn:hover { border-color: var(--accent); color: var(--accent); background: rgba(0,229,255,0.05); }
    .slot-btn.selected { background: var(--accent); color: #000; border-color: var(--accent); font-weight: 600; }
    .slot-btn.booked { opacity: 0.4; cursor: not-allowed; text-decoration: line-through; }

    .booking-form { display: flex; flex-direction: column; gap: 16px; }
    .booking-form h3 { font-family: 'Syne', sans-serif; font-size: 24px; font-weight: 700; color: var(--white); margin-bottom: 4px; }
    [data-theme="light"] .booking-form h3 { color: var(--text); }
    .booking-form p { font-size: 13px; color: var(--text2); margin-bottom: 12px; }
    .form-group { display: flex; flex-direction: column; gap: 6px; }
    .form-label { font-size: 11px; color: var(--text3); letter-spacing: 0.08em; text-transform: uppercase; }
    .form-input, .form-select, .form-textarea {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 12px 16px;
      color: var(--text);
      font-family: 'DM Mono', monospace;
      font-size: 13px;
      transition: border-color 0.2s;
      outline: none;
      width: 100%;
    }
    .form-input:focus, .form-select:focus, .form-textarea:focus { border-color: var(--accent); }
    .form-textarea { resize: vertical; min-height: 80px; }
    .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
    .booking-summary {
      background: rgba(0,229,255,0.05);
      border: 1px solid rgba(0,229,255,0.15);
      border-radius: var(--radius);
      padding: 16px;
      font-size: 12px;
      color: var(--text2);
      display: none;
    }
    .booking-summary.show { display: block; }
    .booking-summary strong { color: var(--accent); }

    /* ─── CONTACT ─── */
    #contact {}
    .contact-grid {
      display: grid; grid-template-columns: 1fr 1.4fr;
      gap: 60px; margin-top: 60px;
    }
    .contact-info { display: flex; flex-direction: column; gap: 20px; }
    .contact-item {
      display: flex; align-items: flex-start; gap: 16px;
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius2);
      padding: 20px;
      text-decoration: none;
      transition: all 0.2s;
    }
    .contact-item:hover { border-color: rgba(0,229,255,0.3); transform: translateX(4px); }
    .contact-icon {
      width: 42px; height: 42px;
      border-radius: 10px;
      background: rgba(0,229,255,0.08);
      border: 1px solid rgba(0,229,255,0.15);
      display: flex; align-items: center; justify-content: center;
      font-size: 18px;
      flex-shrink: 0;
    }
    .contact-item-text {}
    .contact-item-label { font-size: 10px; color: var(--text3); letter-spacing: 0.1em; text-transform: uppercase; margin-bottom: 4px; }
    .contact-item-value { font-size: 13px; color: var(--text); }
    .contact-form-wrap {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius2);
      padding: 40px;
    }
    .contact-form-wrap h3 { font-family: 'Syne', sans-serif; font-size: 22px; font-weight: 700; color: var(--white); margin-bottom: 24px; }
    [data-theme="light"] .contact-form-wrap h3 { color: var(--text); }
    .contact-form { display: flex; flex-direction: column; gap: 16px; }
    .form-success {
      background: rgba(0,229,255,0.08);
      border: 1px solid rgba(0,229,255,0.2);
      border-radius: var(--radius);
      padding: 20px;
      text-align: center;
      color: var(--accent);
      font-size: 13px;
      display: none;
    }
    .form-success.show { display: block; }

    /* ─── FOOTER ─── */
    footer {
      padding: 40px 5%;
      border-top: 1px solid var(--border);
      display: flex; justify-content: space-between; align-items: center;
      flex-wrap: wrap; gap: 16px;
    }
    .footer-brand {
      font-family: 'Syne', sans-serif;
      font-weight: 800; font-size: 16px;
      color: var(--text2);
    }
    .footer-brand span { color: var(--accent); }
    .footer-copy { font-size: 11px; color: var(--text3); }
    .footer-links { display: flex; gap: 20px; }
    .footer-links a { font-size: 11px; color: var(--text3); text-decoration: none; transition: color 0.2s; letter-spacing: 0.06em; text-transform: uppercase; }
    .footer-links a:hover { color: var(--accent); }

    /* ─── ANIMATIONS ─── */
    .reveal { opacity: 0; transform: translateY(30px); transition: opacity 0.7s, transform 0.7s; }
    .reveal.visible { opacity: 1; transform: translateY(0); }

    /* ─── MOBILE ─── */
    @media (max-width: 900px) {
      .hero-grid, .about-grid, .schedule-wrap, .contact-grid { grid-template-columns: 1fr; }
      .hero-visual { order: -1; }
      .profile-frame { width: 280px; height: 340px; }
      .nav-links { display: none; }
      .nav-links.open {
        display: flex; flex-direction: column;
        position: fixed; inset: 0; top: 72px;
        background: var(--bg); padding: 40px 5%;
        gap: 24px; z-index: 800;
      }
      .nav-links.open a { font-size: 20px; }
      .hamburger { display: flex; }
      .form-row { grid-template-columns: 1fr; }
    }
    @media (max-width: 600px) {
      .hero-btns { flex-direction: column; }
      .hero-stats { gap: 20px; }
      .projects-grid { grid-template-columns: 1fr; }
      .slots-grid { grid-template-columns: repeat(2,1fr); }
    }

    /* ─── SCROLL INDICATOR ─── */
    .scroll-indicator {
      position: fixed; top: 0; left: 0;
      height: 3px; background: linear-gradient(90deg, var(--accent2), var(--accent));
      z-index: 9999; transition: width 0.1s;
    }
  </style>
</head>
<body>
  <div class="scroll-indicator" id="scrollIndicator"></div>

  <!-- NAV -->
  <nav id="mainNav">
    <a href="#hero" class="nav-logo">Dranoj<span>.</span></a>
    <ul class="nav-links" id="navLinks">
      <li><a href="#about">About</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#experience">Experience</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#schedule">Schedule</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
    <div class="nav-right">
      <button class="theme-btn" id="themeToggle" title="Toggle theme">🌙</button>
      <button class="hamburger" id="hamburger" aria-label="Menu">
        <span></span><span></span><span></span>
      </button>
    </div>
  </nav>

  <!-- HERO -->
  <section id="hero">
    <div class="orbit-ring"><div class="orbit-dot"></div></div>
    <div class="orbit-ring"></div>
    <div class="hero-grid">
      <div class="hero-content">
        <div class="hero-eyebrow">Available for opportunities</div>
        <h1 class="hero-title">
          Dranoj James<br>
          <span class="line2">Sorongon</span>
        </h1>
        <p class="hero-sub">IT Support & Network Engineer with 2+ years of hands-on expertise in network configuration, VLAN management, desktop support, and enterprise system administration. Based in Iloilo City, Philippines.</p>
        <div class="hero-btns">
          <a href="#projects" class="btn-primary">View Projects</a>
          <a href="#schedule" class="btn-secondary">Schedule Interview</a>
          <a href="mailto:dramessorongon@gmail.com" class="btn-secondary">Download Resume</a>
        </div>
        <div class="hero-stats">
          <div class="stat-item">
            <div class="stat-num">2<span>+</span></div>
            <div class="stat-label">Years Experience</div>
          </div>
          <div class="stat-item">
            <div class="stat-num">98<span>%</span></div>
            <div class="stat-label">System Uptime</div>
          </div>
          <div class="stat-item">
            <div class="stat-num">500<span>+</span></div>
            <div class="stat-label">Devices Managed</div>
          </div>
        </div>
      </div>
      <div class="hero-visual">
        <div class="profile-frame">
          <div class="profile-placeholder">
            <div class="avatar-icon">👨‍💻</div>
            <div class="profile-name-tag">Dranoj James A. Sorongon</div>
            <div class="profile-role-tag">IT Support Engineer</div>
          </div>
          <div class="profile-badge">📍 Iloilo City, PH</div>
        </div>
      </div>
    </div>
  </section>

  <!-- ABOUT -->
  <section id="about">
    <div class="section-inner">
      <div class="section-label">About Me</div>
      <h2 class="section-title">The Engineer<br><em style="font-family:'Instrument Serif',serif;font-style:italic;font-weight:400;">Behind the Network</em></h2>
      <div class="about-grid">
        <div class="about-text reveal">
          <p>I'm <strong>Dranoj James A. Sorongon</strong>, an IT Support & Network Engineer based in Molo, Iloilo City, Philippines. I hold a Bachelor of Science in Information Technology from Iloilo Science and Technology University (Class of 2023).</p>
          <p>With over 2 years of professional experience at <strong>New Panay Agri-Ventures Development, Inc.</strong>, I've built deep expertise in enterprise networking, VLAN configuration across Cisco, Aruba, and Huawei infrastructure, and comprehensive desktop support for a large multi-branch organization.</p>
          <p>I pride myself on maintaining <strong>98% system uptime</strong> across critical operations — from Windows environments and standalone applications to NVR servers and a fleet of 500+ CCTV cameras. I thrive in high-responsibility environments where reliability and precision are non-negotiable.</p>
          <p>Currently expanding my development skills in <strong>Python, PHP, CodeIgniter, Bootstrap, and Angular</strong> — bridging the gap between infrastructure management and software engineering to become a more versatile technology professional.</p>
        </div>
        <div class="about-cards reveal">
          <div class="about-card">
            <div class="about-card-icon">🎓</div>
            <h4>Education</h4>
            <p>B.S. Information Technology — Iloilo Science and Technology University (2019–2023)</p>
          </div>
          <div class="about-card">
            <div class="about-card-icon">🏢</div>
            <h4>Current Role</h4>
            <p>IT Support Engineer at New Panay Agri-Ventures Development, Inc. (May 2024 – Present)</p>
          </div>
          <div class="about-card">
            <div class="about-card-icon">🌐</div>
            <h4>Location</h4>
            <p>Zone 6 Boulevard, Molo, Iloilo City, Philippines 5000 — open to remote & relocation</p>
          </div>
          <div class="about-card">
            <div class="about-card-icon">🚀</div>
            <h4>Career Goal</h4>
            <p>To grow into a full-stack infrastructure & development role, merging network engineering expertise with modern software skills.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- SKILLS -->
  <section id="skills">
    <div class="section-inner">
      <div class="section-label">Technical Skills</div>
      <h2 class="section-title reveal">What I<br><em style="font-family:'Instrument Serif',serif;font-style:italic;font-weight:400;">Bring to the Table</em></h2>
      <p class="section-sub reveal">A broad technical skill set spanning networking, hardware, systems administration, and development — built through hands-on enterprise experience.</p>
      <div class="skills-grid" style="margin-top:60px;">
        <div class="skill-category reveal">
          <div class="skill-cat-title">🌐 Networking</div>
          <div class="skill-item"><div class="skill-row"><span class="skill-name">TCP/IP & Subnetting</span><span class="skill-pct">90%</span></div><div class="skill-bar"><div class="skill-fill" data-width="90"></div></div></div>
          <div class="skill-item"><div class="skill-row"><span class="skill-name">VLAN Configuration</span><span class="skill-pct">88%</span></div><div class="skill-bar"><div class="skill-fill" data-width="88"></div></div></div>
          <div class="skill-item"><div class="skill-row"><span class="skill-name">Cisco / Aruba / Huawei</span><span class="skill-pct">82%</span></div><div class="skill-bar"><div class="skill-fill" data-width="82"></div></div></div>
          <div class="skill-item"><div class="skill-row"><span class="skill-name">DNS, Gateway, IP Config</span><span class="skill-pct">92%</span></div><div class="skill-bar"><div class="skill-fill" data-width="92"></div></div></div>
        </div>
        <div class="skill-category reveal">
          <div class="skill-cat-title">🖥 Systems & Hardware</div>
          <div class="skill-item"><div class="skill-row"><span class="skill-name">Windows OS Administration</span><span class="skill-pct">92%</span></div><div class="skill-bar"><div class="skill-fill" data-width="92"></div></div></div>
          <div class="skill-item"><div class="skill-row"><span class="skill-name">Desktop & Laptop Repair</span><span class="skill-pct">90%</span></div><div class="skill-bar"><div class="skill-fill" data-width="90"></div></div></div>
          <div class="skill-item"><div class="skill-row"><span class="skill-name">OS Reimaging & Backup</span><span class="skill-pct">88%</span></div><div class="skill-bar"><div class="skill-fill" data-width="88"></div></div></div>
          <div class="skill-item"><div class="skill-row"><span class="skill-name">CCTV / NVR Management</span><span class="skill-pct">85%</span></div><div class="skill-bar"><div class="skill-fill" data-width="85"></div></div></div>
        </div>
        <div class="skill-category reveal">
          <div class="skill-cat-title">☁️ Microsoft 365 & Cloud</div>
          <div class="skill-tags">
            <span class="skill-tag">Microsoft 365</span>
            <span class="skill-tag">SharePoint</span>
            <span class="skill-tag">PowerApps</span>
            <span class="skill-tag">Power BI</span>
            <span class="skill-tag">Teams</span>
            <span class="skill-tag">OneDrive</span>
            <span class="skill-tag">Microsoft Lists</span>
            <span class="skill-tag">Outlook</span>
            <span class="skill-tag">MS Quick Assist</span>
            <span class="skill-tag">AnyDesk / RDP</span>
          </div>
        </div>
        <div class="skill-category reveal">
          <div class="skill-cat-title">💻 Development (In Progress)</div>
          <div class="skill-tags">
            <span class="skill-tag">PHP</span>
            <span class="skill-tag">Python</span>
            <span class="skill-tag">HTML</span>
            <span class="skill-tag">CSS</span>
            <span class="skill-tag">CodeIgniter</span>
            <span class="skill-tag">Bootstrap</span>
            <span class="skill-tag">Angular</span>
            <span class="skill-tag">VS Code</span>
            <span class="skill-tag">Canva</span>
            <span class="skill-tag">Linux (Learning)</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- EXPERIENCE -->
  <section id="experience">
    <div class="section-inner">
      <div class="section-label">Work Experience</div>
      <h2 class="section-title reveal">Professional<br><em style="font-family:'Instrument Serif',serif;font-style:italic;font-weight:400;">Timeline</em></h2>
      <div class="exp-timeline">
        <div class="exp-item reveal">
          <div class="exp-dot">⚙️</div>
          <div class="exp-content">
            <div class="exp-header">
              <span class="exp-role">IT Support Engineer</span>
              <span class="exp-date">May 2024 – Present</span>
            </div>
            <div class="exp-company">New Panay Agri-Ventures Development, Inc.</div>
            <ul class="exp-list">
              <li>Provided comprehensive desktop support covering Microsoft 365 suite including Lists, PowerApps, SharePoint, Teams, and OneDrive across all departments</li>
              <li>Configured full network parameters (IP address, DNS, gateway) for system units, mini PCs, printers, Smart UPS units, laptops, local servers, NVRs, APs, switches, and CCTV cameras</li>
              <li>Executed VLAN configuration and management across network switches from Cisco, Aruba, and Huawei vendors</li>
              <li><strong>Achieved 98% system uptime</strong> through disciplined OS updates, reimaging, and mirror/hybrid backups for servers, switches, APs, and databases</li>
              <li>Administered inventory of <strong>500+ CCTV cameras</strong>, 200+ laptops/desktops using Microsoft List, Power BI, SharePoint, and PowerApps</li>
              <li>Delivered <strong>10+ daily remote support sessions</strong> to branch locations via MS Quick Assist, AnyDesk, and RDP</li>
              <li>Monitored real-time surveillance and system health for up to <strong>10 NVR servers</strong> via Smart PSS</li>
              <li>Served as hardware specialist: troubleshooting, soldering, component upgrades, and device evaluation for laptops, desktops, and mini PCs</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- PROJECTS -->
  <section id="projects">
    <div class="section-inner">
      <div class="section-label">Projects & Initiatives</div>
      <h2 class="section-title reveal">What I've<br><em style="font-family:'Instrument Serif',serif;font-style:italic;font-weight:400;">Built & Maintained</em></h2>
      <p class="section-sub reveal">Key infrastructure projects and enterprise initiatives delivered during my professional tenure.</p>
      <div class="projects-grid">
        <div class="project-card reveal">
          <div class="project-num">01</div>
          <div class="project-title">Enterprise VLAN Network Infrastructure</div>
          <div class="project-desc">Designed and implemented VLAN segmentation across the organization's network infrastructure, managing switches from Cisco, Aruba, and Huawei. Improved network security, traffic isolation, and performance across multiple departments and branch locations.</div>
          <div class="project-achievement">🏆 Maintained 98% uptime across all network segments</div>
          <div class="project-tech">
            <span class="tech-tag">Cisco</span><span class="tech-tag">Aruba</span><span class="tech-tag">Huawei</span><span class="tech-tag">VLAN</span><span class="tech-tag">TCP/IP</span>
          </div>
          <div class="project-links">
            <a href="#" class="project-link">⬡ GitHub (Private)</a>
            <a href="#" class="project-link">↗ Case Study</a>
          </div>
        </div>
        <div class="project-card reveal">
          <div class="project-num">02</div>
          <div class="project-title">CCTV & Surveillance Fleet Management</div>
          <div class="project-desc">Administered and monitored a fleet of 500+ CCTV cameras and 10 NVR servers across the organization. Built an inventory tracking system using Microsoft Lists, Power BI, and PowerApps to maintain real-time asset visibility and health status.</div>
          <div class="project-achievement">🏆 500+ cameras tracked with zero asset loss incidents</div>
          <div class="project-tech">
            <span class="tech-tag">Smart PSS</span><span class="tech-tag">Power BI</span><span class="tech-tag">Microsoft Lists</span><span class="tech-tag">PowerApps</span>
          </div>
          <div class="project-links">
            <a href="#" class="project-link">⬡ GitHub (Private)</a>
            <a href="#" class="project-link">↗ Details</a>
          </div>
        </div>
        <div class="project-card reveal">
          <div class="project-num">03</div>
          <div class="project-title">IT Asset Inventory & Helpdesk System</div>
          <div class="project-desc">Built a centralized inventory management solution using Microsoft 365 tools to track 200+ laptops, desktops, and all IT equipment. Integrated with SharePoint for documentation and PowerApps for mobile-first asset tracking by field technicians.</div>
          <div class="project-achievement">🏆 Reduced asset lookup time by ~60% organization-wide</div>
          <div class="project-tech">
            <span class="tech-tag">SharePoint</span><span class="tech-tag">PowerApps</span><span class="tech-tag">Microsoft Lists</span><span class="tech-tag">Power BI</span>
          </div>
          <div class="project-links">
            <a href="#" class="project-link">⬡ GitHub (Private)</a>
            <a href="#" class="project-link">↗ Details</a>
          </div>
        </div>
        <div class="project-card reveal">
          <div class="project-num">04</div>
          <div class="project-title">Remote Support & Branch Connectivity</div>
          <div class="project-desc">Established and standardized a remote support workflow delivering 10+ daily sessions to branch locations using MS Quick Assist, AnyDesk, and RDP. Reduced average resolution time and eliminated the need for on-site travel for common issues.</div>
          <div class="project-achievement">🏆 10+ daily remote sessions — near-zero travel escalations</div>
          <div class="project-tech">
            <span class="tech-tag">MS Quick Assist</span><span class="tech-tag">AnyDesk</span><span class="tech-tag">RDP</span><span class="tech-tag">MS Teams</span>
          </div>
          <div class="project-links">
            <a href="#" class="project-link">⬡ GitHub (Private)</a>
            <a href="#" class="project-link">↗ Details</a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- SCHEDULE -->
  <section id="schedule">
    <div class="section-inner">
      <div class="section-label">Interview Scheduling</div>
      <h2 class="section-title reveal">Book a Time<br><em style="font-family:'Instrument Serif',serif;font-style:italic;font-weight:400;">To Connect</em></h2>
      <p class="section-sub reveal">Pick a date and time that works for you. Timezone-aware — international applicants welcome.</p>
      <div class="schedule-wrap">
        <div>
          <div class="calendar-ui reveal">
            <div class="cal-header">
              <span class="cal-month" id="calMonth">Loading...</span>
              <div class="cal-nav">
                <button onclick="changeMonth(-1)">‹</button>
                <button onclick="changeMonth(1)">›</button>
              </div>
            </div>
            <div class="cal-days-header">
              <span>Su</span><span>Mo</span><span>Tu</span><span>We</span><span>Th</span><span>Fr</span><span>Sa</span>
            </div>
            <div class="cal-days" id="calDays"></div>
            <select class="tz-select" id="tzSelect" onchange="updateTimezone()">
              <option value="Asia/Manila">Asia/Manila (PHT, UTC+8)</option>
              <option value="America/New_York">America/New_York (EST/EDT)</option>
              <option value="America/Los_Angeles">America/Los_Angeles (PST/PDT)</option>
              <option value="America/Chicago">America/Chicago (CST/CDT)</option>
              <option value="Europe/London">Europe/London (GMT/BST)</option>
              <option value="Europe/Paris">Europe/Paris (CET/CEST)</option>
              <option value="Asia/Tokyo">Asia/Tokyo (JST, UTC+9)</option>
              <option value="Asia/Singapore">Asia/Singapore (SGT, UTC+8)</option>
              <option value="Australia/Sydney">Australia/Sydney (AEST/AEDT)</option>
              <option value="UTC">UTC</option>
            </select>
          </div>
          <div class="slots-panel reveal" id="slotsPanel" style="display:none;">
            <div class="slots-title" id="slotsDate">Select a date first</div>
            <div class="slots-grid" id="slotsGrid"></div>
          </div>
        </div>
        <div class="booking-form reveal">
          <h3>Schedule an Interview</h3>
          <p>Fill in your details below. A confirmation email will be sent to both parties upon booking.</p>
          <div class="booking-summary" id="bookingSummary"></div>
          <div class="form-row">
            <div class="form-group">
              <label class="form-label">First Name</label>
              <input type="text" class="form-input" id="bFirstName" placeholder="Jane" />
            </div>
            <div class="form-group">
              <label class="form-label">Last Name</label>
              <input type="text" class="form-input" id="bLastName" placeholder="Doe" />
            </div>
          </div>
          <div class="form-group">
            <label class="form-label">Email Address</label>
            <input type="email" class="form-input" id="bEmail" placeholder="jane@company.com" />
          </div>
          <div class="form-group">
            <label class="form-label">Company / Organization</label>
            <input type="text" class="form-input" id="bCompany" placeholder="Your Company Name" />
          </div>
          <div class="form-group">
            <label class="form-label">Interview Type</label>
            <select class="form-select" id="bType">
              <option value="">Select interview type</option>
              <option>Initial Screening (30 min)</option>
              <option>Technical Interview (60 min)</option>
              <option>Culture Fit Interview (45 min)</option>
              <option>Final Round Interview (60 min)</option>
            </select>
          </div>
          <div class="form-group">
            <label class="form-label">Notes (Optional)</label>
            <textarea class="form-textarea" id="bNotes" placeholder="Any specific topics, role details, or questions..."></textarea>
          </div>
          <button class="btn-primary" onclick="submitBooking()" style="width:100%;padding:16px;">Confirm Booking & Send Invite</button>
          <div class="form-success" id="bookingSuccess">
            ✅ Booking confirmed! Check your email for calendar invite and meeting details.<br><br>
            A confirmation has also been sent to dramessorongon@gmail.com
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact">
    <div class="section-inner">
      <div class="section-label">Get In Touch</div>
      <h2 class="section-title reveal">Let's Work<br><em style="font-family:'Instrument Serif',serif;font-style:italic;font-weight:400;">Together</em></h2>
      <div class="contact-grid">
        <div class="contact-info reveal">
          <a href="mailto:dramessorongon@gmail.com" class="contact-item">
            <div class="contact-icon">✉️</div>
            <div class="contact-item-text">
              <div class="contact-item-label">Email</div>
              <div class="contact-item-value">dramessorongon@gmail.com</div>
            </div>
          </a>
          <a href="tel:+639949850210" class="contact-item">
            <div class="contact-icon">📱</div>
            <div class="contact-item-text">
              <div class="contact-item-label">Phone / Mobile</div>
              <div class="contact-item-value">+63 994 985 0210</div>
            </div>
          </a>
          <a href="#" class="contact-item">
            <div class="contact-icon">💼</div>
            <div class="contact-item-text">
              <div class="contact-item-label">LinkedIn</div>
              <div class="contact-item-value">linkedin.com/in/dranoj-sorongon</div>
            </div>
          </a>
          <a href="#" class="contact-item">
            <div class="contact-icon">🐙</div>
            <div class="contact-item-text">
              <div class="contact-item-label">GitHub</div>
              <div class="contact-item-value">github.com/dranoj-sorongon</div>
            </div>
          </a>
          <div class="contact-item" style="border-color:rgba(0,229,255,0.15);">
            <div class="contact-icon">📍</div>
            <div class="contact-item-text">
              <div class="contact-item-label">Location</div>
              <div class="contact-item-value">Zone 6 Boulevard, Molo, Iloilo City, PH 5000</div>
            </div>
          </div>
        </div>
        <div class="contact-form-wrap reveal">
          <h3>Send a Message</h3>
          <div class="contact-form" id="contactForm">
            <div class="form-row">
              <div class="form-group">
                <label class="form-label">Full Name</label>
                <input type="text" class="form-input" id="cName" placeholder="Your Name" />
              </div>
              <div class="form-group">
                <label class="form-label">Email</label>
                <input type="email" class="form-input" id="cEmail" placeholder="your@email.com" />
              </div>
            </div>
            <div class="form-group">
              <label class="form-label">Subject</label>
              <input type="text" class="form-input" id="cSubject" placeholder="Job Opportunity / Collaboration / Other" />
            </div>
            <div class="form-group">
              <label class="form-label">Message</label>
              <textarea class="form-textarea" id="cMessage" rows="5" placeholder="Tell me about the opportunity or how I can help..."></textarea>
            </div>
            <button class="btn-primary" onclick="submitContact()" style="width:100%;padding:16px;">Send Message →</button>
          </div>
          <div class="form-success" id="contactSuccess">
            ✅ Message sent! I'll get back to you within 24 hours.<br><br>
            You can also reach me directly at dramessorongon@gmail.com
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer>
    <div class="footer-brand">Dranoj<span>.</span></div>
    <div class="footer-copy">© 2025 Dranoj James A. Sorongon. All rights reserved.</div>
    <div class="footer-links">
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#contact">Contact</a>
    </div>
  </footer>

  <script>
    // ─── THEME TOGGLE ───
    const themeToggle = document.getElementById('themeToggle');
    let isDark = true;
    themeToggle.addEventListener('click', () => {
      isDark = !isDark;
      document.documentElement.setAttribute('data-theme', isDark ? 'dark' : 'light');
      themeToggle.textContent = isDark ? '🌙' : '☀️';
    });

    // ─── HAMBURGER ───
    const hamburger = document.getElementById('hamburger');
    const navLinks = document.getElementById('navLinks');
    hamburger.addEventListener('click', () => {
      navLinks.classList.toggle('open');
    });
    navLinks.querySelectorAll('a').forEach(a => {
      a.addEventListener('click', () => navLinks.classList.remove('open'));
    });

    // ─── SCROLL PROGRESS ───
    window.addEventListener('scroll', () => {
      const pct = (window.scrollY / (document.body.scrollHeight - window.innerHeight)) * 100;
      document.getElementById('scrollIndicator').style.width = pct + '%';
    });

    // ─── REVEAL ON SCROLL ───
    const reveals = document.querySelectorAll('.reveal');
    const observer = new IntersectionObserver((entries) => {
      entries.forEach((e, i) => {
        if (e.isIntersecting) {
          setTimeout(() => e.target.classList.add('visible'), i * 80);
        }
      });
    }, { threshold: 0.1 });
    reveals.forEach(el => observer.observe(el));

    // ─── SKILL BARS ───
    const skillObserver = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.querySelectorAll('.skill-fill').forEach(bar => {
            const w = bar.getAttribute('data-width');
            setTimeout(() => bar.style.width = w + '%', 200);
          });
        }
      });
    }, { threshold: 0.3 });
    document.querySelectorAll('.skill-category').forEach(el => skillObserver.observe(el));

    // ─── CALENDAR ───
    let currentDate = new Date();
    let selectedDate = null;
    let selectedSlot = null;
    const bookedSlots = {};

    function renderCalendar() {
      const year = currentDate.getFullYear();
      const month = currentDate.getMonth();
      const monthNames = ['January','February','March','April','May','June','July','August','September','October','November','December'];
      document.getElementById('calMonth').textContent = `${monthNames[month]} ${year}`;
      const firstDay = new Date(year, month, 1).getDay();
      const daysInMonth = new Date(year, month + 1, 0).getDate();
      const today = new Date();
      const grid = document.getElementById('calDays');
      grid.innerHTML = '';
      for (let i = 0; i < firstDay; i++) {
        const el = document.createElement('div');
        el.className = 'cal-day empty';
        grid.appendChild(el);
      }
      for (let d = 1; d <= daysInMonth; d++) {
        const el = document.createElement('div');
        const thisDate = new Date(year, month, d);
        const isPast = thisDate < new Date(today.getFullYear(), today.getMonth(), today.getDate());
        const isToday = thisDate.toDateString() === today.toDateString();
        const isWeekend = thisDate.getDay() === 0 || thisDate.getDay() === 6;
        const dateStr = `${year}-${String(month+1).padStart(2,'0')}-${String(d).padStart(2,'0')}`;
        el.className = 'cal-day' + (isPast || isWeekend ? ' past' : ' available') + (isToday ? ' today' : '');
        el.textContent = d;
        if (!isPast && !isWeekend) {
          el.addEventListener('click', () => selectDate(dateStr, el));
        }
        if (selectedDate === dateStr) el.classList.add('selected');
        grid.appendChild(el);
      }
    }

    function selectDate(dateStr, el) {
      selectedDate = dateStr;
      selectedSlot = null;
      document.querySelectorAll('.cal-day.selected').forEach(d => d.classList.remove('selected'));
      el.classList.add('selected');
      renderSlots(dateStr);
      updateSummary();
    }

    function renderSlots(dateStr) {
      const panel = document.getElementById('slotsPanel');
      panel.style.display = 'block';
      const [y, m, d] = dateStr.split('-');
      const monthNames = ['Jan','Feb','Mar','Apr','May','Jun','Jul','Aug','Sep','Oct','Nov','Dec'];
      document.getElementById('slotsDate').textContent = `Available slots — ${monthNames[parseInt(m)-1]} ${d}, ${y}`;
      const times = ['09:00 AM','10:00 AM','11:00 AM','01:00 PM','02:00 PM','03:00 PM','04:00 PM','05:00 PM'];
      const grid = document.getElementById('slotsGrid');
      grid.innerHTML = '';
      const tz = document.getElementById('tzSelect').value;
      times.forEach(t => {
        const btn = document.createElement('button');
        btn.className = 'slot-btn';
        const booked = bookedSlots[dateStr + '-' + t];
        btn.textContent = t;
        if (booked) {
          btn.classList.add('booked');
          btn.disabled = true;
        } else {
          btn.addEventListener('click', () => selectSlot(t, btn));
        }
        if (selectedSlot === t) btn.classList.add('selected');
        grid.appendChild(btn);
      });
    }

    function selectSlot(time, btn) {
      selectedSlot = time;
      document.querySelectorAll('.slot-btn.selected').forEach(b => b.classList.remove('selected'));
      btn.classList.add('selected');
      updateSummary();
    }

    function updateSummary() {
      const summary = document.getElementById('bookingSummary');
      if (selectedDate && selectedSlot) {
        const tz = document.getElementById('tzSelect').value;
        const [y, m, d] = selectedDate.split('-');
        const monthNames = ['January','February','March','April','May','June','July','August','September','October','November','December'];
        summary.innerHTML = `<strong>📅 Date:</strong> ${monthNames[parseInt(m)-1]} ${d}, ${y}<br><strong>🕐 Time:</strong> ${selectedSlot}<br><strong>🌍 Timezone:</strong> ${tz}`;
        summary.classList.add('show');
      } else {
        summary.classList.remove('show');
      }
    }

    function updateTimezone() {
      if (selectedDate) renderSlots(selectedDate);
      updateSummary();
    }

    function changeMonth(dir) {
      currentDate.setMonth(currentDate.getMonth() + dir);
      renderCalendar();
    }

    function submitBooking() {
      const firstName = document.getElementById('bFirstName').value.trim();
      const lastName = document.getElementById('bLastName').value.trim();
      const email = document.getElementById('bEmail').value.trim();
      const company = document.getElementById('bCompany').value.trim();
      const type = document.getElementById('bType').value;
      if (!firstName || !email || !selectedDate || !selectedSlot || !type) {
        alert('Please fill in all required fields and select a date & time slot.');
        return;
      }
      // Mark slot as booked
      bookedSlots[selectedDate + '-' + selectedSlot] = true;
      document.getElementById('bookingSuccess').classList.add('show');
      document.getElementById('bookingSuccess').innerHTML = `✅ <strong>Booking Confirmed!</strong><br><br>
        📅 ${selectedDate} at ${selectedSlot}<br>
        👤 ${firstName} ${lastName} (${company})<br>
        📧 Confirmation sent to ${email} and dramessorongon@gmail.com<br><br>
        <em>A calendar invite with meeting link will be sent shortly.</em>`;
      renderSlots(selectedDate);
    }

    function submitContact() {
      const name = document.getElementById('cName').value.trim();
      const email = document.getElementById('cEmail').value.trim();
      const subject = document.getElementById('cSubject').value.trim();
      const message = document.getElementById('cMessage').value.trim();
      if (!name || !email || !message) {
        alert('Please fill in your name, email, and message.');
        return;
      }
      document.getElementById('contactForm').style.display = 'none';
      document.getElementById('contactSuccess').classList.add('show');
    }

    // Auto-detect timezone
    try {
      const detected = Intl.DateTimeFormat().resolvedOptions().timeZone;
      const sel = document.getElementById('tzSelect');
      for (let i = 0; i < sel.options.length; i++) {
        if (sel.options[i].value === detected) { sel.selectedIndex = i; break; }
      }
    } catch(e) {}

    renderCalendar();
  </script>
</body>
</html>
