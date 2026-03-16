# stablecoinsexplication<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Les Stablecoins — Guide Complet 2025</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700;900&family=DM+Sans:ital,wght@0,300;0,400;0,500;0,600;1,400&family=DM+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
/* ───────────────────────────────────────────────
   RESET & CUSTOM PROPERTIES
─────────────────────────────────────────────── */
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
:root {
  --navy:       #0D1B2A;
  --navy-mid:   #1A3A5C;
  --navy-card:  #132A45;
  --teal:       #0891B2;
  --teal-lt:    #22D3EE;
  --mint:       #02C39A;
  --white:      #FFFFFF;
  --off-white:  #F0F4F8;
  --light-blue: #BAE6FD;
  --gray:       #94A3B8;
  --dark-gray:  #334155;
  --gold:       #F59E0B;
  --orange:     #FB923C;
  --red:        #EF4444;
  --purple:     #9B59B6;
  --ff-display: 'Playfair Display', Georgia, serif;
  --ff-body:    'DM Sans', system-ui, sans-serif;
  --ff-mono:    'DM Mono', monospace;
  --radius:     12px;
  --ease:       cubic-bezier(.4,0,.2,1);
}
html { scroll-behavior: smooth; }
body { font-family: var(--ff-body); background: var(--navy); color: var(--white); line-height: 1.65; overflow-x: hidden; }
::-webkit-scrollbar { width: 5px; }
::-webkit-scrollbar-track { background: var(--navy); }
::-webkit-scrollbar-thumb { background: var(--teal); border-radius: 3px; }

/* ─── NAV ─── */
nav {
  position: fixed; top: 0; left: 0; right: 0; z-index: 200;
  height: 58px; display: flex; align-items: center; justify-content: space-between;
  padding: 0 2.5rem;
  background: rgba(13,27,42,.92); backdrop-filter: blur(18px);
  border-bottom: 1px solid rgba(8,145,178,.22);
}
.nav-logo { font-family: var(--ff-display); font-size: 1.05rem; font-weight: 700; color: var(--teal-lt); text-decoration: none; letter-spacing: .03em; }
.nav-logo span { color: var(--white); }
.nav-links { display: flex; gap: .15rem; list-style: none; }
.nav-links a { display: block; padding: .28rem .6rem; font-size: .7rem; font-weight: 500; color: var(--gray); text-decoration: none; border-radius: 6px; letter-spacing: .04em; transition: .25s var(--ease); }
.nav-links a:hover, .nav-links a.active { color: var(--teal-lt); background: rgba(8,145,178,.12); }
.nav-badge { font-family: var(--ff-mono); font-size: .68rem; color: var(--teal); border: 1px solid rgba(8,145,178,.35); padding: .18rem .6rem; border-radius: 20px; }

/* ─── SECTIONS ─── */
section { padding: 6rem 2.5rem; position: relative; overflow: hidden; }
.container { max-width: 1160px; margin: 0 auto; }
.eyebrow { display: inline-flex; align-items: center; gap: .5rem; font-family: var(--ff-mono); font-size: .68rem; color: var(--teal-lt); letter-spacing: .14em; text-transform: uppercase; margin-bottom: .6rem; }
.eyebrow::before { content:''; display:block; width:20px; height:2px; background:var(--teal); }
.section-title { font-family: var(--ff-display); font-size: clamp(1.9rem, 3.5vw, 2.8rem); font-weight: 700; line-height: 1.1; margin-bottom: .6rem; }
.section-sub { color: var(--gray); max-width: 560px; margin-bottom: 2.8rem; }
.divider { width: 44px; height: 3px; border-radius: 2px; background: linear-gradient(90deg, var(--teal), var(--mint)); margin-bottom: 2rem; }
.bg-light { background: var(--off-white); }
.bg-light .section-title, .bg-light h3, .bg-light h4 { color: var(--navy); }
.bg-light .section-sub, .bg-light p { color: var(--dark-gray); }
.bg-light .eyebrow { color: var(--teal); }
.bg-light .eyebrow::before { background: var(--teal); }

/* ─── HERO ─── */
#hero { min-height: 100vh; display: flex; align-items: center; padding: 100px 2.5rem 5rem; }
.hero-bg { position: absolute; inset: 0; z-index: 0; background: radial-gradient(ellipse 65% 65% at 78% 18%, rgba(8,145,178,.2) 0%, transparent 60%), radial-gradient(ellipse 45% 45% at 18% 78%, rgba(2,195,154,.09) 0%, transparent 55%); }
.hero-grid { position: absolute; inset: 0; z-index: 0; background-image: linear-gradient(rgba(8,145,178,.055) 1px, transparent 1px), linear-gradient(90deg, rgba(8,145,178,.055) 1px, transparent 1px); background-size: 56px 56px; mask-image: radial-gradient(ellipse 85% 85% at 50% 50%, black 20%, transparent 75%); }
.hero-orb { position: absolute; border-radius: 50%; filter: blur(70px); pointer-events: none; z-index: 0; animation: pulse 7s ease-in-out infinite; }
.hero-orb-1 { width:520px;height:520px; background:rgba(8,145,178,.13); right:-80px;top:-80px; }
.hero-orb-2 { width:320px;height:320px; background:rgba(2,195,154,.08); left:8%;bottom:12%; animation-delay:3s; }
@keyframes pulse { 0%,100%{opacity:.8} 50%{opacity:1} }
.hero-inner { position: relative; z-index: 1; max-width: 1160px; margin: 0 auto; width: 100%; display: grid; grid-template-columns: 1.1fr .9fr; gap: 4rem; align-items: center; }
.hero-kicker { display: inline-flex; align-items: center; gap: .55rem; font-family: var(--ff-mono); font-size: .7rem; color: var(--teal-lt); letter-spacing: .14em; text-transform: uppercase; margin-bottom: 1.4rem; }
.hero-kicker::before { content:''; display:block; width:28px; height:2px; background:var(--teal); }
.hero-title { font-family: var(--ff-display); font-size: clamp(3rem, 6.5vw, 5.8rem); font-weight: 900; line-height: 1.02; letter-spacing: -.025em; margin-bottom: 1.5rem; }
.hero-title .hi { color: var(--teal-lt); }
.hero-desc { font-size: 1.08rem; color: var(--light-blue); max-width: 480px; line-height: 1.8; margin-bottom: 2.2rem; }
.hero-btns { display: flex; gap: .85rem; flex-wrap: wrap; }
.btn { display: inline-flex; align-items: center; gap: .45rem; padding: .7rem 1.65rem; border-radius: 8px; font-family: var(--ff-body); font-size: .88rem; font-weight: 600; cursor: pointer; text-decoration: none; transition: .3s var(--ease); border: none; }
.btn-primary { background: var(--teal); color: var(--white); }
.btn-primary:hover { background: var(--teal-lt); transform: translateY(-2px); box-shadow: 0 10px 36px rgba(8,145,178,.38); }
.btn-outline { background: transparent; color: var(--light-blue); border: 1px solid rgba(186,230,253,.22); }
.btn-outline:hover { border-color: var(--teal-lt); color: var(--teal-lt); }
.hero-stats { display: grid; grid-template-columns: 1fr 1fr; gap: .85rem; }
.stat-card { background: rgba(19,42,69,.75); border: 1px solid rgba(8,145,178,.2); border-radius: var(--radius); padding: 1.2rem; backdrop-filter: blur(10px); transition: .3s var(--ease); position: relative; overflow: hidden; }
.stat-card::after { content:''; position:absolute; top:0; left:0; right:0; height:2px; background: linear-gradient(90deg, var(--teal), var(--teal-lt)); transform:scaleX(0); transform-origin:left; transition:.3s var(--ease); }
.stat-card:hover { transform:translateY(-4px); border-color:rgba(8,145,178,.45); }
.stat-card:hover::after { transform:scaleX(1); }
.stat-val { font-family: var(--ff-display); font-size: 2rem; font-weight: 900; color: var(--teal-lt); line-height: 1; margin-bottom: .25rem; }
.stat-lbl { font-size: .75rem; color: var(--gray); }
.scroll-hint { position: absolute; bottom: 2.5rem; left: 50%; transform: translateX(-50%); z-index: 1; display: flex; flex-direction: column; align-items: center; gap: .5rem; font-size: .68rem; color: var(--gray); letter-spacing: .1em; text-transform: uppercase; animation: fadeUp 1s 1.5s both; }
.scroll-hint svg { animation: bounce 2s ease-in-out infinite; }
@keyframes bounce { 0%,100%{transform:translateY(0)} 50%{transform:translateY(6px)} }
@keyframes fadeUp { from{opacity:0;transform:translateX(-50%) translateY(12px)} to{opacity:1;transform:translateX(-50%) translateY(0)} }

/* ─── 01 DÉFINITION ─── */
#definition .def-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 2.5rem; align-items: start; }
.def-box { background: rgba(26,58,92,.55); border: 1px solid rgba(8,145,178,.22); border-radius: var(--radius); padding: 1.8rem; }
.def-box p { color: var(--light-blue); font-size: 1.02rem; line-height: 1.82; }
.pillars { display: flex; flex-direction: column; gap: .85rem; }
.pillar { display: flex; align-items: flex-start; gap: 1rem; background: var(--navy-card); border: 1px solid rgba(8,145,178,.15); border-radius: 10px; padding: 1.1rem; transition: .3s var(--ease); }
.pillar:hover { border-color: var(--teal); transform: translateX(4px); }
.pillar-icon { width: 40px; height: 40px; min-width: 40px; border-radius: 8px; display: flex; align-items: center; justify-content: center; font-size: 1.15rem; }
.pillar h4 { font-size: .88rem; font-weight: 600; color: var(--white); margin-bottom: .2rem; }
.pillar p { font-size: .82rem; color: var(--gray); }

/* ─── 02 TYPES ─── */
#types .types-grid { display: grid; grid-template-columns: repeat(3,1fr); gap: 1.5rem; }
.type-card { background: var(--white); border-radius: var(--radius); overflow: hidden; box-shadow: 0 4px 24px rgba(0,0,0,.08); transition: .3s var(--ease); position: relative; }
.type-card:hover { transform: translateY(-6px); box-shadow: 0 12px 40px rgba(0,0,0,.14); }
.type-accent { position: absolute; top: 0; left: 0; right: 0; height: 3px; }
.type-top { padding: 2rem 1.5rem 1.2rem; display: flex; flex-direction: column; align-items: center; gap: .8rem; text-align: center; }
.type-icon { width: 62px; height: 62px; border-radius: 16px; display: flex; align-items: center; justify-content: center; font-size: 1.6rem; }
.type-card h3 { font-family: var(--ff-display); font-size: 1.1rem; font-weight: 700; color: var(--navy); }
.type-badge { font-size: .68rem; font-weight: 600; letter-spacing: .06em; padding: .22rem .7rem; border-radius: 20px; }
.type-card > p { font-size: .85rem; color: var(--dark-gray); line-height: 1.7; padding: 0 1.4rem; }
.type-examples { font-size: .8rem; font-weight: 600; padding: .6rem 1.4rem; }
.type-proscons { border-top: 1px solid #E2E8F0; padding: .9rem 1.4rem; display: flex; flex-direction: column; gap: .35rem; }
.type-proscons span { font-size: .8rem; display: flex; align-items: center; gap: .4rem; color: var(--dark-gray); }

/* ─── 03 ACTEURS ─── */
.acteurs-list { display: flex; flex-direction: column; gap: .85rem; }
.acteur-row { display: grid; grid-template-columns: 2.8rem 1fr auto 1fr; align-items: center; gap: 1.5rem; background: var(--navy-card); border-radius: var(--radius); padding: 1.1rem 1.5rem; border-left: 3px solid transparent; transition: .3s var(--ease); }
.acteur-row:hover { transform: translateX(5px); }
.acteur-rank { font-family: var(--ff-display); font-size: 1.4rem; font-weight: 900; text-align: center; }
.acteur-info h4 { font-size: .95rem; font-weight: 600; margin-bottom: .2rem; }
.acteur-meta { display: flex; align-items: center; gap: .6rem; flex-wrap: wrap; }
.acteur-type { font-size: .68rem; font-weight: 600; letter-spacing: .05em; padding: .15rem .55rem; border-radius: 20px; }
.acteur-cap { font-size: .78rem; color: var(--gray); }
.acteur-pct { font-family: var(--ff-display); font-size: 2.2rem; font-weight: 900; text-align: right; min-width: 80px; }
.acteur-bar-wrap { display: flex; flex-direction: column; gap: .3rem; }
.acteur-bar-lbl { font-size: .7rem; color: var(--gray); }
.acteur-bar-bg { height: 6px; background: rgba(255,255,255,.08); border-radius: 3px; overflow: hidden; }
.acteur-bar-fill { height: 100%; border-radius: 3px; transition: width 1.2s var(--ease); }
.acteur-source { font-size: .75rem; color: var(--gray); margin-top: 1rem; text-align: right; }

/* ─── 04 USAGES ─── */
#usages .usages-grid { display: grid; grid-template-columns: repeat(3,1fr); gap: 1.4rem; }
.usage-card { background: var(--white); border-radius: var(--radius); padding: 1.5rem; border-left: 3px solid transparent; box-shadow: 0 2px 16px rgba(0,0,0,.06); transition: .3s var(--ease); }
.usage-card:hover { transform: translateY(-4px); box-shadow: 0 10px 36px rgba(0,0,0,.12); }
.usage-icon-wrap { width: 48px; height: 48px; border-radius: 12px; display: flex; align-items: center; justify-content: center; font-size: 1.3rem; margin-bottom: 1rem; }
.usage-card h4 { font-size: .95rem; font-weight: 700; color: var(--navy); margin-bottom: .5rem; }
.usage-card p { font-size: .83rem; color: var(--dark-gray); line-height: 1.7; }

/* ─── 05 RISQUES ─── */
.risques-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 2rem; }
.risques-col h3 { font-size: .78rem; font-weight: 700; letter-spacing: .1em; text-transform: uppercase; margin-bottom: 1.2rem; padding: .6rem 1rem; border-radius: 8px; }
.risques-col.danger h3 { background: rgba(127,29,29,.5); color: #FCA5A5; }
.risques-col.regle  h3 { background: rgba(26,58,92,.8); color: var(--teal-lt); }
.risk-item, .reg-item { display: flex; align-items: flex-start; gap: .9rem; padding: .9rem 1rem; border-radius: 10px; margin-bottom: .7rem; transition: .25s var(--ease); }
.risk-item { background: var(--navy-card); border: 1px solid rgba(239,68,68,.15); }
.reg-item  { background: var(--navy-card); border: 1px solid rgba(8,145,178,.15); }
.risk-item:hover { border-color: rgba(239,68,68,.4); }
.reg-item:hover  { border-color: rgba(8,145,178,.4); }
.ri-icon { font-size: 1.1rem; margin-top: .1rem; flex-shrink:0; }
.ri-text p { font-size: .83rem; color: var(--light-blue); line-height: 1.65; }
.ri-text strong { display: block; font-size: .78rem; color: var(--teal-lt); margin-bottom: .2rem; }

/* ─── 06 ÉVOLUTION ─── */
.timeline-wrap { position: relative; padding: 3rem 0; }
.timeline-line { position: absolute; left: 50%; top: 0; bottom: 0; width: 2px; background: linear-gradient(180deg, transparent, var(--teal) 10%, var(--teal) 90%, transparent); transform: translateX(-50%); }
.timeline-items { display: flex; flex-direction: column; gap: 0; }
.tl-item { display: grid; grid-template-columns: 1fr 60px 1fr; gap: 1rem; align-items: center; margin-bottom: 1.5rem; }
.tl-item.right .tl-content { grid-column: 3; grid-row: 1; }
.tl-item.right .tl-spacer { grid-column: 1; grid-row: 1; }
.tl-dot-wrap { grid-column: 2; display: flex; justify-content: center; z-index: 1; }
.tl-dot { width: 16px; height: 16px; border-radius: 50%; border: 2px solid var(--navy); outline: 3px solid; flex-shrink: 0; }
.tl-content { background: var(--navy-card); border-radius: var(--radius); padding: 1.1rem 1.3rem; border: 1px solid rgba(8,145,178,.15); transition: .3s var(--ease); }
.tl-content:hover { border-color: var(--teal); transform: scale(1.01); }
.tl-year { font-family: var(--ff-display); font-size: 1.15rem; font-weight: 900; margin-bottom: .25rem; }
.tl-name { font-size: .88rem; font-weight: 600; color: var(--white); margin-bottom: .3rem; }
.tl-desc { font-size: .8rem; color: var(--gray); line-height: 1.6; }
.evo-stats { display: grid; grid-template-columns: repeat(4,1fr); gap: 1rem; margin-top: 3rem; }
.evo-stat { text-align: center; padding: 1.2rem; background: var(--navy-card); border: 1px solid rgba(8,145,178,.18); border-radius: var(--radius); }
.evo-stat-val { font-family: var(--ff-display); font-size: 1.8rem; font-weight: 900; color: var(--teal-lt); }
.evo-stat-lbl { font-size: .75rem; color: var(--gray); margin-top: .2rem; }

/* ─── 07 MONDE ─── */
.monde-grid { display: grid; grid-template-columns: 1.2fr 1fr; gap: 2rem; align-items: start; }
.monde-map { background: var(--navy-card); border: 1px solid rgba(8,145,178,.2); border-radius: var(--radius); padding: 1.5rem; }
.monde-map h4 { font-size: .8rem; color: var(--gray); text-transform: uppercase; letter-spacing: .08em; margin-bottom: 1rem; }
.region-row { display: grid; grid-template-columns: 1.4rem 7rem 1fr 2.5rem; gap: .7rem; align-items: center; margin-bottom: .7rem; }
.region-flag { font-size: 1rem; text-align: center; }
.region-name { font-size: .8rem; font-weight: 500; }
.region-track { height: 7px; background: rgba(255,255,255,.07); border-radius: 4px; overflow: hidden; }
.region-fill { height: 100%; border-radius: 4px; transition: width 1.2s var(--ease); }
.region-pct { font-family: var(--ff-mono); font-size: .75rem; color: var(--teal-lt); text-align: right; }
.monde-regions { display: flex; flex-direction: column; gap: .8rem; }
.monde-region-card { background: var(--navy-card); border: 1px solid rgba(8,145,178,.15); border-radius: 10px; padding: 1rem 1.2rem; border-left: 3px solid transparent; transition: .3s var(--ease); }
.monde-region-card:hover { transform: translateX(4px); }
.monde-rc-head { display: flex; justify-content: space-between; align-items: baseline; margin-bottom: .3rem; }
.monde-rc-head h4 { font-size: .88rem; font-weight: 600; }
.monde-rc-head span { font-size: .78rem; font-weight: 700; }
.monde-rc-desc { font-size: .8rem; color: var(--gray); line-height: 1.6; }
.monde-footer { background: var(--navy-mid); border-radius: 10px; padding: .85rem 1.2rem; font-size: .85rem; color: var(--teal-lt); text-align: center; margin-top: 2rem; }

/* ─── 08 MÉCANISMES ─── */
.meca-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 2.5rem; }
.flowchart-wrap { background: var(--navy-card); border: 1px solid rgba(8,145,178,.2); border-radius: var(--radius); overflow: hidden; }
.flowchart-header { background: var(--navy-mid); padding: .6rem 1rem; font-family: var(--ff-mono); font-size: .7rem; color: var(--teal-lt); letter-spacing: .12em; text-align: center; }
.flowchart-cols { display: grid; grid-template-columns: 1fr 1fr; padding: 1rem; gap: 1rem; }
.fc-col-label { font-size: .73rem; font-weight: 700; letter-spacing: .06em; text-align: center; margin-bottom: .75rem; padding: .25rem; border-radius: 4px; }
.fc-col-label.mint   { color: var(--mint);   background: rgba(2,195,154,.1); }
.fc-col-label.redeem { color: var(--orange); background: rgba(251,146,60,.1); }
.fc-nodes { display: flex; flex-direction: column; align-items: center; }
.fc-node { width: 100%; padding: .55rem .7rem; border-radius: 8px; text-align: center; border: 1.5px solid transparent; }
.fc-node h5 { font-size: .82rem; font-weight: 600; color: var(--white); }
.fc-node p { font-size: .72rem; color: var(--light-blue); margin-top: .1rem; }
.fc-arrow { font-size: .8rem; margin: .25rem 0; opacity: .7; }
.fc-node.mint-node   { background: rgba(8,145,178,.15);  border-color: var(--teal); }
.fc-node.mint-end    { background: rgba(2,195,154,.15);  border-color: var(--mint); }
.fc-node.redeem-node { background: rgba(251,146,60,.15); border-color: var(--orange); }
.fc-node.redeem-end  { background: rgba(239,68,68,.15);  border-color: var(--red); }
.fc-node.neutral     { background: rgba(26,58,92,.8);    border-color: rgba(148,163,184,.2); }
.meca-blocks { display: flex; flex-direction: column; gap: 1.2rem; }
.meca-block { background: var(--navy-card); border-radius: var(--radius); padding: 1.3rem; border-left: 3px solid transparent; transition: .3s var(--ease); }
.meca-block:hover { transform: translateX(4px); }
.meca-block-head { display: flex; align-items: center; gap: .7rem; margin-bottom: .75rem; }
.meca-block-head span { font-size: 1.2rem; }
.meca-block-head h4 { font-size: .92rem; font-weight: 700; }
.meca-block p { font-size: .82rem; color: var(--light-blue); line-height: 1.72; }
.meca-block p strong { color: var(--teal-lt); }
.meca-block p em { color: var(--gold); font-style: normal; }
.collat-bar { display: flex; height: 10px; border-radius: 5px; overflow: hidden; margin: .85rem 0 .4rem; gap: 2px; }
.collat-seg { height: 100%; border-radius: 5px; }
.collat-labels { display: flex; justify-content: space-between; font-size: .72rem; }

/* ─── 09 CBDC ─── */
.cbdc-grid { border-radius: var(--radius); overflow: hidden; box-shadow: 0 8px 40px rgba(0,0,0,.15); }
.cbdc-headers { display: grid; grid-template-columns: 1fr 1fr; }
.cbdc-header { padding: 1.1rem 1.5rem; display: flex; align-items: center; gap: .8rem; }
.cbdc-header h3 { font-size: 1rem; font-weight: 700; color: var(--white); }
.cbdc-header p  { font-size: .75rem; opacity: .75; color: var(--white); margin-top: .1rem; }
.cbdc-header.priv { background: var(--teal); }
.cbdc-header.pub  { background: var(--purple); }
.cbdc-row-label { grid-column: 1/-1; display: flex; align-items: center; gap: .5rem; padding: .5rem 1.4rem; background: rgba(0,0,0,.04); border-bottom: 1px solid rgba(0,0,0,.06); font-size: .72rem; font-weight: 700; text-transform: uppercase; letter-spacing: .08em; color: var(--dark-gray); }
.cbdc-row { display: grid; grid-template-columns: 1fr 1fr; }
.cbdc-cell { padding: 1.1rem 1.4rem; border-bottom: 1px solid rgba(0,0,0,.07); }
.cbdc-cell.priv-cell { background: rgba(8,145,178,.05);  border-right: 1px solid rgba(0,0,0,.06); }
.cbdc-cell.pub-cell  { background: rgba(155,89,182,.05); }
.cbdc-cell h5 { font-size: .8rem; font-weight: 700; margin-bottom: .3rem; }
.cbdc-cell p  { font-size: .8rem; color: var(--dark-gray); line-height: 1.65; }
.privacy-slider { margin-top: 2rem; background: var(--navy-card); border-radius: 10px; padding: 1.2rem 1.5rem; }
.slider-title { font-size: .78rem; color: var(--gray); margin-bottom: .8rem; text-align: center; letter-spacing: .06em; text-transform: uppercase; }
.slider-track { height: 12px; border-radius: 6px; position: relative; background: linear-gradient(90deg, var(--teal), #4a7fc1, var(--purple)); }
.slider-labels { display: flex; justify-content: space-between; margin-top: .5rem; font-size: .75rem; }
.slider-labels .l { color: var(--teal-lt); }
.slider-labels .r { color: #cc90e0; }
.slider-marker { position: absolute; top: 50%; transform: translate(-50%,-50%); width: 22px; height: 22px; border-radius: 50%; background: var(--white); display: flex; align-items: center; justify-content: center; font-family: var(--ff-mono); font-size: .5rem; font-weight: 700; box-shadow: 0 2px 8px rgba(0,0,0,.3); }
.slider-marker.sc { left: 18%; color: var(--teal);   border: 2px solid var(--teal); }
.slider-marker.cb { left: 82%; color: var(--purple); border: 2px solid var(--purple); }

/* ─── 10 MARCHÉS ─── */
.marches-kpis { display: grid; grid-template-columns: repeat(4,1fr); gap: 1.2rem; margin-bottom: 2.5rem; }
.mkpi { background: var(--navy-card); border: 1px solid rgba(8,145,178,.18); border-radius: var(--radius); padding: 1.4rem; text-align: center; transition: .3s var(--ease); }
.mkpi:hover { border-color: var(--teal); transform: translateY(-4px); }
.mkpi-val { font-family: var(--ff-display); font-size: 2rem; font-weight: 900; color: var(--teal-lt); margin-bottom: .25rem; }
.mkpi-lbl { font-size: .78rem; color: var(--gray); }
.marches-note { font-size: .82rem; color: var(--gray); text-align: center; }

/* ─── 11 AVENIR ─── */
.avenir-grid { display: grid; grid-template-columns: 1fr .85fr; gap: 3rem; align-items: start; }
.avenir-items { display: flex; flex-direction: column; gap: 1rem; }
.avenir-item { display: flex; align-items: flex-start; gap: 1.1rem; background: var(--navy-card); border-radius: var(--radius); padding: 1.2rem; border: 1px solid rgba(8,145,178,.15); transition: .3s var(--ease); }
.avenir-item:hover { border-color: var(--teal); transform: translateX(5px); }
.avenir-icon { width: 44px; height: 44px; min-width: 44px; border-radius: 10px; display: flex; align-items: center; justify-content: center; font-size: 1.2rem; }
.avenir-item h4 { font-size: .92rem; font-weight: 700; color: var(--white); margin-bottom: .3rem; }
.avenir-item p  { font-size: .82rem; color: var(--light-blue); line-height: 1.7; }
.avenir-keypoints { background: rgba(8,145,178,.08); border: 1px solid rgba(8,145,178,.25); border-radius: var(--radius); padding: 1.8rem; position: sticky; top: 80px; }
.avenir-keypoints h3 { font-family: var(--ff-display); font-size: 1.3rem; font-weight: 700; color: var(--teal-lt); margin-bottom: 1.2rem; }
.kp-list { display: flex; flex-direction: column; gap: .75rem; }
.kp-item { display: flex; align-items: center; gap: .7rem; padding: .6rem .8rem; background: rgba(13,27,42,.5); border-radius: 8px; font-size: .88rem; font-weight: 500; }
.kp-item::before { content:'▸'; color: var(--teal-lt); font-size: .8rem; flex-shrink:0; }

/* ─── FOOTER ─── */
footer { background: var(--navy-mid); border-top: 1px solid rgba(8,145,178,.2); padding: 2rem 2.5rem; text-align: center; font-size: .8rem; color: var(--gray); }
footer strong { color: var(--teal-lt); }

/* ─── ANIMATIONS ─── */
.reveal { opacity: 0; transform: translateY(28px); transition: opacity .7s var(--ease), transform .7s var(--ease); }
.reveal.visible { opacity: 1; transform: none; }
.reveal-delay-1 { transition-delay: .1s; }
.reveal-delay-2 { transition-delay: .2s; }
.reveal-delay-3 { transition-delay: .3s; }

/* ─── RESPONSIVE ─── */
@media (max-width: 900px) {
  .hero-inner, #definition .def-grid, .meca-grid, .monde-grid, .avenir-grid { grid-template-columns: 1fr; }
  .hero-stats { grid-template-columns: 1fr 1fr; }
  #types .types-grid, #usages .usages-grid { grid-template-columns: 1fr 1fr; }
  .marches-kpis, .evo-stats { grid-template-columns: 1fr 1fr; }
  .acteur-row { grid-template-columns: 2rem 1fr auto; }
  .acteur-bar-wrap { display: none; }
  .tl-item { grid-template-columns: 1fr 40px 1fr; }
  .nav-links { display: none; }
  .risques-grid { grid-template-columns: 1fr; }
}
@media (max-width: 600px) {
  section { padding: 4rem 1.2rem; }
  nav { padding: 0 1.2rem; }
  #types .types-grid, #usages .usages-grid, .hero-stats { grid-template-columns: 1fr; }
  .evo-stats, .marches-kpis { grid-template-columns: 1fr 1fr; }
  .cbdc-row { grid-template-columns: 1fr; }
}
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <a href="#hero" class="nav-logo">Stable<span>coins</span></a>
  <ul class="nav-links">
    <li><a href="#definition">Définition</a></li>
    <li><a href="#types">Types</a></li>
    <li><a href="#acteurs">Acteurs</a></li>
    <li><a href="#usages">Usages</a></li>
    <li><a href="#risques">Risques</a></li>
    <li><a href="#evolution">Évolution</a></li>
    <li><a href="#monde">Monde</a></li>
    <li><a href="#mecanismes">Mécanismes</a></li>
    <li><a href="#cbdc">vs CBDC</a></li>
    <li><a href="#avenir">Avenir</a></li>
  </ul>
  <span class="nav-badge">2025</span>
</nav>

<!-- HERO -->
<section id="hero">
  <div class="hero-bg"></div>
  <div class="hero-grid"></div>
  <div class="hero-orb hero-orb-1"></div>
  <div class="hero-orb hero-orb-2"></div>
  <div class="hero-inner">
    <div>
      <p class="hero-kicker">Finance &amp; Crypto · Guide Complet</p>
      <h1 class="hero-title">Les<br><span class="hi">Stable</span>coins</h1>
      <p class="hero-desc">Comprendre les actifs numériques à valeur stable et leur rôle central dans l'écosystème crypto mondial — de la définition aux perspectives 2025.</p>
      <div class="hero-btns">
        <a href="#definition" class="btn btn-primary">Explorer le guide ↓</a>
        <a href="#mecanismes" class="btn btn-outline">Deep Dive →</a>
      </div>
    </div>
    <div class="hero-stats">
      <div class="stat-card"><div class="stat-val">$165B+</div><div class="stat-lbl">Capitalisation mondiale 2024</div></div>
      <div class="stat-card"><div class="stat-val">×300</div><div class="stat-lbl">Croissance depuis 2020</div></div>
      <div class="stat-card"><div class="stat-val">200+</div><div class="stat-lbl">Stablecoins actifs</div></div>
      <div class="stat-card"><div class="stat-val">$10T+</div><div class="stat-lbl">Volume annuel (2023)</div></div>
    </div>
  </div>
  <div class="scroll-hint">
    <svg width="16" height="24" viewBox="0 0 16 24" fill="none"><rect x="1" y="1" width="14" height="22" rx="7" stroke="#94A3B8" stroke-width="1.5"/><rect x="6.5" y="5" width="3" height="6" rx="1.5" fill="#94A3B8"/></svg>
    Défiler
  </div>
</section>

<!-- 01 DÉFINITION -->
<section id="definition" class="bg-light">
  <div class="container">
    <p class="eyebrow">01 — Définition</p>
    <h2 class="section-title">Qu'est-ce qu'un Stablecoin ?</h2>
    <p class="section-sub">Définition et principes fondamentaux</p>
    <div class="divider"></div>
    <div class="def-grid reveal">
      <div class="def-box">
        <p>Un <strong>stablecoin</strong> est une cryptomonnaie dont la valeur est ancrée à un actif de référence stable — généralement une devise fiat (USD, EUR) ou une matière première (or). Contrairement au Bitcoin ou à l'Ethereum, il maintient une parité fixe, éliminant la volatilité inhérente aux cryptoactifs.</p>
        <br>
        <p>Cette stabilité le rend particulièrement adapté aux transactions quotidiennes, aux contrats intelligents et à la finance décentralisée (DeFi), où une unité de compte prévisible est indispensable.</p>
        <br>
        <p style="background:rgba(8,145,178,.1);border:1px solid rgba(8,145,178,.25);border-radius:8px;padding:1rem;font-size:.88rem;">
          📌 <strong>Capitalisation mondiale :</strong> +$165 milliards (2024)
        </p>
      </div>
      <div class="pillars">
        <div class="pillar reveal reveal-delay-1">
          <div class="pillar-icon" style="background:rgba(8,145,178,.12);">⚖️</div>
          <div><h4>Stabilité</h4><p>Valeur arrimée à un actif de référence. Le prix oscille typiquement entre $0,999 et $1,001.</p></div>
        </div>
        <div class="pillar reveal reveal-delay-2">
          <div class="pillar-icon" style="background:rgba(2,195,154,.12);">🔄</div>
          <div><h4>Liquidité</h4><p>Échangeable 24h/24, 7j/7 sans friction sur toutes les plateformes crypto et DeFi mondiales.</p></div>
        </div>
        <div class="pillar reveal reveal-delay-3">
          <div class="pillar-icon" style="background:rgba(245,158,11,.12);">🔍</div>
          <div><h4>Transparence</h4><p>Réserves auditables selon le type — de l'audit trimestriel à la preuve on-chain temps réel.</p></div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- 02 TYPES -->
<section id="types">
  <div class="container">
    <p class="eyebrow">02 — Classification</p>
    <h2 class="section-title">Les Types de Stablecoins</h2>
    <p class="section-sub">Trois approches très différentes pour maintenir la stabilité de la valeur.</p>
    <div class="divider"></div>
    <div class="types-grid">
      <div class="type-card reveal">
        <div class="type-accent" style="background:var(--teal);"></div>
        <div class="type-top">
          <div class="type-icon" style="background:rgba(8,145,178,.1);">🏦</div>
          <h3>Collatéralisés Fiat</h3>
          <span class="type-badge" style="background:rgba(2,195,154,.12);color:var(--mint);">Le plus répandu</span>
        </div>
        <p>Chaque token est adossé à une réserve en devises (USD, EUR) détenue par un dépositaire central agréé.</p>
        <p class="type-examples" style="color:var(--teal);">Exemples : USDT · USDC · BUSD</p>
        <div class="type-proscons">
          <span><span style="color:var(--mint);">✓</span> Simplicité, stabilité maximale</span>
          <span><span style="color:var(--red);">✗</span> Centralisation, risque contrepartie</span>
        </div>
      </div>
      <div class="type-card reveal reveal-delay-2">
        <div class="type-accent" style="background:var(--gold);"></div>
        <div class="type-top">
          <div class="type-icon" style="background:rgba(245,158,11,.1);">🪙</div>
          <h3>Collatéralisés Crypto</h3>
          <span class="type-badge" style="background:rgba(245,158,11,.12);color:var(--gold);">Décentralisé</span>
        </div>
        <p>Sur-collatéralisés par des actifs crypto (ETH, BTC). Gérés par des contrats intelligents on-chain.</p>
        <p class="type-examples" style="color:var(--gold);">Exemples : DAI · sUSD · FRAX</p>
        <div class="type-proscons">
          <span><span style="color:var(--mint);">✓</span> Décentralisation, transparence totale</span>
          <span><span style="color:var(--red);">✗</span> Volatilité du collatéral, liquidations</span>
        </div>
      </div>
      <div class="type-card reveal reveal-delay-3">
        <div class="type-accent" style="background:var(--orange);"></div>
        <div class="type-top">
          <div class="type-icon" style="background:rgba(251,146,60,.1);">📉</div>
          <h3>Algorithmiques</h3>
          <span class="type-badge" style="background:rgba(239,68,68,.12);color:var(--red);">Haute risque</span>
        </div>
        <p>Stabilité maintenue par des mécanismes algorithmiques ajustant l'offre automatiquement, sans collatéral physique.</p>
        <p class="type-examples" style="color:var(--orange);">Exemples : UST (Terra) · AMPL · FRAX v2</p>
        <div class="type-proscons">
          <span><span style="color:var(--mint);">✓</span> Décentralisation totale</span>
          <span><span style="color:var(--red);">✗</span> Instabilité prouvée (Terra 2022)</span>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- 03 ACTEURS -->
<section id="acteurs">
  <div class="container">
    <p class="eyebrow">03 — Acteurs</p>
    <h2 class="section-title">Les Stablecoins Dominants</h2>
    <p class="section-sub">Classement par capitalisation boursière — données CoinGecko 2024.</p>
    <div class="divider"></div>
    <div class="acteurs-list">
      <div class="acteur-row reveal" style="border-left-color:var(--mint);">
        <div class="acteur-rank" style="color:var(--mint);">1</div>
        <div class="acteur-info"><h4>Tether (USDT)</h4><div class="acteur-meta"><span class="acteur-type" style="background:rgba(2,195,154,.12);color:var(--mint);">Fiat</span><span class="acteur-cap">Cap. mkt : $95B+</span></div></div>
        <div class="acteur-pct" style="color:var(--mint);">66%</div>
        <div class="acteur-bar-wrap"><span class="acteur-bar-lbl">Part de marché</span><div class="acteur-bar-bg"><div class="acteur-bar-fill" style="width:66%;background:var(--mint);"></div></div></div>
      </div>
      <div class="acteur-row reveal reveal-delay-1" style="border-left-color:var(--teal-lt);">
        <div class="acteur-rank" style="color:var(--teal-lt);">2</div>
        <div class="acteur-info"><h4>USD Coin (USDC)</h4><div class="acteur-meta"><span class="acteur-type" style="background:rgba(34,211,238,.1);color:var(--teal-lt);">Fiat</span><span class="acteur-cap">Cap. mkt : $32B+</span></div></div>
        <div class="acteur-pct" style="color:var(--teal-lt);">20%</div>
        <div class="acteur-bar-wrap"><span class="acteur-bar-lbl">Part de marché</span><div class="acteur-bar-bg"><div class="acteur-bar-fill" style="width:20%;background:var(--teal-lt);"></div></div></div>
      </div>
      <div class="acteur-row reveal reveal-delay-2" style="border-left-color:var(--gold);">
        <div class="acteur-rank" style="color:var(--gold);">3</div>
        <div class="acteur-info"><h4>DAI</h4><div class="acteur-meta"><span class="acteur-type" style="background:rgba(245,158,11,.12);color:var(--gold);">Crypto</span><span class="acteur-cap">Cap. mkt : $8B+</span></div></div>
        <div class="acteur-pct" style="color:var(--gold);">5%</div>
        <div class="acteur-bar-wrap"><span class="acteur-bar-lbl">Part de marché</span><div class="acteur-bar-bg"><div class="acteur-bar-fill" style="width:5%;background:var(--gold);"></div></div></div>
      </div>
      <div class="acteur-row reveal reveal-delay-3" style="border-left-color:var(--orange);">
        <div class="acteur-rank" style="color:var(--orange);">4</div>
        <div class="acteur-info"><h4>FRAX</h4><div class="acteur-meta"><span class="acteur-type" style="background:rgba(251,146,60,.12);color:var(--orange);">Hybride</span><span class="acteur-cap">Cap. mkt : $4B+</span></div></div>
        <div class="acteur-pct" style="color:var(--orange);">3%</div>
        <div class="acteur-bar-wrap"><span class="acteur-bar-lbl">Part de marché</span><div class="acteur-bar-bg"><div class="acteur-bar-fill" style="width:3%;background:var(--orange);"></div></div></div>
      </div>
    </div>
    <p class="acteur-source reveal">Source : CoinGecko, 2024 · Part de marché par capitalisation boursière</p>
  </div>
</section>

<!-- 04 USAGES -->
<section id="usages" class="bg-light">
  <div class="container">
    <p class="eyebrow">04 — Applications</p>
    <h2 class="section-title">Cas d'Usage</h2>
    <p class="section-sub">Des paiements internationaux à la DeFi, les stablecoins s'imposent comme infrastructure financière mondiale.</p>
    <div class="divider"></div>
    <div class="usages-grid">
      <div class="usage-card reveal" style="border-left-color:var(--teal);">
        <div class="usage-icon-wrap" style="background:rgba(8,145,178,.1);">💸</div>
        <h4>Paiements</h4>
        <p>Transactions internationales rapides et peu coûteuses. Frais quasi nuls vs 3-8% pour les virements SWIFT traditionnels.</p>
      </div>
      <div class="usage-card reveal reveal-delay-1" style="border-left-color:var(--gold);">
        <div class="usage-icon-wrap" style="background:rgba(245,158,11,.1);">📈</div>
        <h4>Finance Décentralisée</h4>
        <p>Prêts, emprunts, yield farming et market making sur les protocoles DeFi (Aave, Compound, Uniswap).</p>
      </div>
      <div class="usage-card reveal reveal-delay-2" style="border-left-color:var(--mint);">
        <div class="usage-icon-wrap" style="background:rgba(2,195,154,.1);">🌍</div>
        <h4>Remittances</h4>
        <p>Envoi d'argent vers les pays émergents sans banque. Révolutionnaire pour les 1,7 milliards de non-bancarisés.</p>
      </div>
      <div class="usage-card reveal" style="border-left-color:var(--orange);">
        <div class="usage-icon-wrap" style="background:rgba(251,146,60,.1);">🛡️</div>
        <h4>Couverture des risques</h4>
        <p>Refuge contre la volatilité crypto. Sécuriser ses gains sans quitter l'écosystème blockchain.</p>
      </div>
      <div class="usage-card reveal reveal-delay-1" style="border-left-color:var(--purple);">
        <div class="usage-icon-wrap" style="background:rgba(155,89,182,.1);">🎮</div>
        <h4>Commerce &amp; NFTs</h4>
        <p>Paiement dans les marketplaces NFT et le Web3. Standard de prix dans les jeux blockchain (GameFi).</p>
      </div>
      <div class="usage-card reveal reveal-delay-2" style="border-left-color:#E74C3C;">
        <div class="usage-icon-wrap" style="background:rgba(231,76,60,.1);">🏛️</div>
        <h4>CBDCs &amp; Institutions</h4>
        <p>Les banques centrales développent leurs propres stablecoins (e€, e-CNY). Adoption institutionnelle en hausse.</p>
      </div>
    </div>
  </div>
</section>

<!-- 05 RISQUES -->
<section id="risques">
  <div class="container">
    <p class="eyebrow">05 — Enjeux</p>
    <h2 class="section-title">Risques &amp; Régulation</h2>
    <p class="section-sub">Comprendre les risques et le cadre réglementaire mondial en évolution rapide.</p>
    <div class="divider"></div>
    <div class="risques-grid reveal">
      <div class="risques-col danger">
        <h3>⚠️ RISQUES PRINCIPAUX</h3>
        <div class="risk-item"><span class="ri-icon">🔴</span><div class="ri-text"><strong>Risque de dépeg</strong><p>Perte de l'ancrage à la valeur de référence. Exemple : TerraUSD -99% en mai 2022.</p></div></div>
        <div class="risk-item"><span class="ri-icon">🔴</span><div class="ri-text"><strong>Risque de contrepartie</strong><p>Insolvabilité du dépositaire des réserves. Le collatéral fiat dépend d'un tiers centralisé.</p></div></div>
        <div class="risk-item"><span class="ri-icon">🔴</span><div class="ri-text"><strong>Risque réglementaire</strong><p>Interdictions ou restrictions gouvernementales susceptibles de paralyser l'émission.</p></div></div>
        <div class="risk-item"><span class="ri-icon">🔴</span><div class="ri-text"><strong>Risque de liquidité</strong><p>Gel ou restriction de rachat en période de stress de marché ou de bank run numérique.</p></div></div>
      </div>
      <div class="risques-col regle">
        <h3>🏛️ CADRE RÉGLEMENTAIRE</h3>
        <div class="reg-item"><span class="ri-icon">🇪🇺</span><div class="ri-text"><strong>Europe</strong><p>MiCA (2024) : premier cadre réglementaire complet pour les stablecoins et crypto-actifs.</p></div></div>
        <div class="reg-item"><span class="ri-icon">🇺🇸</span><div class="ri-text"><strong>États-Unis</strong><p>GENIUS Act en discussion au Congrès. SEC &amp; CFTC en compétition de juridiction.</p></div></div>
        <div class="reg-item"><span class="ri-icon">🌏</span><div class="ri-text"><strong>Asie</strong><p>Hong Kong et Singapour : régimes favorables. Chine : interdiction totale des cryptos.</p></div></div>
        <div class="reg-item"><span class="ri-icon">🌍</span><div class="ri-text"><strong>Émergents</strong><p>Adoption croissante pour protéger contre l'inflation locale (Argentine, Nigeria, Zimbabwe).</p></div></div>
      </div>
    </div>
  </div>
</section>

<!-- 06 ÉVOLUTION -->
<section id="evolution">
  <div class="container">
    <p class="eyebrow">06 — Histoire</p>
    <h2 class="section-title">Évolution des Stablecoins</h2>
    <p class="section-sub">De l'expérimentation à l'institutionnalisation — 10 ans de croissance fulgurante.</p>
    <div class="divider"></div>
    <div class="timeline-wrap">
      <div class="timeline-line"></div>
      <div class="timeline-items">
        <div class="tl-item reveal">
          <div class="tl-content" style="border-color:rgba(148,163,184,.3);"><div class="tl-year" style="color:var(--gray);">2014</div><div class="tl-name">BitUSD &amp; NuBits</div><div class="tl-desc">Premiers stablecoins crypto-collatéralisés. Concept encore expérimental, adoption marginale.</div></div>
          <div class="tl-dot-wrap"><div class="tl-dot" style="background:var(--gray);outline-color:var(--gray);"></div></div>
          <div class="tl-spacer"></div>
        </div>
        <div class="tl-item right reveal">
          <div class="tl-spacer"></div>
          <div class="tl-dot-wrap"><div class="tl-dot" style="background:var(--teal);outline-color:var(--teal);"></div></div>
          <div class="tl-content" style="border-color:var(--teal);"><div class="tl-year" style="color:var(--teal);">2015</div><div class="tl-name">Tether (USDT)</div><div class="tl-desc">Premier stablecoin fiat dominant. Ancré 1:1 au dollar, révolutionne les échanges crypto mondiaux.</div></div>
        </div>
        <div class="tl-item reveal">
          <div class="tl-content" style="border-color:var(--gold);"><div class="tl-year" style="color:var(--gold);">2018</div><div class="tl-name">DAI &amp; MakerDAO</div><div class="tl-desc">Naissance du stablecoin décentralisé. Collatéral crypto, gouvernance DAO, transparent et sans tiers centralisé.</div></div>
          <div class="tl-dot-wrap"><div class="tl-dot" style="background:var(--gold);outline-color:var(--gold);"></div></div>
          <div class="tl-spacer"></div>
        </div>
        <div class="tl-item right reveal">
          <div class="tl-spacer"></div>
          <div class="tl-dot-wrap"><div class="tl-dot" style="background:var(--teal-lt);outline-color:var(--teal-lt);"></div></div>
          <div class="tl-content" style="border-color:var(--teal-lt);"><div class="tl-year" style="color:var(--teal-lt);">2018</div><div class="tl-name">USDC (Circle)</div><div class="tl-desc">USD Coin lancé par Circle &amp; Coinbase. Réserves auditées mensuellement par un cabinet indépendant.</div></div>
        </div>
        <div class="tl-item reveal">
          <div class="tl-content" style="border-color:var(--mint);"><div class="tl-year" style="color:var(--mint);">2020</div><div class="tl-name">Explosion DeFi</div><div class="tl-desc">Boom de la finance décentralisée. Les stablecoins deviennent l'épine dorsale du secteur crypto mondial.</div></div>
          <div class="tl-dot-wrap"><div class="tl-dot" style="background:var(--mint);outline-color:var(--mint);"></div></div>
          <div class="tl-spacer"></div>
        </div>
        <div class="tl-item right reveal">
          <div class="tl-spacer"></div>
          <div class="tl-dot-wrap"><div class="tl-dot" style="background:var(--red);outline-color:var(--red);"></div></div>
          <div class="tl-content" style="border-color:var(--red);"><div class="tl-year" style="color:var(--red);">2022</div><div class="tl-name">Effondrement UST</div><div class="tl-desc">TerraUSD perd son ancrage. -$50 milliards en 72h. Prise de conscience mondiale sur les risques algorithmiques.</div></div>
        </div>
        <div class="tl-item reveal">
          <div class="tl-content" style="border-color:var(--orange);"><div class="tl-year" style="color:var(--orange);">2024</div><div class="tl-name">Règlementation MiCA</div><div class="tl-desc">L'Europe instaure le premier cadre légal complet pour les stablecoins. Adoption institutionnelle en forte hausse.</div></div>
          <div class="tl-dot-wrap"><div class="tl-dot" style="background:var(--orange);outline-color:var(--orange);"></div></div>
          <div class="tl-spacer"></div>
        </div>
      </div>
    </div>
    <div class="evo-stats">
      <div class="evo-stat reveal"><div class="evo-stat-val">$165B+</div><div class="evo-stat-lbl">Capitalisation 2024</div></div>
      <div class="evo-stat reveal reveal-delay-1"><div class="evo-stat-val">×300</div><div class="evo-stat-lbl">Croissance depuis 2020</div></div>
      <div class="evo-stat reveal reveal-delay-2"><div class="evo-stat-val">200+</div><div class="evo-stat-lbl">Stablecoins actifs</div></div>
      <div class="evo-stat reveal reveal-delay-3"><div class="evo-stat-val">$10T+</div><div class="evo-stat-lbl">Volume annuel 2023</div></div>
    </div>
  </div>
</section>

<!-- 07 MONDE -->
<section id="monde" class="bg-light">
  <div class="container">
    <p class="eyebrow">07 — Géographie</p>
    <h2 class="section-title">Utilisation dans le Monde</h2>
    <p class="section-sub">Adoption mondiale et cartographie de l'intensité d'usage par région.</p>
    <div class="divider"></div>
    <div class="monde-grid">
      <div class="monde-map reveal">
        <h4>Intensité d'adoption par région</h4>
        <div class="region-row"><span class="region-flag">🇺🇸</span><span class="region-name" style="color:var(--navy);">Amérique du Nord</span><div class="region-track"><div class="region-fill" style="width:85%;background:var(--teal);"></div></div><span class="region-pct">85%</span></div>
        <div class="region-row"><span class="region-flag">🌏</span><span class="region-name" style="color:var(--navy);">Asie du Sud-Est</span><div class="region-track"><div class="region-fill" style="width:80%;background:var(--teal-lt);"></div></div><span class="region-pct">80%</span></div>
        <div class="region-row"><span class="region-flag">🇪🇺</span><span class="region-name" style="color:var(--navy);">Europe</span><div class="region-track"><div class="region-fill" style="width:72%;background:var(--mint);"></div></div><span class="region-pct">72%</span></div>
        <div class="region-row"><span class="region-flag">🌎</span><span class="region-name" style="color:var(--navy);">Amérique Latine</span><div class="region-track"><div class="region-fill" style="width:60%;background:var(--gold);"></div></div><span class="region-pct">60%</span></div>
        <div class="region-row"><span class="region-flag">🌍</span><span class="region-name" style="color:var(--navy);">Afrique</span><div class="region-track"><div class="region-fill" style="width:45%;background:var(--orange);"></div></div><span class="region-pct">45%</span></div>
        <div class="region-row"><span class="region-flag">🌐</span><span class="region-name" style="color:var(--navy);">Océanie</span><div class="region-track"><div class="region-fill" style="width:30%;background:var(--gray);"></div></div><span class="region-pct">30%</span></div>
      </div>
      <div class="monde-regions">
        <div class="monde-region-card reveal" style="border-left-color:var(--teal);"><div class="monde-rc-head"><h4>🇺🇸 Amérique du Nord</h4><span style="color:var(--teal);">~45% des volumes</span></div><p class="monde-rc-desc">Principale zone d'usage institutionnel. Coinbase, Circle et Tether dominent. Adoption DeFi record.</p></div>
        <div class="monde-region-card reveal reveal-delay-1" style="border-left-color:var(--mint);"><div class="monde-rc-head"><h4>🇪🇺 Europe</h4><span style="color:var(--mint);">Adoption MiCA 2024</span></div><p class="monde-rc-desc">Cadre MiCA en vigueur. Forte adoption B2B pour paiements transfrontaliers intra-UE. EURC en hausse.</p></div>
        <div class="monde-region-card reveal reveal-delay-2" style="border-left-color:var(--teal-lt);"><div class="monde-rc-head"><h4>🌏 Asie du Sud-Est</h4><span style="color:var(--teal-lt);">Croissance +120%/an</span></div><p class="monde-rc-desc">Singapour, Hong Kong, Philippines : hubs régionaux. Remittances massivement basées sur stablecoins.</p></div>
        <div class="monde-region-card reveal reveal-delay-3" style="border-left-color:var(--gold);"><div class="monde-rc-head"><h4>🌍 Afrique &amp; Amérique Latine</h4><span style="color:var(--gold);">Refuge contre inflation</span></div><p class="monde-rc-desc">Argentine (+200% inflation), Nigeria, Zimbabwe. Stablecoins = protection de l'épargne populaire.</p></div>
      </div>
    </div>
    <div class="monde-footer reveal">🌐 Plus de <strong>180 pays</strong> utilisent activement des stablecoins en 2024 · <strong>300M+</strong> d'utilisateurs estimés</div>
  </div>
</section>

<!-- 08 MÉCANISMES -->
<section id="mecanismes">
  <div class="container">
    <p class="eyebrow">08 — Deep Dive</p>
    <h2 class="section-title">Mécanismes de Stabilité &amp; Collatéral</h2>
    <p class="section-sub">Le cycle Mint/Redeem, la Proof of Reserves, la sur-collatéralisation et l'arbitrage expliqués.</p>
    <div class="divider"></div>
    <div class="meca-grid">
      <div class="flowchart-wrap reveal">
        <div class="flowchart-header">CYCLE MINT / REDEEM</div>
        <div class="flowchart-cols">
          <div>
            <div class="fc-col-label mint">MINT → Émission</div>
            <div class="fc-nodes">
              <div class="fc-node mint-node"><h5>Utilisateur</h5><p>Envoie 1 000 USD</p></div>
              <div class="fc-arrow" style="color:var(--teal);">▼</div>
              <div class="fc-node mint-node"><h5>Émetteur</h5><p>Vérifie &amp; reçoit</p></div>
              <div class="fc-arrow" style="color:var(--teal);">▼</div>
              <div class="fc-node neutral"><h5>Réserve</h5><p>1 000 USD stockés</p></div>
              <div class="fc-arrow" style="color:var(--mint);">▼</div>
              <div class="fc-node mint-end"><h5>Mint ✓</h5><p>1 000 USDC créés</p></div>
            </div>
          </div>
          <div>
            <div class="fc-col-label redeem">REDEEM → Rachat</div>
            <div class="fc-nodes">
              <div class="fc-node redeem-node"><h5>Utilisateur</h5><p>Renvoie 1 000 USDC</p></div>
              <div class="fc-arrow" style="color:var(--orange);">▼</div>
              <div class="fc-node redeem-node"><h5>Émetteur</h5><p>Vérifie &amp; brûle</p></div>
              <div class="fc-arrow" style="color:var(--orange);">▼</div>
              <div class="fc-node neutral"><h5>Réserve</h5><p>Libère les fonds</p></div>
              <div class="fc-arrow" style="color:var(--red);">▼</div>
              <div class="fc-node redeem-end"><h5>Redeem ✓</h5><p>1 000 USD restitués</p></div>
            </div>
          </div>
        </div>
      </div>
      <div class="meca-blocks">
        <div class="meca-block reveal" style="border-left-color:var(--teal);">
          <div class="meca-block-head"><span>🛡️</span><h4 style="color:var(--teal-lt);">Proof of Reserves</h4></div>
          <p><strong>Audits trimestriels</strong> (ex: USDT) — un cabinet externe vérifie les réserves 4×/an et publie un rapport officiel.<br><br><em>Attestations temps réel</em> (ex: USDC / Chainlink PoR) — le collatéral est vérifiable on-chain à tout instant, sans intermédiaire.</p>
        </div>
        <div class="meca-block reveal reveal-delay-1" style="border-left-color:var(--gold);">
          <div class="meca-block-head"><span>🪙</span><h4 style="color:var(--gold);">Sur-Collatéralisation (DAI)</h4></div>
          <p>Pour émettre 100 DAI, un utilisateur dépose 150 $ d'ETH (ratio 150%). Si l'ETH chute, le système liquide automatiquement le collatéral avant d'atteindre la parité — protégeant le peg à $1.</p>
          <div class="collat-bar"><div class="collat-seg" style="width:66.6%;background:var(--gold);"></div><div class="collat-seg" style="width:33.4%;background:var(--mint);"></div></div>
          <div class="collat-labels"><span style="color:var(--gold);">150% collatéral</span><span style="color:var(--mint);">100% valeur émise</span></div>
        </div>
        <div class="meca-block reveal reveal-delay-2" style="border-left-color:var(--orange);">
          <div class="meca-block-head"><span>↔️</span><h4 style="color:var(--orange);">L'Arbitrage Stabilisateur</h4></div>
          <p><strong>Prix &lt; $1 ($0,99) :</strong> les traders achètent massivement → pression haussière.<br><strong>Prix &gt; $1 ($1,01) :</strong> ils vendent → pression baissière.<br><br>Ce mécanisme de marché libre ramène automatiquement le cours à $1 sans intervention centralisée.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- 09 CBDC -->
<section id="cbdc" class="bg-light">
  <div class="container">
    <p class="eyebrow">09 — Comparaison</p>
    <h2 class="section-title">Stablecoins vs CBDC</h2>
    <p class="section-sub">Monnaies numériques privées face aux Monnaies Numériques de Banque Centrale.</p>
    <div class="divider"></div>
    <div class="cbdc-grid reveal">
      <div class="cbdc-headers">
        <div class="cbdc-header priv"><span style="font-size:1.4rem;">🌐</span><div><h3>STABLECOINS PRIVÉS</h3><p>Tether · Circle · MakerDAO</p></div></div>
        <div class="cbdc-header pub"><span style="font-size:1.4rem;">🏛️</span><div><h3>CBDC PUBLIQUES</h3><p>BCE · Fed · Banque de Chine</p></div></div>
      </div>
      <div class="cbdc-row"><div style="grid-column:1/-1;" class="cbdc-row-label">🏢 Émetteur</div><div class="cbdc-cell priv-cell"><h5 style="color:var(--teal);">Entreprises Privées</h5><p>Tether Ltd, Circle, MakerDAO. Aucune garantie étatique — confiance fondée sur les audits et la réputation.</p></div><div class="cbdc-cell pub-cell"><h5 style="color:var(--purple);">Banques Centrales</h5><p>BCE, Fed, PBoC. Garantie souveraine de l'État — équivalent numérique de la monnaie banque centrale.</p></div></div>
      <div class="cbdc-row"><div style="grid-column:1/-1;" class="cbdc-row-label">🎯 Objectif</div><div class="cbdc-cell priv-cell"><h5 style="color:var(--teal);">Efficacité &amp; DeFi</h5><p>Trading 24h/7j, accès mondial sans frontières, DeFi, remittances — ouvert à tous, sans KYC obligatoire.</p></div><div class="cbdc-cell pub-cell"><h5 style="color:var(--purple);">Inclusion &amp; Souveraineté</h5><p>Inclusion financière des non-bancarisés, souveraineté monétaire, politique économique nationale.</p></div></div>
      <div class="cbdc-row"><div style="grid-column:1/-1;" class="cbdc-row-label">🔒 Anonymat vs Contrôle</div><div class="cbdc-cell priv-cell"><h5 style="color:var(--teal);">Pseudonymat</h5><p>Transactions on-chain traçables mais non nominatives. Pas d'identité obligatoire pour transacter.</p></div><div class="cbdc-cell pub-cell"><h5 style="color:var(--purple);">Contrôle Total</h5><p>KYC obligatoire, historique des transactions accessible aux autorités. Possibilité de gel de comptes.</p></div></div>
      <div class="cbdc-row"><div style="grid-column:1/-1;" class="cbdc-row-label">⚡ Stabilité &amp; Risque</div><div class="cbdc-cell priv-cell"><h5 style="color:var(--teal);">Risque Marché</h5><p>Risque de dépegging, faillite d'émetteur (ex: UST). Stabilité dépendante de la confiance des marchés.</p></div><div class="cbdc-cell pub-cell"><h5 style="color:var(--purple);">Risque Politique</h5><p>Stabilité garantie par la banque centrale. Risque politique de surveillance de masse et contrôle des flux.</p></div></div>
    </div>
    <div class="privacy-slider reveal">
      <p class="slider-title">Curseur Anonymat → Contrôle</p>
      <div class="slider-track">
        <div class="slider-marker sc">SC</div>
        <div class="slider-marker cb">CB</div>
      </div>
      <div class="slider-labels"><span class="l">◀ Anonymat total (Stablecoins)</span><span class="r">(CBDCs) Contrôle total ▶</span></div>
    </div>
  </div>
</section>

<!-- 10 MARCHÉS -->
<section id="marches">
  <div class="container">
    <p class="eyebrow">10 — Données</p>
    <h2 class="section-title">Marchés &amp; Statistiques</h2>
    <p class="section-sub">Chiffres clés et indicateurs de marché — sources CoinGecko / DefiLlama 2024.</p>
    <div class="divider"></div>
    <div class="marches-kpis">
      <div class="mkpi reveal"><div class="mkpi-val">$165B+</div><div class="mkpi-lbl">Capitalisation totale</div></div>
      <div class="mkpi reveal reveal-delay-1"><div class="mkpi-val">$10T+</div><div class="mkpi-lbl">Volume annuel (2023)</div></div>
      <div class="mkpi reveal reveal-delay-2"><div class="mkpi-val">200+</div><div class="mkpi-lbl">Stablecoins actifs</div></div>
      <div class="mkpi reveal reveal-delay-3"><div class="mkpi-val">300M+</div><div class="mkpi-lbl">Utilisateurs estimés</div></div>
    </div>
    <p class="marches-note reveal">Sources : CoinGecko, DefiLlama, Chainalysis — données 2024</p>
  </div>
</section>

<!-- 11 AVENIR -->
<section id="avenir" class="bg-light">
  <div class="container">
    <p class="eyebrow">11 — Perspectives</p>
    <h2 class="section-title">L'Avenir des Stablecoins</h2>
    <p class="section-sub">Quatre grandes tendances qui définiront l'écosystème stablecoin dans les prochaines années.</p>
    <div class="divider"></div>
    <div class="avenir-grid">
      <div class="avenir-items">
        <div class="avenir-item reveal"><div class="avenir-icon" style="background:rgba(8,145,178,.12);">🏦</div><div><h4>CBDCs</h4><p>Plus de 130 pays explorent des monnaies numériques de banque centrale. L'euro numérique est prévu pour 2025-2026.</p></div></div>
        <div class="avenir-item reveal reveal-delay-1"><div class="avenir-icon" style="background:rgba(245,158,11,.12);">📈</div><div><h4>Croissance DeFi</h4><p>Les stablecoins resteront le pilier de la finance décentralisée avec une adoption institutionnelle en forte hausse.</p></div></div>
        <div class="avenir-item reveal reveal-delay-2"><div class="avenir-icon" style="background:rgba(2,195,154,.12);">🌐</div><div><h4>Interopérabilité</h4><p>Les bridges cross-chain et standards communs permettront une utilisation fluide entre toutes les blockchains.</p></div></div>
        <div class="avenir-item reveal reveal-delay-3"><div class="avenir-icon" style="background:rgba(251,146,60,.12);">⚖️</div><div><h4>Régulation Claire</h4><p>Le cadre MiCA européen servira de modèle mondial, renforçant la confiance et l'adoption grand public.</p></div></div>
      </div>
      <div class="avenir-keypoints reveal">
        <h3>Points Clés</h3>
        <div class="kp-list">
          <div class="kp-item">Marché de +$165 milliards</div>
          <div class="kp-item">Pilier incontournable de la DeFi</div>
          <div class="kp-item">Adoption mondiale en accélération</div>
          <div class="kp-item">Régulation en cours de définition</div>
          <div class="kp-item">CBDCs émergentes à surveiller</div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <strong>Les Stablecoins</strong> · Guide Complet 2025 · Présentation Professionnelle<br><br>
  <span style="font-size:.72rem;">Données : CoinGecko, DefiLlama, Chainalysis — à titre informatif uniquement, ne constitue pas un conseil financier.</span>
</footer>

<script>
// Scroll reveal
const revealEls = document.querySelectorAll('.reveal');
const io = new IntersectionObserver(entries => {
  entries.forEach(e => { if (e.isIntersecting) { e.target.classList.add('visible'); io.unobserve(e.target); } });
}, { threshold: 0.1, rootMargin: '0px 0px -40px 0px' });
revealEls.forEach(el => io.observe(el));

// Active nav
const secs = document.querySelectorAll('section[id]');
const links = document.querySelectorAll('.nav-links a');
const nio = new IntersectionObserver(entries => {
  entries.forEach(e => {
    if (e.isIntersecting) {
      links.forEach(l => l.classList.remove('active'));
      const a = document.querySelector(`.nav-links a[href="#${e.target.id}"]`);
      if (a) a.classList.add('active');
    }
  });
}, { threshold: 0.4 });
secs.forEach(s => nio.observe(s));

// Animated bars on scroll
const barSections = document.querySelectorAll('#acteurs, #monde');
const barIO = new IntersectionObserver(entries => {
  entries.forEach(e => {
    if (e.isIntersecting) {
      e.target.querySelectorAll('.acteur-bar-fill, .region-fill').forEach(bar => {
        const finalW = bar.style.width;
        bar.style.width = '0';
        setTimeout(() => { bar.style.width = finalW; }, 150);
      });
      barIO.unobserve(e.target);
    }
  });
}, { threshold: 0.3 });
barSections.forEach(s => barIO.observe(s));
</script>
</body>
</html>
