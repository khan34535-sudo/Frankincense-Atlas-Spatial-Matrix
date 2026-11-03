<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<meta name="description" content="Interactive scientific atlas of Boswellia sacra (frankincense): trade routes, archaeology, chemistry, genomics, conservation and Dhofari heritage." />
<title>Asia Khan | Frankincense Atlas · Boswellia sacra</title>

<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" />
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700&family=Plus+Jakarta+Sans:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/three@0.128.0/examples/js/controls/OrbitControls.js"></script>
<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>
<script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.1/dist/chart.umd.min.js"></script>

<style>
  :root{
    --bg-deep:#08090b; --bg-surface:#111318; --bg-glass:rgba(17,19,24,.78);
    --gold:#d4af37; --gold-light:#f3e5ab; --gold-glow:#e6c666;
    --emerald:#2ecc71; --amber:#f39c12; --rose:#e74c3c;
    --cyan:#3498db; --violet:#9b59b6; --purple:#a855f7; --orange:#e67e22;
    --text:#e2e8f0; --muted:#8b98ab;
    --border:rgba(212,175,55,.22); --border-soft:rgba(255,255,255,.07);
    --font-title:'Cinzel',serif; --font-body:'Plus Jakarta Sans',sans-serif;
    --radius:16px;
  }
  *{margin:0;padding:0;box-sizing:border-box}
  html{scroll-behavior:smooth}
  body{
    background:var(--bg-deep);color:var(--text);font-family:var(--font-body);
    line-height:1.6;overflow-x:hidden;
    background-image:
      radial-gradient(circle at 12% 8%,rgba(212,175,55,.07) 0%,transparent 42%),
      radial-gradient(circle at 88% 92%,rgba(46,204,113,.05) 0%,transparent 42%);
    background-attachment:fixed;
  }
  body.modal-open{overflow:hidden}
  body::before{
    content:'';position:fixed;inset:0;pointer-events:none;z-index:0;opacity:.5;
    background-image:
      radial-gradient(1px 1px at 20% 30%,rgba(243,229,171,.5),transparent),
      radial-gradient(1px 1px at 70% 60%,rgba(243,229,171,.3),transparent),
      radial-gradient(1px 1px at 40% 80%,rgba(243,229,171,.35),transparent),
      radial-gradient(1px 1px at 85% 20%,rgba(243,229,171,.4),transparent);
    background-size:600px 600px;animation:drift 90s linear infinite;
  }
  @keyframes drift{to{background-position:600px 600px}}
  .container{max-width:1320px;margin:0 auto;padding:0 24px;position:relative;z-index:1}

  /* HEADER */
  .proto-header{
    background:linear-gradient(135deg,rgba(20,22,28,.96),rgba(8,9,11,.99));
    border-bottom:1px solid var(--border);backdrop-filter:blur(14px);
    padding:12px 24px;position:sticky;top:0;z-index:1000;
    display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:12px;
  }
  .badge{
    background:rgba(212,175,55,.14);border:1px solid var(--gold);color:var(--gold);
    font-family:var(--font-title);font-size:.7rem;letter-spacing:2.4px;
    padding:4px 10px;border-radius:4px;font-weight:700;
    animation:badgeGlow 3s ease-in-out infinite;
  }
  @keyframes badgeGlow{0%,100%{box-shadow:0 0 0 rgba(212,175,55,0)}50%{box-shadow:0 0 18px rgba(212,175,55,.35)}}
  .head-left{display:flex;align-items:center;gap:12px;flex-wrap:wrap}
  .head-left strong{font-family:var(--font-title);font-size:1rem;color:#fff}
  .cred{font-size:.8rem;color:var(--muted);display:flex;align-items:center;gap:14px;flex-wrap:wrap}
  .cred strong{color:#fff}
  .link{color:var(--gold);text-decoration:none;transition:color .3s}
  .link:hover{color:var(--gold-light);text-decoration:underline}

  /* HERO */
  .hero-pad{padding:48px 0 28px;text-align:center}
  .hero-pad h1{
    font-family:var(--font-title);font-size:clamp(2rem,4.6vw,3.2rem);
    margin-bottom:12px;letter-spacing:1px;line-height:1.15;
    background:linear-gradient(120deg,#fff 0%,var(--gold) 40%,#fff 60%,var(--gold) 80%,#fff 100%);
    background-size:220% auto;-webkit-background-clip:text;background-clip:text;
    -webkit-text-fill-color:transparent;animation:titleShimmer 8s linear infinite;
  }
  @keyframes titleShimmer{to{background-position:220% center}}
  .hero-pad .sub{
    font-size:1rem;color:var(--muted);max-width:860px;margin:0 auto 28px;
    font-weight:300;line-height:1.7;
  }

  /* BUTTON OPTIONS - Sticking Out Effect */
  .section-options{
    display:flex;flex-wrap:wrap;gap:12px;justify-content:center;
    margin-top:12px;margin-bottom:12px;
  }
  .opt-btn{
    display:flex;flex-direction:column;align-items:center;gap:4px;
    padding:16px 18px 12px;min-width:110px;
    background:linear-gradient(135deg,rgba(212,175,55,.08),rgba(0,0,0,.4));
    border:1px solid var(--border);border-radius:12px;
    cursor:pointer;font-family:var(--font-body);color:var(--text);
    transition:all .25s;position:relative;
  }
  .opt-btn:hover,.opt-btn:focus-visible{
    border-color:var(--gold);transform:translateY(-3px);
    box-shadow:0 10px 26px rgba(212,175,55,.28);
    background:linear-gradient(135deg,rgba(212,175,55,.18),rgba(0,0,0,.4));
    outline:none;
  }
  .opt-btn .oe{
    font-size:1.6rem;position:absolute;top:-14px;
    filter:drop-shadow(0 4px 6px rgba(0,0,0,0.8)) drop-shadow(0 0 10px rgba(212,175,55,.4));
    background:var(--bg-surface);border-radius:50%;
    width:34px;height:34px;display:grid;place-items:center;
    border:1px solid var(--border);transition:all .25s;
  }
  .opt-btn:hover .oe{
    transform:scale(1.1) translateY(-2px);
    border-color:var(--gold);
  }
  .opt-btn .ol{
    font-family:var(--font-title);font-size:.74rem;color:var(--gold-light);
    letter-spacing:.04em;font-weight:600;margin-top:12px;
  }

  /* MAP PANEL */
  .map-panel{
    background:var(--bg-glass);border:1px solid var(--border);border-radius:var(--radius);
    padding:20px;backdrop-filter:blur(12px);
    box-shadow:0 16px 44px rgba(0,0,0,.55),inset 0 1px 0 rgba(243,229,171,.05);
    position:relative;overflow:hidden;margin-bottom:32px;
  }
  .map-panel-title{
    display:flex;align-items:center;justify-content:space-between;gap:10px;
    margin-bottom:14px;flex-wrap:wrap;
  }
  .map-panel-title h2{
    font-family:var(--font-title);font-size:1.2rem;color:var(--gold-light);
    display:flex;align-items:center;gap:10px;
  }

  #map{
    height:560px;border-radius:12px;border:1px solid var(--border);
    overflow:hidden;position:relative;z-index:0;background:#000;
  }

  /* MODAL OVERLAY */
  .modal{
    position:fixed;inset:0;z-index:2000;
    background:rgba(4,5,7,.88);backdrop-filter:blur(10px);
    display:none;overflow-y:auto;padding:30px 16px;
  }
  .modal.show{display:block}
  .modal-card{
    background:linear-gradient(135deg,#14161b,#0a0b0d);
    border:1px solid var(--border);border-radius:16px;
    max-width:1100px;margin:0 auto;
    box-shadow:0 40px 100px rgba(0,0,0,.9),0 0 0 1px rgba(212,175,55,.15);
    animation:popIn .35s cubic-bezier(.2,.9,.3,1.2);
    position:relative;
    overflow:hidden;
  }
  .modal-card::before{
    content:'';position:absolute;top:0;left:-100%;width:50%;height:100%;
    background:linear-gradient(90deg,transparent,rgba(255,255,255,0.03),transparent);
    animation:scanline 8s linear infinite;pointer-events:none;
  }
  @keyframes scanline{to{left:200%}}
  @keyframes popIn{from{opacity:0;transform:scale(.96) translateY(20px)}to{opacity:1;transform:none}}
  
  /* MODAL HEAD - Sticking Out Icon */
  .modal-head{
    padding:24px 26px 16px;border-bottom:1px solid var(--border);
    display:flex;align-items:center;justify-content:space-between;gap:16px;
    position:sticky;top:0;
    background:linear-gradient(135deg,#1a1d24,#0e0f12);z-index:10;
    border-radius:16px 16px 0 0;
  }
  .modal-head-left{display:flex;align-items:center;gap:16px;position:relative}
  .modal-head .me{
    font-size:1.8rem;position:absolute;top:-20px;left:-10px;
    filter:drop-shadow(0 6px 8px rgba(0,0,0,0.9)) drop-shadow(0 0 15px var(--pop-color,var(--gold)));
    background:var(--bg-surface);border-radius:50%;
    width:48px;height:48px;display:grid;place-items:center;
    border:2px solid var(--pop-color,var(--gold));z-index:12;
  }
  .modal-head h3{font-family:var(--font-title);font-size:1.35rem;color:var(--pop-color,var(--gold-light));margin:0 0 0 32px;}
  .modal-head .kick{font-size:.64rem;letter-spacing:.15em;text-transform:uppercase;color:var(--muted);margin-top:4px;margin-left:32px}
  
  .modal-close{
    background:rgba(255,255,255,.06);border:1px solid var(--border-soft);color:var(--text);
    width:36px;height:36px;border-radius:50%;cursor:pointer;font-size:1rem;
    transition:all .2s;flex-shrink:0;
  }
  .modal-close:hover{background:var(--rose);border-color:var(--rose);color:#fff;transform:rotate(90deg)}
  .modal-body{padding:26px}

  /* 5W STRIP */
  .fivew{display:grid;grid-template-columns:repeat(5,1fr);gap:10px;margin-bottom:24px}
  @media(max-width:900px){.fivew{grid-template-columns:repeat(2,1fr)}}
  .w{
    background:linear-gradient(135deg,rgba(255,255,255,.03),rgba(0,0,0,.3));
    border:1px solid var(--border-soft);border-radius:10px;
    padding:11px 13px;position:relative;overflow:hidden;
  }
  .w::before{
    content:'';position:absolute;top:0;left:0;right:0;height:2px;
    background:var(--pop-color,var(--gold));opacity:.85;
  }
  .wk{font-family:var(--font-title);font-size:.58rem;letter-spacing:.14em;text-transform:uppercase;color:var(--pop-color,var(--gold));margin-bottom:4px}
  .wv{font-size:.8rem;color:var(--text);line-height:1.45}

  /* GRID SYSTEM */
  .grid-2{display:grid;grid-template-columns:1fr 1fr;gap:20px}
  .grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
  @media(max-width:900px){.grid-2,.grid-3{grid-template-columns:1fr}}
  .info{
    background:rgba(255,255,255,.02);border:1px solid var(--border-soft);
    border-radius:12px;padding:18px;position:relative;overflow:hidden;
    transition:all .3s;
  }
  .info::before{
    content:'';position:absolute;top:0;left:0;width:3px;height:100%;
    background:linear-gradient(180deg,var(--pop-color,var(--gold)),transparent);opacity:.6;
  }
  .info:hover{background:rgba(212,175,55,.05);transform:translateY(-2px);box-shadow:0 0 20px rgba(212,175,55,0.1)}
  .info h4{font-family:var(--font-title);color:var(--pop-color,var(--gold-light));margin-bottom:8px;font-size:1rem}
  .info p{color:var(--muted);font-size:.88rem;line-height:1.6}
  .info ul{padding-left:16px;color:var(--muted);font-size:.86rem;margin-top:6px}
  .info li{margin-bottom:5px}
  .info strong{color:#fff}

  /* 3D RESIN STAGE */
  .resin-stage{
    height:420px;border-radius:12px;
    background:radial-gradient(circle at center,rgba(30,35,45,.9) 0%,rgba(8,9,11,1) 100%);
    border:1px solid var(--border);position:relative;overflow:hidden;cursor:grab;
    width:100%;
    box-shadow:inset 0 0 40px rgba(46,204,113,0.05);
  }
  .resin-stage:active{cursor:grabbing}
  .resin-stage canvas{display:block;width:100%!important;height:100%!important}
  .resin-hint{
    position:absolute;bottom:12px;left:50%;transform:translateX(-50%);
    font-size:.68rem;color:var(--gold-light);background:rgba(8,9,11,.78);
    border:1px solid var(--border);padding:4px 12px;border-radius:999px;
    pointer-events:none;backdrop-filter:blur(6px);white-space:nowrap;
  }
  .grade-row{
    display:grid;grid-template-columns:repeat(4,1fr);gap:8px;margin-top:12px;
  }
  @media(max-width:600px){.grade-row{grid-template-columns:repeat(2,1fr)}}
  .grade-btn{
    background:rgba(255,255,255,.03);border:1px solid var(--border-soft);
    border-radius:99px;padding:10px 6px;cursor:pointer;
    font-family:var(--font-body);font-size:.72rem;font-weight:600;
    color:var(--text);transition:all .22s;text-align:center;
    position:relative;overflow:hidden;
  }
  .grade-btn::before{
    content:'';position:absolute;top:0;left:0;right:0;height:2px;
    background:var(--gc,var(--gold));
  }
  .grade-btn:hover,.grade-btn.active{
    background:color-mix(in srgb,var(--gc,var(--gold)) 14%,transparent);
    border-color:var(--gc,var(--gold));color:#fff;
    box-shadow:0 0 15px color-mix(in srgb,var(--gc,var(--gold)) 30%,transparent);
  }
  .grade-btn .gn{
    display:block;font-family:var(--font-title);font-size:.85rem;
    color:var(--gc,var(--gold));margin-bottom:2px;
  }

  /* TERROIR & MICROCLIMATE STYLING */
  #terroirMap{
    height:380px;border-radius:12px;border:1px solid var(--border);
    overflow:hidden;position:relative;margin-top:10px;background:#05070a;
    box-shadow:inset 0 0 30px rgba(212,175,55,0.05);
  }
  .terroir-grid{
    display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:12px;margin-top:14px;
  }
  .climate-card{
    background:rgba(255,255,255,.02);border:1px solid var(--border-soft);
    border-radius:10px;padding:14px;position:relative;
  }
  .climate-card h5{
    font-family:var(--font-title);font-size:.82rem;color:var(--gold-light);
    margin-bottom:6px;display:flex;align-items:center;gap:6px;
  }
  .climate-card p{font-size:.78rem;color:var(--muted);line-height:1.45}
  .zone-pill{
    display:inline-block;font-size:.65rem;font-weight:700;padding:2px 8px;
    border-radius:999px;margin-bottom:6px;text-transform:uppercase;letter-spacing:.05em;
  }

  /* GRADE CARDS */
  .grade-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(230px,1fr));gap:14px;margin-top:14px}
  .grade-card{
    background:linear-gradient(135deg,rgba(255,255,255,.03),rgba(0,0,0,.3));
    border:1px solid var(--border-soft);border-radius:12px;padding:16px;
    cursor:pointer;transition:all .25s;position:relative;overflow:hidden;
  }
  .grade-card::before{
    content:'';position:absolute;top:0;left:0;right:0;height:3px;
    background:var(--rc,var(--gold));
  }
  .grade-card:hover{border-color:var(--rc,var(--gold));transform:translateY(-3px);box-shadow:0 12px 30px rgba(0,0,0,.5),0 0 20px color-mix(in srgb,var(--rc) 20%,transparent)}
  .grade-card h4{
    font-family:var(--font-title);color:#fff;font-size:1rem;margin-bottom:3px;
    display:flex;align-items:center;justify-content:space-between;gap:8px;
  }
  .grade-card .rt{
    font-family:var(--font-body);font-size:.6rem;font-weight:700;
    letter-spacing:.08em;text-transform:uppercase;
    background:color-mix(in srgb,var(--rc,var(--gold)) 18%,transparent);
    color:var(--rc,var(--gold));padding:2px 8px;border-radius:999px;
  }
  .grade-card p{font-size:.78rem;color:var(--muted);line-height:1.45;margin-top:6px}
  .grade-card .open-hint{font-size:.66rem;color:var(--rc,var(--gold));margin-top:8px;font-weight:600}

  /* CHART */
  .chart-wrap{position:relative;height:340px;width:100%}

  /* TIMELINE */
  .tl-strip{
    display:flex;gap:10px;overflow-x:auto;padding:10px 4px 16px;
    scrollbar-width:thin;scrollbar-color:var(--gold) transparent;
  }
  .tl-strip::-webkit-scrollbar{height:6px}
  .tl-strip::-webkit-scrollbar-thumb{background:linear-gradient(90deg,var(--gold),var(--amber));border-radius:3px}
  .tl-chip{
    flex:0 0 auto;
    background:linear-gradient(135deg,color-mix(in srgb,var(--era) 10%,transparent),rgba(255,255,255,.02));
    border:1px solid color-mix(in srgb,var(--era) 30%,transparent);
    border-radius:14px;padding:14px 16px;cursor:pointer;transition:all .25s;
    text-align:left;font-family:inherit;color:inherit;min-width:140px;
    position:relative;overflow:hidden;
  }
  .tl-chip::before{
    content:'';position:absolute;top:0;left:0;right:0;height:3px;
    background:var(--era);box-shadow:0 0 12px var(--era);
  }
  .tl-chip:hover{
    border-color:var(--era);transform:translateY(-3px);
    box-shadow:0 8px 24px color-mix(in srgb,var(--era) 30%,transparent);
  }
  .tl-chip.active{
    border-color:var(--era);
    background:linear-gradient(135deg,color-mix(in srgb,var(--era) 22%,transparent),rgba(0,0,0,.3));
    box-shadow:0 0 24px color-mix(in srgb,var(--era) 50%,transparent),inset 0 0 20px color-mix(in srgb,var(--era) 15%,transparent);
    transform:translateY(-2px) scale(1.03);
  }
  .tl-chip .te{font-size:1.5rem;display:block;margin-bottom:4px;filter:drop-shadow(0 0 8px var(--era))}
  .tl-chip .yr{display:block;font-family:var(--font-title);font-size:.85rem;font-weight:700;color:var(--era);letter-spacing:.04em}
  .tl-chip .sh{display:block;font-size:.68rem;color:var(--muted);margin-top:2px}
  .tl-detail{
    background:linear-gradient(135deg,color-mix(in srgb,var(--era) 6%,rgba(255,255,255,.02)),rgba(0,0,0,.3));
    border:1px solid color-mix(in srgb,var(--era) 40%,transparent);
    border-radius:14px;padding:22px;margin-top:8px;animation:fadeUp .35s ease both;
    box-shadow:0 0 30px color-mix(in srgb,var(--era) 15%,transparent);
  }
  @keyframes fadeUp{from{opacity:0;transform:translateY(8px)}to{opacity:1;transform:none}}
  .tl-detail .when{
    font-family:var(--font-title);font-size:1.15rem;margin-bottom:6px;
    color:var(--era);display:flex;align-items:center;gap:10px;
  }
  .tl-detail .when .de{font-size:1.5rem;filter:drop-shadow(0 0 12px var(--era))}
  .tl-detail .who{font-size:.84rem;color:var(--gold-glow);margin-bottom:14px;font-weight:500}
  .tl-5w{display:grid;grid-template-columns:repeat(auto-fit,minmax(180px,1fr));gap:10px;margin-bottom:12px}
  .tl-5w .w{background:rgba(0,0,0,.35);border-radius:8px;padding:10px 12px;border-left:2px solid var(--era)}
  .tl-5w .wk{font-family:var(--font-title);font-size:.58rem;letter-spacing:.14em;text-transform:uppercase;color:var(--era);margin-bottom:3px}
  .tl-5w .wv{font-size:.8rem;color:var(--text);line-height:1.45}

  /* STATS */
  .stats-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));gap:12px}
  .stat{
    background:linear-gradient(135deg,rgba(212,175,55,.06),rgba(0,0,0,.3));
    border:1px solid var(--border);border-radius:12px;padding:16px 14px;text-align:center;
    transition:all .25s;
  }
  .stat:hover{transform:translateY(-2px);border-color:var(--gold-glow);box-shadow:0 0 15px rgba(212,175,55,0.2)}
  .stat .num{
    font-family:var(--font-title);font-size:1.7rem;font-weight:700;
    background:linear-gradient(135deg,#fff,var(--gold));
    -webkit-background-clip:text;background-clip:text;-webkit-text-fill-color:transparent;
    line-height:1;margin-bottom:4px;
  }
  .stat .lbl{font-size:.68rem;color:var(--muted);text-transform:uppercase;letter-spacing:.1em}
  .stat .src{font-size:.62rem;color:rgba(139,152,171,.7);margin-top:5px;font-style:italic}

  /* HEALTH CARDS */
  .health-grid{
    display:grid;grid-template-columns:repeat(auto-fit,minmax(300px,1fr));gap:16px;
  }
  .health-card{
    background:linear-gradient(135deg,rgba(255,255,255,.03),rgba(0,0,0,.4));
    border:1px solid var(--border-soft);border-radius:14px;
    padding:0;overflow:hidden;position:relative;transition:all .3s;
  }
  .health-card::before{
    content:'';position:absolute;top:0;left:0;right:0;height:3px;
    background:var(--hc,var(--gold));box-shadow:0 0 14px var(--hc,var(--gold));
  }
  .health-card:hover{
    border-color:var(--hc,var(--gold));transform:translateY(-3px);
    box-shadow:0 14px 36px rgba(0,0,0,.6),0 0 20px color-mix(in srgb,var(--hc) 20%,transparent);
  }
  .health-header{
    padding:18px 20px 14px;display:flex;align-items:center;gap:12px;
    border-bottom:1px solid var(--border-soft);
  }
  .health-icon{
    flex:0 0 auto;width:48px;height:48px;border-radius:12px;
    background:color-mix(in srgb,var(--hc,var(--gold)) 15%,transparent);
    border:1px solid color-mix(in srgb,var(--hc,var(--gold)) 40%,transparent);
    display:grid;place-items:center;font-size:1.5rem;
    filter:drop-shadow(0 0 10px color-mix(in srgb,var(--hc,var(--gold)) 40%,transparent));
  }
  .health-header h4{
    font-family:var(--font-title);font-size:1.05rem;
    color:var(--hc,var(--gold-light));margin:0;line-height:1.3;
  }
  .health-header .sub{
    font-size:.7rem;color:var(--muted);margin-top:2px;letter-spacing:.04em;
  }
  .health-body{padding:16px 20px 20px}
  .health-row{margin-bottom:14px}
  .health-row:last-child{margin-bottom:0}
  .health-label{
    font-family:var(--font-title);font-size:.58rem;letter-spacing:.14em;
    text-transform:uppercase;margin-bottom:5px;
    display:flex;align-items:center;gap:6px;
  }
  .health-label.trad{color:#d9a44c}
  .health-label.mod{color:#5ac8e8}
  .health-row p{
    font-size:.84rem;color:var(--text);line-height:1.55;
    padding-left:10px;border-left:2px solid var(--border-soft);
  }
  .health-label.trad + p{border-left-color:rgba(217,164,76,.5)}
  .health-label.mod + p{border-left-color:rgba(90,200,232,.5)}
  .health-row p strong{color:var(--gold-light)}
  .health-row p em{color:#a9bacb;font-style:normal;font-weight:500}
  .health-src{
    font-size:.68rem;color:rgba(139,152,171,.75);font-style:italic;
    margin-top:10px;padding-top:10px;border-top:1px dashed var(--border-soft);
  }
  .health-src a{color:var(--gold);text-decoration:none}
  .health-src a:hover{text-decoration:underline}

  .evidence-badge{
    display:inline-block;font-family:var(--font-body);font-size:.6rem;
    font-weight:700;letter-spacing:.06em;text-transform:uppercase;
    padding:2px 8px;border-radius:999px;margin-top:8px;
  }
  .evidence-badge.strong{background:rgba(46,204,113,.15);color:#2ecc71;border:1px solid rgba(46,204,113,.4)}
  .evidence-badge.moderate{background:rgba(243,156,18,.15);color:#f39c12;border:1px solid rgba(243,156,18,.4)}
  .evidence-badge.emerging{background:rgba(155,89,182,.15);color:#b07ad0;border:1px solid rgba(155,89,182,.4)}
  .evidence-badge.preliminary{background:rgba(231,76,60,.15);color:#e74c3c;border:1px solid rgba(231,76,60,.4)}

  .caution{
    background:linear-gradient(135deg,rgba(231,76,60,.08),rgba(0,0,0,.3));
    border-left:3px solid var(--rose);border-radius:0 10px 10px 0;
    padding:14px 18px;font-size:.86rem;color:var(--muted);margin-top:20px;
  }
  .caution strong{color:var(--rose)}

  /* GALLERY CARDS & HOLOGRAPHIC FRAMES */
  .gal-card{
    background:rgba(0,0,0,.4);border:1px solid var(--border);border-radius:12px;
    overflow:hidden;transition:all .3s;display:flex;flex-direction:column;
  }
  .gal-card:hover{transform:translateY(-4px);box-shadow:0 16px 40px rgba(0,0,0,.6);border-color:var(--gold)}
  .gal-card .frame{position:relative;width:100%;height:280px;background:#05070a;overflow:hidden;perspective:1000px}
  .gal-card .badge-i{
    position:absolute;top:10px;left:10px;font-size:.6rem;font-weight:700;
    letter-spacing:.1em;text-transform:uppercase;background:rgba(8,9,11,.9);
    border:1px solid var(--border);color:var(--gold-light);padding:3px 9px;
    border-radius:999px;z-index:10;backdrop-filter:blur(4px);
  }
  .gal-card .info-body{padding:16px;flex-grow:1;display:flex;flex-direction:column;justify-content:space-between}
  .gal-card h5{font-family:var(--font-title);color:var(--gold-light);font-size:.95rem;margin-bottom:6px}
  .gal-card p{font-size:.82rem;color:var(--muted);line-height:1.5}
  .gal-card .actions{margin-top:12px;display:flex;flex-wrap:wrap;gap:8px}
  .gal-card .actions a, .gal-card .actions button{
    font-size:.72rem;font-weight:600;padding:5px 12px;border-radius:999px;
    background:rgba(212,175,55,.1);border:1px solid var(--border);
    color:var(--gold);text-decoration:none;transition:all .18s;cursor:pointer;
  }
  .gal-card .actions a:hover, .gal-card .actions button:hover{background:var(--gold);color:#0a0a0a;border-color:var(--gold)}

  /* 3D HOLOGRAPHIC FRAME TILT EFFECTS */
  .holographic-3d-card {
    perspective: 1000px;
    overflow: hidden;
    border: 1px solid var(--border);
    box-shadow: inset 0 0 15px rgba(212, 175, 55, 0.15);
    background: #05070a;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: transform 0.15s ease-out;
  }

  .holographic-3d-card img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.15s ease-out;
  }

  /* REFS */
  .refs{padding-left:22px;color:var(--muted);font-size:.86rem}
  .refs li{margin-bottom:10px;line-height:1.6;padding-left:4px}
  .refs li::marker{color:var(--gold);font-weight:700}

  footer{text-align:center;padding:36px 20px;border-top:1px solid var(--border);color:var(--muted);font-size:.8rem;margin-top:40px}

  /* SVG DATA VISUALIZATIONS */
  .data-svg text {
    font-family: 'Plus Jakarta Sans', sans-serif;
    text-shadow: 0 0 5px currentColor;
    transition: all 0.3s;
  }
  .data-svg .node {
    filter: drop-shadow(0 0 8px currentColor);
    animation: nodePulse 2s infinite alternate;
  }
  @keyframes nodePulse {
    from { opacity: 0.7; transform: scale(1); }
    to { opacity: 1; transform: scale(1.1); }
  }
  .data-svg .scan-line {
    stroke: rgba(46, 204, 113, 0.3);
    stroke-width: 2;
    animation: scanLine 3s linear infinite;
  }
  @keyframes scanLine {
    0% { transform: translateX(-200px); opacity: 0; }
    10% { opacity: 1; }
    90% { opacity: 1; }
    100% { transform: translateX(1000px); opacity: 0; }
  }
  .data-svg .branch {
    stroke-dasharray: 1000;
    stroke-dashoffset: 1000;
    animation: drawBranch 2s ease-out forwards;
  }
  @keyframes drawBranch { to { stroke-dashoffset: 0; } }

  /* ========== LAYMAN POPUP (PURPLE STAR) ========== */
  .layman-trigger {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    width: 26px;
    height: 26px;
    margin-left: 8px;
    vertical-align: middle;
    cursor: pointer;
    filter: drop-shadow(0 0 6px #a855f7);
    transition: transform .2s;
  }
  .layman-trigger:hover {
    transform: scale(1.25);
  }
  .layman-trigger svg {
    width: 100%;
    height: 100%;
    display: block;
  }
  .layman-badge {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    background: rgba(168,85,247,.12);
    border: 1px solid rgba(168,85,247,.5);
    padding: 3px 10px 3px 6px;
    border-radius: 999px;
    font-size: .68rem;
    color: #c084fc;
    cursor: pointer;
    transition: all .2s;
    margin-top: 6px;
    font-weight: 600;
    letter-spacing: .04em;
  }
  .layman-badge:hover {
    background: rgba(168,85,247,.25);
    border-color: #a855f7;
    box-shadow: 0 0 14px rgba(168,85,247,.4);
  }
  .layman-badge svg {
    width: 16px;
    height: 16px;
    flex-shrink: 0;
  }
  /* modal for layman */
  #m-layman {
    z-index: 2500;
  }
  .layman-card {
    max-width: 640px;
    border-color: #a855f7;
    box-shadow: 0 40px 100px rgba(0,0,0,.9), 0 0 0 1px rgba(168,85,247,.3);
  }
  .layman-card .modal-head {
    background: linear-gradient(135deg,#1f122b,#0e0714);
  }
  .layman-card .modal-head h3 {
    color: #c084fc;
  }
  .layman-card .me {
    border-color: #a855f7;
    color: #c084fc;
  }
  .layman-content {
    font-size: .92rem;
    line-height: 1.7;
    color: #e2e8f0;
  }
  .layman-content p {
    margin-bottom: 12px;
  }
  .layman-content strong {
    color: #c084fc;
  }
  .layman-content em {
    color: #f3e5ab;
    font-style: normal;
  }
  .layman-content ul {
    padding-left: 20px;
    margin: 10px 0;
  }
  .layman-content li {
    margin-bottom: 8px;
  }

  /* ========== TIMELINE MAP LABEL ========== */
  .tl-map-label {
    position: absolute;
    top: 8px;
    left: 8px;
    z-index: 1000;
    background: rgba(8,9,11,.92);
    border: 1px solid var(--border);
    border-radius: 8px;
    padding: 4px 10px;
    font-size: .68rem;
    font-weight: 600;
    color: var(--gold-light);
    letter-spacing: .04em;
    backdrop-filter: blur(6px);
    pointer-events: none;
    display: flex;
    align-items: center;
    gap: 6px;
    box-shadow: 0 2px 10px rgba(0,0,0,.6);
  }
  .tl-map-label .lbl-dot {
    width: 8px;
    height: 8px;
    border-radius: 50%;
    flex-shrink: 0;
  }
  .tl-map-wrapper {
    position: relative;
    flex: 1;
    min-width: 220px;
    height: 200px;
    border-radius: 12px;
    overflow: hidden;
  }

  /* ===================== v2 ADDITIONS ===================== */
  .hero-pad{position:relative;overflow:hidden}
  .hero-pad>*:not(canvas){position:relative;z-index:1}
  #heroSmoke{position:absolute;inset:0;width:100%;height:100%;z-index:0;pointer-events:none}
  .legend-line{font-size:.76rem;color:var(--muted);margin:-10px auto 20px;max-width:860px;line-height:1.9}

  /* evidence tags */
  .nv,.ill,.vf{display:inline-block;font-family:var(--font-body);font-size:.58rem;font-weight:700;letter-spacing:.06em;
    text-transform:uppercase;padding:1px 7px;border-radius:999px;margin-left:4px;vertical-align:middle;white-space:nowrap;font-style:normal}
  .nv{background:rgba(231,76,60,.12);color:#ff8f80;border:1px solid rgba(231,76,60,.45)}
  .ill{background:rgba(168,85,247,.12);color:#cfa8ff;border:1px solid rgba(168,85,247,.5)}
  .vf{background:rgba(46,204,113,.12);color:#63e6a6;border:1px solid rgba(46,204,113,.45)}
  .srcline{font-size:.76rem;color:var(--muted);margin-top:10px;font-style:italic;line-height:1.7}
  .srcline a,.refs a{color:var(--gold)}
  .ref-h{font-family:var(--font-title);color:var(--gold-light);font-size:.95rem;margin:22px 0 8px}

  /* grouped navigation: every section visible, themed colour bands */
  .theme-nav{margin:28px 0 8px}
  .nav-groups{display:flex;flex-wrap:wrap;gap:26px 22px;justify-content:center;align-items:flex-start}
  .nav-group{--gc:#d4af37;display:flex;flex-direction:column;gap:20px;max-width:100%}
  .nav-group[data-theme="origins"]{--gc:#d4af37}
  .nav-group[data-theme="science"]{--gc:#5dade2}
  .nav-group[data-theme="conservation"]{--gc:#2ecc71}
  .nav-group[data-theme="culture"]{--gc:#c39bd3}
  .nav-group[data-theme="trade"]{--gc:#e67e22}
  .nav-group[data-theme="refs"]{--gc:#8b98ab}
  .nav-group-label{font-family:var(--font-title);font-size:.72rem;letter-spacing:.14em;text-transform:uppercase;
    color:var(--gc);padding:0 2px 7px;border-bottom:3px solid var(--gc);
    box-shadow:0 8px 14px -10px var(--gc);display:flex;align-items:center;gap:7px}
  .nav-group-label em{margin-left:auto;font-style:normal;font-family:var(--font-body);opacity:.6;font-size:.68rem}
  .nav-group-btns{display:flex;flex-wrap:nowrap;gap:20px 7px;padding-top:6px}
  .nav-group .opt-btn{min-width:0;width:84px;padding:16px 6px 11px}
  .nav-group .opt-btn .ol{font-size:.68rem;text-align:center;line-height:1.25;letter-spacing:.02em}
  .nav-group .opt-btn:hover,.nav-group .opt-btn:focus-visible{border-color:var(--gc);box-shadow:0 10px 26px color-mix(in srgb,var(--gc) 35%,transparent)}
  .nav-group .opt-btn .ol{color:var(--text)}
  @media (max-width:1240px){.nav-group-btns{flex-wrap:wrap}}
  .opt-btn{transform-style:preserve-3d;will-change:transform}
  @media (max-width:640px){
    .nav-groups{gap:22px 0}
    .nav-group{width:100%}
    .nav-group-btns{gap:20px 8px}
    .nav-group .opt-btn{flex:1 1 calc(33% - 8px);width:auto}
  }
  @keyframes btnEnter{from{opacity:0;transform:translateY(14px) rotateX(-25deg)}to{opacity:1;transform:none}}
  .opt-btn.enter{animation:btnEnter .45s cubic-bezier(.2,.9,.3,1.1) both}

  /* tilted 3D satellite map */
  .map-3d-stage{perspective:1500px;perspective-origin:50% 0%;height:560px;border-radius:12px;overflow:hidden;
    background:radial-gradient(circle at 50% 100%,#10202c,#05070a)}
  .map-3d-stage #map{transition:transform .85s cubic-bezier(.2,.8,.2,1);transform-origin:50% 100%}
  .map-3d-stage.tilted #map{transform:rotateX(40deg) scale(1.3)}

  /* 3D terroir relief */
  .t3d-head{margin-top:22px}
  .t3d-head h4{font-family:var(--font-title);color:var(--gold-light);font-size:1rem;margin-bottom:4px}
  .t3d-head p{font-size:.8rem;color:var(--muted);margin-bottom:10px;line-height:1.55}
  .terroir3d{height:440px}
  .t3d-bar{display:flex;flex-wrap:wrap;gap:8px;margin-top:10px}
  .t3d-btn{font-family:var(--font-body);font-size:.76rem;font-weight:600;color:var(--text);min-height:40px;
    background:rgba(255,255,255,.04);border:1px solid var(--border);border-radius:999px;padding:8px 16px;cursor:pointer;transition:all .2s}
  .t3d-btn:hover,.t3d-btn:focus-visible{border-color:var(--gold);background:rgba(212,175,55,.12);outline:none}
  @media(max-width:600px){.terroir3d{height:340px}.map-3d-stage{height:440px}#map{height:440px}}

  @media (prefers-reduced-motion: reduce){
    #heroSmoke{display:none}
    *,*::before,*::after{animation-duration:.01ms!important;animation-iteration-count:1!important;transition-duration:.01ms!important;scroll-behavior:auto!important}
  }
</style>
</head>
<body>

<header class="proto-header">
  <div class="head-left">
    <span class="badge">◈ PROTOTYPE</span>
    <strong>Frankincense Atlas</strong>
  </div>
  <div class="cred">
    <span>Author: <strong>Asia Khan</strong> · Behavioural UX Researcher &amp; 3D Spatial Architect</span>
    <span>Hon. BA, McMaster University</span>
    <span>✉ <a href="mailto:asiaaamirkhan@outlook.com" class="link">asiaaamirkhan@outlook.com</a></span>
  </div>
</header>

<div class="container">
  <section class="hero-pad">
    <canvas id="heroSmoke" aria-hidden="true"></canvas>
    <h1>The Sacred Resin: Boswellia Sacra &amp; Spatial Matrix</h1>
    <p class="sub">An interactive scientific atlas exploring <em>Boswellia sacra</em> — historical trade routes, archaeological discoveries, chemical biomarkers, paleoclimate proxies, evolutionary genomics, population dynamics, and indigenous Dhofari ethnography.</p>
    <p class="legend-line">Evidence labels used throughout: <span class="vf">verified</span> checked against the original record · <span class="ill">illustrative</span> conceptual graphic or score, not measured data · <span class="nv">needs source</span> claim retained but not yet traced to a primary source.</p>
  </section>

  <!-- GROUPED NAVIGATION: all sections visible, grouped by theme -->
  <nav class="theme-nav" aria-label="Atlas sections">
    <div class="nav-groups" id="sectionOptions">
      <div class="nav-group" data-theme="origins" role="group" aria-label="Origins">
        <div class="nav-group-label"><span>🏺</span> Origins<em>5</em></div>
        <div class="nav-group-btns">
          <button class="opt-btn" data-open="origin" data-group="origins"><span class="oe">🏺</span><span class="ol">Origin &amp; Discovery</span></button>
          <button class="opt-btn" data-open="timeline" data-group="origins"><span class="oe">⏳</span><span class="ol">Timeline</span></button>
          <button class="opt-btn" data-open="archaeology" data-group="origins"><span class="oe">🏛️</span><span class="ol">Archaeology</span></button>
          <button class="opt-btn" data-open="residue" data-group="origins"><span class="oe">⚱️</span><span class="ol">Residues</span></button>
          <button class="opt-btn" data-open="etymology" data-group="origins"><span class="oe">💎</span><span class="ol">Etymology</span></button>
        </div>
      </div>
      <div class="nav-group" data-theme="science" role="group" aria-label="Science">
        <div class="nav-group-label"><span>🧪</span> Science<em>8</em></div>
        <div class="nav-group-btns">
          <button class="opt-btn" data-open="resin" data-group="science"><span class="oe">🔶</span><span class="ol">Resin 3D</span></button>
          <button class="opt-btn" data-open="smell" data-group="science"><span class="oe">👃</span><span class="ol">Smell Index</span></button>
          <button class="opt-btn" data-open="botanical" data-group="science"><span class="oe">🌿</span><span class="ol">Botanical</span></button>
          <button class="opt-btn" data-open="biomarkers" data-group="science"><span class="oe">🧪</span><span class="ol">Biomarkers</span></button>
          <button class="opt-btn" data-open="provenance" data-group="science"><span class="oe">🔍</span><span class="ol">Provenance</span></button>
          <button class="opt-btn" data-open="evolution" data-group="science"><span class="oe">🧬</span><span class="ol">Evolution</span></button>
          <button class="opt-btn" data-open="genomics" data-group="science"><span class="oe">🧬</span><span class="ol">Genomics Lab</span></button>
          <button class="opt-btn" data-open="microbiome" data-group="science"><span class="oe">🦠</span><span class="ol">Microbiome</span></button>
        </div>
      </div>
      <div class="nav-group" data-theme="conservation" role="group" aria-label="Conservation">
        <div class="nav-group-label"><span>🌳</span> Conservation<em>5</em></div>
        <div class="nav-group-btns">
          <button class="opt-btn" data-open="population" data-group="conservation"><span class="oe">📊</span><span class="ol">Population Impact</span></button>
          <button class="opt-btn" data-open="climate" data-group="conservation"><span class="oe">🌡️</span><span class="ol">Threats</span></button>
          <button class="opt-btn" data-open="carbon" data-group="conservation"><span class="oe">💨</span><span class="ol">Carbon Balance</span></button>
          <button class="opt-btn" data-open="satellite" data-group="conservation"><span class="oe">🛰️</span><span class="ol">Satellite Mapping</span></button>
          <button class="opt-btn" data-open="future" data-group="conservation"><span class="oe">🚀</span><span class="ol">Future Lab</span></button>
        </div>
      </div>
      <div class="nav-group" data-theme="culture" role="group" aria-label="Culture">
        <div class="nav-group-label"><span>📖</span> Culture<em>3</em></div>
        <div class="nav-group-btns">
          <button class="opt-btn" data-open="ethnography" data-group="culture"><span class="oe">⛺</span><span class="ol">Ethnography</span></button>
          <button class="opt-btn" data-open="scriptural" data-group="culture"><span class="oe">📖</span><span class="ol">Sacred Texts</span></button>
          <button class="opt-btn" data-open="uses" data-group="culture"><span class="oe">⚕️</span><span class="ol">Health Profiles</span></button>
        </div>
      </div>
      <div class="nav-group" data-theme="trade" role="group" aria-label="Trade">
        <div class="nav-group-label"><span>🚢</span> Trade<em>2</em></div>
        <div class="nav-group-btns">
          <button class="opt-btn" data-open="history" data-group="trade"><span class="oe">📜</span><span class="ol">Trade Route</span></button>
          <button class="opt-btn" data-open="trade" data-group="trade"><span class="oe">🚢</span><span class="ol">Trade Today</span></button>
        </div>
      </div>
      <div class="nav-group" data-theme="refs" role="group" aria-label="Sources">
        <div class="nav-group-label"><span>📚</span> Sources</div>
        <div class="nav-group-btns">
          <button class="opt-btn" data-open="refs" data-group="refs"><span class="oe">📚</span><span class="ol">References</span></button>
        </div>
      </div>
    </div>
  </nav>

  <section class="map-panel">
    <div class="map-panel-title">
      <h2><span>🛰️</span> Where Frankincense Grows Today · 3D Aerial Satellite GIS</h2>
      <span class="tag">Esri World Imagery</span>
    </div>
    <div class="map-3d-stage" id="mapStage"><div id="map"></div></div>
    <p class="srcline">Tap ⛰️ for a tilted 3D perspective · 🌳 zooms to tree level · pinch or scroll to zoom · drag to pan.</p>
  </section>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · ORIGIN & ANCIENT DISCOVERY
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-origin" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#d4af37">
      <div class="modal-head-left">
        <span class="me">🏺</span>
        <div><h3>Origin &amp; Ancient Discovery</h3><div class="kick">Credible Historical &amp; Archaeological Timeline</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Early South Arabian communities &amp; Egyptian expeditions</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Early ritual use &amp; incense trade</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Southern Arabia (incl. Dhofar) &amp; Punt (location debated)</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Earliest use debated | c. 1479–1458 BCE (Hatshepsut)</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Sacred offerings, mummification, &amp; royal prestige</div></div>
      </div>

      <div class="grid-2">
        <div class="info" style="--pop-color:#d4af37">
          <h4>📜 First Archaeological Evidence &amp; Discovery
            <span class="layman-badge" onclick="openLayman('origin')">
              <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2L14.5 9H22L16 13.5L18.5 21L12 16.5L5.5 21L8 13.5L2 9H9.5L12 2Z" fill="#a855f7" stroke="#d8b4fe" stroke-width="0.8"/></svg>
              Simple Summary
            </span>
          </h4>
          <p>Frankincense has been used in southern Arabia since prehistory, but <strong>when</strong> harvesting and trade began is not firmly established. A date of roughly <strong>6000 BCE</strong> is often quoted <span class="nv">needs source</span> and should be read as an estimate. The best-documented trade infrastructure in this atlas is later: <strong>Sumhuram (Khor Rori)</strong> from the 3rd century BCE and <strong>Al-Baleed</strong> in the medieval period (UNESCO, 2000).</p>
          <p style="margin-top:10px;">Reliefs at <strong>Queen Hatshepsut's temple at Deir el-Bahari (c. 1479–1458 BCE)</strong> record an Egyptian expedition to <strong>Punt</strong> and show incense trees being carried to Egypt in baskets. Where Punt lay is debated (often placed in the Horn of Africa / southern Red Sea region), and the species shown is not certain, so the reliefs should not be read as evidence for <em>Boswellia sacra</em> in Oman.</p>
        </div>

        <div class="info" style="--pop-color:#3498db">
          <h4>📚 Credible Classical Sources</h4>
          <ul>
            <li><strong>Herodotus (c. 484–425 BCE):</strong> Recorded in <em>Histories (Book III)</em> that Southern Arabia was the sole source of frankincense, myrrh, and cinnamon, guarded by winged serpents.</li>
            <li><strong>Pliny the Elder (23–79 CE):</strong> In <em>Natural History</em> 12.32 he describes the route from Thomna (Tamna), capital of the Gebbanitae, to Gaza as <strong>65 stages</strong> with halts for camels, and in 12.65 lists frankincense at 3–6 denarii per pound by quality. He makes no comparison with gold.</li>
            <li><strong>Periplus of the Erythraean Sea (1st Century CE):</strong> An anonymous Graeco-Roman maritime guide that names a frankincense-exporting harbour on the Dhofar coast (<em>Moscha Limen</em>, usually identified with Sumhuram / Khor Rori).</li>
          </ul>
        </div>
      </div>

      <!-- PERSON OF INTEREST: PROF. AHMED AL-HARRASI -->
      <div class="info" style="margin-top:20px; --pop-color:#2ecc71;">
        <h4>👨‍🔬 Person of Interest: Prof. Ahmed Al-Harrasi</h4>
        <p>Prof. Ahmed Al-Harrasi is the Chair of the Natural & Medical Sciences Research Center (NMSRC) and Vice Chancellor for Graduate Studies, Research & External Relations at the University of Nizwa, Oman. He is a leading global authority on the chemistry and extraction of <em>Boswellia sacra</em> frankincense, spearheading research into its bioactive compounds, including boswellic acids and incensole acetate.</p>
        <p style="margin-top:8px;"><em>Key Contributions:</em> His group has published extensively on the chemistry and bioactivity of <em>Boswellia</em> resins, including the 2022 <em>B. sacra</em> genome (Khan et al., <em>iScience</em>). Titles and roles are as listed by the University of Nizwa and may have changed.</p>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · RESIN 3D & TERROIR
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-resin" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#2ecc71">
      <div class="modal-head-left">
        <span class="me">🔶</span>
        <div><h3>3D Resin Grade Viewer &amp; Microclimate Terroir Matrix</h3><div class="kick">Drag to rotate · pinch or scroll to zoom · pick a grade or zone</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Dhofari harvesters · Salalah traders</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Four commercial grades: Hojari, Najdi, Shathari, Shaabi</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Jebel Samhan · Nejd Plateau · NW Dhofar · Escarpment</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Traditional trade categories · composition studied in recent decades</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Microclimate, rainfall &amp; elevation drive chemical synthesis</div></div>
      </div>

      <div class="info" style="margin-bottom: 20px; --pop-color: #2ecc71;">
        <h4>🌳 Are there different species of trees?
          <span class="layman-badge" onclick="openLayman('resin')">
            <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2L14.5 9H22L16 13.5L18.5 21L12 16.5L5.5 21L8 13.5L2 9H9.5L12 2Z" fill="#a855f7" stroke="#d8b4fe" stroke-width="0.8"/></svg>
            Simple Summary
          </span>
        </h4>
        <p>No. The four trade grades are all described as coming from the <strong>same species</strong> (<em>Boswellia sacra</em>). Differences in colour, chemistry and aroma are linked to <strong>where the tree grows</strong> (microclimate, altitude, rainfall) and also to <strong>harvest timing, tapping practice and how the resin is sorted and graded</strong>. Whether genetic differences between Dhofari populations also contribute has not been ruled out <span class="nv">open question</span>.</p>
      </div>

      <div class="resin-stage" id="resin-3d">
        <div class="resin-hint">Drag to rotate · pinch / scroll to zoom · pick a grade below</div>
      </div>
      <div class="grade-row" id="gradeRow">
        <button class="grade-btn active" data-grade="hojari" style="--gc:#2ecc71"><span class="gn">Hojari</span>Royal Green</button>
        <button class="grade-btn" data-grade="najdi" style="--gc:#f39c12"><span class="gn">Najdi</span>Amber</button>
        <button class="grade-btn" data-grade="shathari" style="--gc:#d4af37"><span class="gn">Shathari</span>Golden</button>
        <button class="grade-btn" data-grade="shaabi" style="--gc:#8b98ab"><span class="gn">Shaabi</span>Dark</button>
      </div>

      <div style="margin-top:28px;">
        <h3 style="font-family:var(--font-title);color:var(--gold-light);font-size:1.1rem;margin-bottom:6px">🗺️ Dhofar Terroir &amp; Microclimate Geographic Map</h3>
        <p style="font-size:.82rem;color:var(--muted);margin-bottom:12px">Explore the microclimate, elevation and rainfall gradient across the Dhofar region that is associated with differences in resin grade. Zone locations and the altitude and rainfall ranges below are indicative summaries, not outputs of a single dataset <span class="nv">needs source</span>.</p>

        <div id="terroirMap"></div>

        <div class="t3d-head">
          <h4>🏔️ 3D Terroir Relief <span class="ill">schematic</span></h4>
          <p>A vertically exaggerated sketch of the south-to-north gradient: Arabian Sea → Khareef escarpment → Samhan highlands → Nejd plateau. Heights are illustrative (not a DEM); zone positions follow the map above. Tap a glowing zone to open its grade profile.</p>
        </div>
        <div class="resin-stage terroir3d" id="terroir3d"><div class="resin-hint">Drag to rotate · two-finger drag to pan · pinch / scroll to zoom</div></div>
        <div class="t3d-bar">
          <button type="button" class="t3d-btn" id="t3dFog" aria-pressed="true">☁️ Khareef fog: on</button>
          <button type="button" class="t3d-btn" id="t3dReset">↺ Reset view</button>
        </div>

        <div class="terroir-grid">
          <div class="climate-card" style="border-left: 3px solid #2ecc71;">
            <span class="zone-pill" style="background:rgba(46,204,113,.15);color:#2ecc71;">Hojari Zone</span>
            <h5>⛰️ Jebel Samhan &amp; High Valleys</h5>
            <p><strong>Altitude:</strong> 800m – 1,500m<br>
            <strong>Rainfall:</strong> &lt; 50 mm/yr (Behind fog belt)<br>
            <strong>Microclimate:</strong> Dry, arid, desert monsoon rain shadow. High diurnal temperature swings.<br>
            <strong>Terroir Impact:</strong> Stress causes low fluid yield, translucent green hue, high <em>α-pinene</em> concentration.</p>
          </div>

          <div class="climate-card" style="border-left: 3px solid #f39c12;">
            <span class="zone-pill" style="background:rgba(243,156,18,.15);color:#f39c12;">Najdi Zone</span>
            <h5>🏜️ Nejd Desert Plateau</h5>
            <p><strong>Altitude:</strong> 500m – 900m<br>
            <strong>Rainfall:</strong> 30 – 80 mm/yr<br>
            <strong>Microclimate:</strong> Extreme desert heat, zero monsoon fog reach, dry northerly winds.<br>
            <strong>Terroir Impact:</strong> High heat drives high <em>myrcene</em> monoterpenes; amber-pale yellow colouration.</p>
          </div>

          <div class="climate-card" style="border-left: 3px solid #d4af37;">
            <span class="zone-pill" style="background:rgba(212,175,55,.15);color:#d4af37;">Shathari Zone</span>
            <h5>🌾 North-West Dry Wadis</h5>
            <p><strong>Altitude:</strong> 300m – 600m<br>
            <strong>Rainfall:</strong> 50 – 100 mm/yr<br>
            <strong>Microclimate:</strong> Moderate desert transitional zone, warm limestone gravel plains.<br>
            <strong>Terroir Impact:</strong> Higher <em>limonene</em> levels yield bright citrus notes and warm golden tears.</p>
          </div>

          <div class="climate-card" style="border-left: 3px solid #8b98ab;">
            <span class="zone-pill" style="background:rgba(139,152,171,.15);color:#8b98ab;">Shaabi Zone</span>
            <h5>🌫️ Coastal Escarpment / Khareef Belt</h5>
            <p><strong>Altitude:</strong> 50m – 400m<br>
            <strong>Rainfall:</strong> 150 – 300 mm/yr (Monsoon moisture)<br>
            <strong>Microclimate:</strong> Dense summer fog (Khareef), high ambient humidity, mild temperature.<br>
            <strong>Terroir Impact:</strong> High moisture yields high fluid volume, darker amber colour, deeper woody base notes.</p>
          </div>
        </div>
      </div>

      <h3 style="font-family:var(--font-title);color:var(--gold-light);font-size:1.05rem;margin-top:28px;margin-bottom:6px">Click any grade for its full profile</h3>
      <div class="grade-grid">
        <div class="grade-card" data-info="hojari" style="--rc:#2ecc71">
          <h4>Hojari <span class="rt">Grade 1</span></h4>
          <p>Pale translucent · Samhan mountains · reference grade</p>
          <div class="open-hint">→ Full profile</div>
        </div>
        <div class="grade-card" data-info="najdi" style="--rc:#f39c12">
          <h4>Najdi <span class="rt">Grade 2</span></h4>
          <p>Pale yellow · plateau behind Dhofar · high myrcene</p>
          <div class="open-hint">→ Full profile</div>
        </div>
        <div class="grade-card" data-info="shathari" style="--rc:#d4af37">
          <h4>Shathari <span class="rt">Grade 3</span></h4>
          <p>Golden yellow · north-west Dhofar · high limonene</p>
          <div class="open-hint">→ Full profile</div>
        </div>
        <div class="grade-card" data-info="shaabi" style="--rc:#8b98ab">
          <h4>Shaabi <span class="rt">Grade 4</span></h4>
          <p>Darker amber · everyday / local · deeper woody</p>
          <div class="open-hint">→ Full profile</div>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · SMELL INDEX
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-smell" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#e6c666">
      <div class="modal-head-left">
        <span class="me">👃</span>
        <div><h3>Smell Index · Radar Comparison</h3><div class="kick">Illustrative sensory profile · not measured data</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Atlas author’s qualitative synthesis</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Six odour dimensions across four grades</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Samhan · Nejd · north-west Dhofar</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Scores are illustrative</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Compare how the four grades are described to smell</div></div>
      </div>
      <div class="chart-wrap"><canvas id="smellChart"></canvas></div>
      <div class="info" style="margin-top:22px">
        <h4>Comparison Table</h4>
        <table style="width:100%;border-collapse:collapse;font-size:.82rem;margin-top:10px">
          <thead>
            <tr style="text-align:left;color:var(--gold);border-bottom:1px solid var(--border)">
              <th style="padding:8px 6px">Attribute</th>
              <th style="padding:8px 6px">Hojari</th>
              <th style="padding:8px 6px">Najdi</th>
              <th style="padding:8px 6px">Shathari</th>
              <th style="padding:8px 6px">Shaabi</th>
            </tr>
          </thead>
          <tbody style="color:var(--muted)">
            <tr><td style="padding:6px">Resinous / incense</td><td>9</td><td>8</td><td>7</td><td>8</td></tr>
            <tr><td style="padding:6px">Citrus (lemon/orange)</td><td>6</td><td>8</td><td>8</td><td>4</td></tr>
            <tr><td style="padding:6px">Minty-turpentine</td><td>7</td><td>5</td><td>4</td><td>3</td></tr>
            <tr><td style="padding:6px">Woody</td><td>4</td><td>5</td><td>6</td><td>7</td></tr>
            <tr><td style="padding:6px">Sweet / balsamic</td><td>5</td><td>6</td><td>6</td><td>5</td></tr>
            <tr><td style="padding:6px">Spicy / herb-like</td><td>3</td><td>4</td><td>4</td><td>4</td></tr>
          </tbody>
        </table>
        <p style="font-size:.76rem;color:var(--muted);font-style:italic;margin-top:10px">The 0–10 scores are the atlas author’s illustrative summary of how the four grades are described in the trade and in the literature <span class="ill">illustrative</span>. They are <strong>not</strong> published GC-olfactometry or panel measurements. See Al-Harrasi et al. (2019) for the underlying chemistry.</p>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · ARCHAEOLOGY
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-archaeology" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#d4af37">
      <div class="modal-head-left">
        <span class="me">🏛️</span>
        <div><h3>Archaeological Discoveries &amp; Maritime Port Heritage</h3><div class="kick">Al-Baleed Archaeological Park · Khor Rori (Sumhuram) · UNESCO Land of Frankincense</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Hadrami Kings · Omani Sailors · Roman, Indian &amp; Chinese Merchants</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Port Cities, Forts, Grand Mosque, Ancient Dhow Ships &amp; Lagoons</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Al-Baleed Archaeological Park &amp; Sumhuram (Khor Rori)</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">3rd c. BCE (Sumhuram) → 8th-16th c. CE (Al-Baleed)</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Maritime frankincense trade hubs connecting Arabia to global empires</div></div>
      </div>

      <div class="info" style="margin-bottom:20px; --pop-color:#d4af37;">
        <h4>🏰 Al-Baleed Archaeological Park &amp; The Ancient Maritime City (Zafar)
          <span class="layman-badge" onclick="openLayman('archaeology')">
            <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2L14.5 9H22L16 13.5L18.5 21L12 16.5L5.5 21L8 13.5L2 9H9.5L12 2Z" fill="#a855f7" stroke="#d8b4fe" stroke-width="0.8"/></svg>
            Simple Summary
          </span>
        </h4>
        <p>Al-Baleed (ancient Zafar) stands as one of the premier maritime trading hubs of the medieval Islamic world on the Indian Ocean. Prospering between the 8th and 16th centuries CE, the city grew rich from controlling the harvest and seaward export of Dhofar's royal frankincense. Systematic excavations have brought to light four principal architectural structures that defined the civic, military, economic, and maritime heart of the port.</p>
      </div>

      <!-- 4 STRUCTURED CARDS FOR AL-BALEED LANDMARKS WITH 3D VIEWERS & LOCAL IMAGES -->
      <div class="grid-2" style="margin-bottom:24px">
        
        <!-- CARD 1: GRAND MOSQUE -->
        <div class="gal-card">
          <div class="frame holographic-3d-card">
            <span class="badge-i">Landmark 1 · Grand Mosque</span>
            <img src="1.png" alt="Al-Baleed Grand Mosque Landmark 1" onerror="this.onerror=null; this.src='https://placehold.co/600x400/111318/d4af37?text=Image+Not+Found+In+Folder';" />
          </div>
          <div class="info-body">
            <h5>🕌 1. The Grand Mosque (Al-Balid)</h5>
            <p>A monumental 8th–10th century sanctuary spanning over 1,732 m². It featured a grand central courtyard and a vast prayer hall supported by <strong>144 octagonal stone columns</strong>.</p>
            <div class="actions">
              <button onclick="openLandmarkDetail(1)">📜 View Historical Importance</button>
              <a href="https://nabataea.net/explore/cities_and_sites/al-balid-mosque/" target="_blank" rel="noopener">Nabataea Report</a>
            </div>
          </div>
        </div>

        <!-- CARD 2: AL-BALEED FORT -->
        <div class="gal-card">
          <div class="frame holographic-3d-card">
            <span class="badge-i">Landmark 2 · Citadel / Fort</span>
            <img src="2.png" alt="Al-Baleed Fortress Landmark 2" onerror="this.onerror=null; this.src='https://placehold.co/600x400/111318/d4af37?text=Image+Not+Found+In+Folder';" />
          </div>
          <div class="info-body">
            <h5>🏰 2. Al-Baleed Fortress (Husn)</h5>
            <p>Spanning 3,623 m², this multi-story royal citadel housed the governor and elite garrison, with massive curtain towers protecting secure resin storehouses.</p>
            <div class="actions">
              <button onclick="openLandmarkDetail(2)">📜 View Historical Importance</button>
              <a href="https://www.a61s.it/en/lavori/projects/baleed-fortress-husn/sym_589" target="_blank" rel="noopener">Acaia 61 Project</a>
            </div>
          </div>
        </div>

        <!-- CARD 3: DEFENSIVE CITY WALLS -->
        <div class="gal-card">
          <div class="frame holographic-3d-card">
            <span class="badge-i">Landmark 3 · Perimeter Wall</span>
            <img src="3.png" alt="Defensive City Walls Landmark 3" onerror="this.onerror=null; this.src='https://placehold.co/600x400/111318/d4af37?text=Image+Not+Found+In+Folder';" />
          </div>
          <div class="info-body">
            <h5>🧱 3. Defensive City Walls &amp; Moat</h5>
            <p>A fortified outer wall reinforced with watchtowers and a deep defensive moat channel connected to the lagoon provided security against inland raids.</p>
            <div class="actions">
              <button onclick="openLandmarkDetail(3)">📜 View Historical Importance</button>
              <a href="https://whc.unesco.org/en/list/1010/" target="_blank" rel="noopener">UNESCO listing</a>
            </div>
          </div>
        </div>

        <!-- CARD 4: KHOR LAGOON & MULTIPLE BOATS -->
        <div class="gal-card">
          <div class="frame holographic-3d-card">
            <span class="badge-i">Landmark 4 &amp; 4.1 · Harbor &amp; Dhow Fleet</span>
            <div style="display:flex; width:100%; height:100%;">
              <img src="4.png" alt="Khor Al-Baleed Lagoon Landmark 4" style="width:50%; height:100%; object-fit:cover; border-right:1px solid var(--border);" onerror="this.onerror=null; this.src='https://placehold.co/600x400/111318/d4af37?text=Image+4+Missing';" />
              <img src="4.1.png" alt="Additional Vessel 4.1 Sambuk / Dhow" style="width:50%; height:100%; object-fit:cover;" onerror="this.onerror=null; this.src='https://placehold.co/600x400/111318/d4af37?text=Image+4.1+Missing';" />
            </div>
          </div>
          <div class="info-body">
            <h5>🌊 4. Khor Al-Baleed Lagoon &amp; 4.1 Traditional Vessels</h5>
            <p>Natural sheltered lagoon where traditional Omani dhows (including Sambuk and Ghanja models) loaded frankincense for high-seas trade to China and India.</p>
            <div class="actions">
              <button onclick="openLandmarkDetail(4)">📜 View Historical Importance</button>
              <a href="https://whc.unesco.org/en/list/1010/" target="_blank" rel="noopener">UNESCO listing</a>
            </div>
          </div>
        </div>

      </div>

      <div class="grid-2">
        <div class="info" style="--pop-color:#3498db;">
          <h4>⚓ Sumhuram (Khor Rori) — The Incense Route Outpost</h4>
          <p>Founded in the 3rd century BCE by the Hadramaut Kingdom, Sumhuram was built as a fortified coastal outpost to control the collection and maritime export of Dhofari frankincense.</p>
          <ul style="margin-top:8px;">
            <li><strong>Natural Harbor:</strong> Built on a prominent limestone bluff overlooking the Khor Rori lagoon, providing a sheltered anchorage for ocean-crossing dhows.</li>
            <li><strong>Inscriptions &amp; Storage:</strong> South Arabian inscriptions and storage structures were recovered at the site <span class="nv">details need source</span>.</li>
            <li><strong>Global Reach:</strong> Excavated artifacts include Roman amphorae, Bronze incense burners, and Indian pottery, indicating trade links across the Indian Ocean.</li>
          </ul>
        </div>

        <div class="info" style="--pop-color:#2ecc71;">
          <h4>⛵ Museum of the Frankincense Land &amp; Historic Ships (Vessels 4 &amp; 4.1)</h4>
          <p>Located right within the Al-Baleed Archaeological Park, the museum features two main exhibition halls highlighting maritime and land trade history:</p>
          <ul style="margin-top:8px;">
            <li><strong>Maritime Hall &amp; Significant Ships:</strong> Displays meticulously detailed scale models and timber construction techniques of historic Omani ships—including the <em>Sohar</em>, traditional <em>Baghla</em>, <em>Ghanja</em>, and the <strong>4.1 Sambuk Dhow</strong> that carried resin across the high seas.</li>
            <li><strong>Ancient Navigation:</strong> Displays traditional celestial navigation tools (such as the <em>Kamal</em>) used by Omani navigators like Ibn Majid to ride monsoon winds across the Arabian Sea.</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- SECONDARY NESTED MODAL (WINDOW WITHIN A WINDOW) FOR LANDMARK DETAILS -->
<div class="modal" id="m-landmark-detail" aria-hidden="true" style="z-index:2200">
  <div class="modal-card" role="dialog" aria-modal="true" style="max-width:700px">
    <div class="modal-head" id="landmarkDetailHead">
      <div class="modal-head-left">
        <span class="me" id="landmarkDetailEmoji">🏛️</span>
        <div><h3 id="landmarkDetailTitle">Landmark Detail</h3><div class="kick">Archaeological &amp; Historical Importance</div></div>
      </div>
      <button class="modal-close" onclick="closeLandmarkDetail()">✕</button>
    </div>
    <div class="modal-body" id="landmarkDetailBody"></div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · ETHNOGRAPHY
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-ethnography" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#e67e22">
      <div class="modal-head-left">
        <span class="me">⛺</span>
        <div><h3>Ethnographic Matrix &amp; Indigenous Heritage</h3><div class="kick">Modern South Arabian Tribes · Tapping Seasons · Folk Rituals</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Shahri (Jibbali) &amp; Mahri pastoralists</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Modern South Arabian languages &amp; tribal tree tenure</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Jebel Samhan · Nejd Plateau · Dhofar Wadis</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Pre-Arabic antiquity → Traditional harvesting calendar</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Preserve indigenous ecological knowledge &amp; living heritage</div></div>
      </div>

      <div class="grid-3">
        <div class="info" style="--pop-color:#e67e22">
          <h4>🗣️ Indigenous Language &amp; Lineage</h4>
          <p>The traditional harvesters of Dhofar belong primarily to the <strong>Shahri (Jibbali)</strong> and <strong>Mahri</strong> tribal lineages. They speak unwritten Modern South Arabian languages—Semitic languages that are distinct from Arabic and not descended from it, with rich local botanical vocabularies.</p>
        </div>

        <div class="info" style="--pop-color:#f39c12">
          <h4>📅 Seasonal Harvesting Calendar <span class="nv">verify terms &amp; dates</span></h4>
          <p style="font-size:.74rem;color:var(--muted);margin-bottom:6px">Indicative only. Local season names and months should be checked against field ethnography (e.g., Miller &amp; Morris, 1988) before reuse.</p>
          <ul>
            <li><strong>Al-Khafif (Spring / March–April):</strong> The first light incision (<em>tazwa</em>) is made in the bark using the traditional <em>manqaf</em> knife to wake the tree.</li>
            <li><strong>Al-Sarb (Autumn / Oct–Nov):</strong> The primary harvesting season following the Khareef monsoon fog, yielding the highest-grade resin tears after drying for 2–3 weeks.</li>
            <li><strong>Al-Jaz (Winter Rest):</strong> Trees are left dormant to recover fluids and avoid permanent cell damage during dry winds.</li>
          </ul>
        </div>

        <div class="info" style="--pop-color:#2ecc71">
          <h4>🔥 Domestic Rituals &amp; Folk Medicine</h4>
          <p>In Dhofari homes, frankincense resin is burned daily in ornate clay incense burners (<em>Majmar</em>) for purification, welcoming guests, and scenting clothes. Ethnographic records document its medicinal role in chewing for oral hygiene, boiling in hot water for bronchial clarity, and applying oil to soothe joints.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · BIOMARKERS & PALEOCLIMATE (REDESIGNED)
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-biomarkers" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#2ecc71">
      <div class="modal-head-left">
        <span class="me">🧪</span>
        <div><h3>Analytical Biomarkers &amp; Paleoclimate Matrix</h3><div class="kick">GC-MS Fingerprinting · Isotope Geochemistry · Monsoon Proxies</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Analytical chemists · Geochemists · Paleoclimatologists</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Incensole acetate, Boswellic acids, &amp; δ¹³C/δ¹⁸O isotopes</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Dhofar monsoon shadow · Global paleoclimate archives</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Proxy approach (concept)</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Illustrate how chemistry and isotopes can inform trade and climate studies</div></div>
      </div>

      <div class="grid-3" style="margin-bottom:20px">
        <div class="info" style="--pop-color:#2ecc71">
          <h4>🔬 Diagnostic Resin Biomarkers
            <span class="layman-badge" onclick="openLayman('biomarkers')">
              <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2L14.5 9H22L16 13.5L18.5 21L12 16.5L5.5 21L8 13.5L2 9H9.5L12 2Z" fill="#a855f7" stroke="#d8b4fe" stroke-width="0.8"/></svg>
              Simple Summary
            </span>
          </h4>
          <p>Mass spectrometry can profile the chemistry of <em>Boswellia</em> resins. <strong>Incensole</strong> and <strong>incensole acetate</strong> are characteristic diterpenoids (especially abundant in <em>B. papyrifera</em>) and, together with pentacyclic triterpenes such as <strong>AKBA</strong> (3-O-acetyl-11-keto-β-boswellic acid), are used as chemical markers. How specific each marker is varies by species and sample.</p>
        </div>

        <div class="info" style="--pop-color:#3498db">
          <h4>🌪️ Paleoclimate Proxies (δ¹³C &amp; δ¹⁸O)
            <span class="layman-badge" onclick="openLayman('paleoclimate')">
              <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2L14.5 9H22L16 13.5L18.5 21L12 16.5L5.5 21L8 13.5L2 9H9.5L12 2Z" fill="#a855f7" stroke="#d8b4fe" stroke-width="0.8"/></svg>
              Simple Summary
            </span>
          </h4>
          <p>Stable carbon (δ¹³C) and oxygen (δ¹⁸O) isotope ratios in plant tissue respond to water stress: higher δ¹³C can reflect stomatal closure and greater water-use efficiency, and enriched δ¹⁸O can reflect dry air and strong evaporation. This is a well-established approach in other plants. A published, dated Holocene isotope record from <em>Boswellia</em> resin or wood is <strong>not cited here</strong>, so the chart below is a concept sketch only <span class="nv">no B. sacra record cited</span>.</p>
        </div>

        <div class="info" style="--pop-color:#e74c3c">
          <h4>🔥 Thermal Oxidation Products
            <span class="layman-badge" onclick="openLayman('thermal')">
              <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2L14.5 9H22L16 13.5L18.5 21L12 16.5L5.5 21L8 13.5L2 9H9.5L12 2Z" fill="#a855f7" stroke="#d8b4fe" stroke-width="0.8"/></svg>
              Simple Summary
            </span>
          </h4>
          <p>When resin is burned during rituals, thermal degradation creates oxidized compounds such as <strong>incensole oxide</strong>. Finding heat-altered compounds in ancient censers can provide supporting evidence that incense was burned rather than only stored.</p>
        </div>
      </div>

      <!-- FUTURISTIC BIOMARKER SPECTRUM GRAPH -->
      <div class="gal-card" style="margin-bottom:20px;">
        <div class="frame" style="aspect-ratio:16/7; background:#05070a; position:relative; overflow:hidden;">
          <span class="badge-i">Plate IV · GC-MS Biomarker Spectrum · Illustrative</span>
          
          <svg class="data-svg" viewBox="0 0 1000 400" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
            <defs>
              <filter id="neonGlowGreen" x="-50%" y="-50%" width="200%" height="200%">
                <feGaussianBlur stdDeviation="6" result="blur" />
                <feMerge>
                  <feMergeNode in="blur" />
                  <feMergeNode in="blur" />
                  <feMergeNode in="SourceGraphic" />
                </feMerge>
              </filter>
              <filter id="neonGlowCyan" x="-50%" y="-50%" width="200%" height="200%">
                <feGaussianBlur stdDeviation="6" result="blur" />
                <feMerge>
                  <feMergeNode in="blur" />
                  <feMergeNode in="SourceGraphic" />
                </feMerge>
              </filter>
            </defs>

            <!-- Background Grid -->
            <g stroke="rgba(46, 204, 113, 0.1)" stroke-width="1">
              <line x1="50" y1="50" x2="50" y2="350" />
              <line x1="50" y1="350" x2="950" y2="350" />
              <line x1="50" y1="200" x2="950" y2="200" stroke-dasharray="5 5" />
              <line x1="50" y1="100" x2="950" y2="100" stroke-dasharray="5 5" />
              <line x1="250" y1="50" x2="250" y2="350" stroke-dasharray="5 5" />
              <line x1="450" y1="50" x2="450" y2="350" stroke-dasharray="5 5" />
              <line x1="650" y1="50" x2="650" y2="350" stroke-dasharray="5 5" />
              <line x1="850" y1="50" x2="850" y2="350" stroke-dasharray="5 5" />
            </g>

            <!-- Axis Labels -->
            <text x="500" y="390" fill="#8b98ab" font-size="14" text-anchor="middle" letter-spacing="2">RETENTION TIME (schematic)</text>
            <text x="20" y="200" fill="#8b98ab" font-size="14" text-anchor="middle" transform="rotate(-90 20 200)" letter-spacing="2">ABUNDANCE</text>

            <!-- Moving Scanline -->
            <line class="scan-line" x1="50" y1="50" x2="50" y2="350" />

            <!-- Main Spectrum Path -->
            <path class="branch" d="M50 350 L120 345 L150 320 L165 348 L210 342 L230 180 L245 345 L310 340 L340 90 L355 345 L410 348 L460 210 L480 345 L540 340 L580 60 L600 348 L680 342 L720 140 L740 345 L820 348 L880 300 L950 350" 
                  fill="none" stroke="#2ecc71" stroke-width="3" filter="url(#neonGlowGreen)"/>
            
            <!-- Secondary Cyan Path for layered look -->
            <path d="M50 340 L120 335 L150 310 L165 338 L210 332 L230 170 L245 335 L310 330 L340 80 L355 335 L410 338 L460 200 L480 335 L540 330 L580 50 L600 338 L680 332 L720 130 L740 335 L820 338 L880 290 L950 340" 
                  fill="none" stroke="#3498db" stroke-width="1.5" opacity="0.6" stroke-dasharray="4 4"/>

            <!-- Nodes and Labels -->
            <!-- α-Pinene -->
            <circle cx="230" cy="180" r="6" fill="#2ecc71" class="node"/>
            <line x1="230" y1="180" x2="230" y2="120" stroke="#2ecc71" stroke-width="1.5"/>
            <text x="230" y="105" fill="#2ecc71" font-size="12" text-anchor="middle" font-weight="700">α-Pinene</text>
            <text x="230" y="90" fill="#8b98ab" font-size="10" text-anchor="middle">MW 136</text>

            <!-- Incensole Acetate -->
            <circle cx="340" cy="90" r="6" fill="#2ecc71" class="node"/>
            <line x1="340" y1="90" x2="340" y2="60" stroke="#2ecc71" stroke-width="1.5"/>
            <text x="340" y="45" fill="#2ecc71" font-size="12" text-anchor="middle" font-weight="700">Incensole Acetate</text>
            <text x="340" y="30" fill="#8b98ab" font-size="10" text-anchor="middle">MW 348</text>

            <!-- AKBA -->
            <circle cx="580" cy="60" r="6" fill="#e6c666" class="node" style="color:#e6c666"/>
            <line x1="580" y1="60" x2="580" y2="30" stroke="#e6c666" stroke-width="1.5"/>
            <text x="580" y="20" fill="#e6c666" font-size="12" text-anchor="middle" font-weight="700">AKBA</text>
            <text x="580" y="10" fill="#8b98ab" font-size="10" text-anchor="middle">MW 513</text>

            <!-- Incensole Oxide -->
            <circle cx="720" cy="140" r="6" fill="#e74c3c" class="node" style="color:#e74c3c"/>
            <line x1="720" y1="140" x2="720" y2="100" stroke="#e74c3c" stroke-width="1.5"/>
            <text x="720" y="85" fill="#e74c3c" font-size="12" text-anchor="middle" font-weight="700">Incensole Oxide</text>
            <text x="720" y="70" fill="#8b98ab" font-size="10" text-anchor="middle">MW 322</text>
          </svg>
        </div>
      </div>

      <p class="srcline" style="margin:-6px 0 18px">Plate IV is a schematic chromatogram: peak positions and heights are invented for illustration; labels give approximate molecular weights (g/mol).</p>
      <h4 style="font-family:var(--font-title);color:var(--gold-light);margin-bottom:8px">📊 Isotope Proxy Concept <span class="ill">illustrative</span></h4>
      <p class="srcline" style="margin:0 0 10px">Invented values to show how two proxies could move together. Not measured data.</p>
      <div class="chart-wrap"><canvas id="isotopeChart"></canvas></div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · ARCHAEOLOGICAL RESIDUE INDEX
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-residue" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#9b59b6">
      <div class="modal-head-left">
        <span class="me">⚱️</span>
        <div><h3>Archaeological Residue Index</h3><div class="kick">Egyptian Mummification · Graeco-Roman Altars · Unguentaria</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Archaeological chemists · conservators</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Pyrolysis-GC-MS residue extraction from artifacts</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Nile Valley · Tel Arad · Roman Empire sarcophagi</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">1500 BCE – 400 CE</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Physical evidence of sacred, medicinal, &amp; funerary use</div></div>
      </div>

      <div class="grid-2" style="margin-bottom:20px">
        <div class="info" style="--pop-color:#9b59b6">
          <h4>⚰️ Egyptian Embalming Balms</h4>
          <p>Chemical analyses of Egyptian embalming materials have identified many resins, balms and gums. <em>Boswellia</em> / frankincense has been reported in some analyses, but it is documented far less often than conifer and pistacia resins, and how central it was to mummification is still debated <span class="nv">cite specific studies</span>.</p>
        </div>

        <div class="info" style="--pop-color:#f39c12">
          <h4>🏛️ Altar Residues &amp; Roman Unguentaria</h4>
          <p>Residue analysis of the incense altars at the Judahite shrine of Tel Arad reported frankincense with animal fat on the larger altar (Arie, Rosen &amp; Namdar, 2020) <span class="nv">re-check citation</span>. Claims about boswellic acids in Roman <em>unguentaria</em> are retained from the earlier draft but need a specific citation <span class="nv">needs source</span>.</p>
        </div>
      </div>

      <!-- VISUAL PLATE FOR MUMMY & RESIDUE ANALYSIS -->
      <div class="gal-card">
        <div class="frame" style="aspect-ratio:16/7">
          <span class="badge-i">Plate V · Residue analysis workflow · Illustrative</span>
          <svg viewBox="0 0 1000 400" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
            <rect width="1000" height="400" fill="#0d0f14"/>
            <g transform="translate(150, 80)">
              <path d="M50 200 C20 180 10 120 30 80 C40 60 45 30 50 10 L150 10 C155 30 160 60 170 80 C190 120 180 180 150 200 Z" fill="#2b2015" stroke="#d4af37" stroke-width="3"/>
              <ellipse cx="100" cy="10" rx="50" ry="8" fill="#4a3825" stroke="#d4af37" stroke-width="2"/>
              <path d="M40 120 Q100 150 160 120" fill="none" stroke="#9b59b6" stroke-width="3" stroke-dasharray="4 4"/>
              <text x="100" y="240" fill="#f3e5ab" font-family="sans-serif" font-size="12" text-anchor="middle">Canopic Jar / Altar Vessel</text>
            </g>
            <path d="M380 180 L480 180" stroke="#d4af37" stroke-width="3"/>
            <g transform="translate(520, 80)">
              <rect x="0" y="20" width="380" height="180" rx="12" fill="#151922" stroke="#3498db" stroke-width="2"/>
              <text x="190" y="50" fill="#3498db" font-family="sans-serif" font-size="14" font-weight="700" text-anchor="middle">Pyrolysis-GC-MS Spectrometry</text>
              <path d="M30 150 L80 140 L110 80 L130 150 L180 150 L210 60 L240 150 L300 150 L330 110 L350 150" fill="none" stroke="#2ecc71" stroke-width="2"/>
              <text x="190" y="180" fill="#8b98ab" font-family="sans-serif" font-size="11" text-anchor="middle">Detection of AKBA &amp; Incensole Acetate</text>
            </g>
          </svg>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · EVOLUTIONARY GENOMICS (REDESIGNED)
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-evolution" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#a855f7">
      <div class="modal-head-left">
        <span class="me">🧬</span>
        <div><h3>Evolutionary Genomics &amp; Phylogenetics</h3><div class="kick">667.8 Mb Assembly · Gypsy Retroelements · Speciation</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Botanical geneticists · Evolutionary biologists</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">De novo genome assembly (667.8 Mb, 18,564 genes)</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Arabian Peninsula &amp; Horn of Africa</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Genome published 2022 (Khan et al., <em>iScience</em>)</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Understand resin pathway expansion &amp; xerophytic survival</div></div>
      </div>

      <div class="grid-2" style="margin-bottom:20px">
        <div class="info" style="--pop-color:#a855f7">
          <h4>🧬 Genome Structure &amp; Gene Duplication
            <span class="layman-badge" onclick="openLayman('genome')">
              <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2L14.5 9H22L16 13.5L18.5 21L12 16.5L5.5 21L8 13.5L2 9H9.5L12 2Z" fill="#a855f7" stroke="#d8b4fe" stroke-width="0.8"/></svg>
              Simple Summary
            </span>
          </h4>
          <p>Recent de novo genome sequencing of <em>Boswellia sacra</em> revealed a <strong>667.8 Mb assembly</strong> encoding 18,564 high-confidence protein-encoding genes. The genome retains the signature of the ancient eudicot-wide hexaploidy (about 115–130 million years ago) and shows no further whole-genome duplication in the <em>B. sacra</em> lineage. The authors report a major expansion of <strong>Gypsy retroelements within the last ~2 million years</strong> (Gypsy elements make up 119.1 Mb). Links from that expansion to stress-response pathways are the authors’ interpretation <span class="vf">verified</span>.</p>
        </div>

        <div class="info" style="--pop-color:#3498db">
          <h4>🌳 Speciation &amp; Chemical Divergence</h4>
          <p>Boswellia species differ in chemistry and range, including <em>Boswellia sacra</em> (Arabia/Somaliland), <em>B. frereana</em> (Somaliland), <em>B. serrata</em> (India), and <em>B. papyrifera</em> (Ethiopia). <em>B. sacra</em> resin is rich in pentacyclic triterpenes (boswellic acids), whereas <em>B. frereana</em> resin is chemically distinct (reported to be rich in lupeol-type triterpenes). Ecological explanations for these differences are not cited here <span class="nv">needs source</span>.</p>
        </div>
      </div>

      <!-- FUTURISTIC PHYLOGENETIC TREE GRAPH -->
      <div class="gal-card">
        <div class="frame" style="aspect-ratio:16/7; background:#05070a; position:relative; overflow:hidden;">
          <span class="badge-i">Plate VI · Schematic species diagram · Illustrative (not a computed phylogeny)</span>
          
          <svg class="data-svg" viewBox="0 0 1000 350" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
            <rect width="1000" height="350" fill="#0a0c10"/>
            
            <!-- Background Grid -->
            <g stroke="rgba(168, 85, 247, 0.1)" stroke-width="1">
              <line x1="100" y1="50" x2="100" y2="300" />
              <line x1="250" y1="50" x2="250" y2="300" />
              <line x1="400" y1="50" x2="400" y2="300" />
              <line x1="550" y1="50" x2="550" y2="300" />
              <line x1="700" y1="50" x2="700" y2="300" />
            </g>

            <!-- Axis / Time scale -->
            <text x="100" y="330" fill="#8b98ab" font-size="12" text-anchor="middle">Ancestor</text>
            <text x="550" y="330" fill="#8b98ab" font-size="12" text-anchor="middle">Divergence Time</text>
            <text x="700" y="330" fill="#8b98ab" font-size="12" text-anchor="middle">Present</text>

            <!-- Tree Branches -->
            <g stroke="#a855f7" stroke-width="3" fill="none" filter="url(#neonGlowGreen)">
              <path class="branch" d="M100 175 L250 175"/>
              <path class="branch" d="M250 100 L250 250"/>
              
              <!-- Top Clade -->
              <path class="branch" d="M250 100 L450 100"/>
              <path class="branch" d="M450 60 L450 140"/>
              <path class="branch" d="M450 60 L650 60"/>
              <path class="branch" d="M450 140 L650 140"/>
              
              <!-- Bottom Clade -->
              <path class="branch" d="M250 250 L380 250"/>
              <path class="branch" d="M380 200 L380 300"/>
              <path class="branch" d="M380 200 L650 200"/>
              <path class="branch" d="M380 300 L650 300"/>
            </g>

            <!-- Nodes (Glowing dots at branch points) -->
            <circle cx="250" cy="175" r="5" fill="#a855f7" class="node"/>
            <circle cx="250" cy="100" r="4" fill="#a855f7" class="node"/>
            <circle cx="250" cy="250" r="4" fill="#a855f7" class="node"/>
            <circle cx="450" cy="100" r="4" fill="#a855f7" class="node"/>
            <circle cx="380" cy="250" r="4" fill="#a855f7" class="node"/>

            <!-- Leaf Labels -->
            <g font-family="sans-serif" font-size="14" font-weight="700">
              <!-- B. sacra -->
              <text x="670" y="55" fill="#2ecc71">🌿 Boswellia sacra (Dhofar)</text>
              <text x="670" y="75" fill="#8b98ab" font-size="11" font-weight="400">High Boswellic Acids</text>

              <!-- B. frereana -->
              <text x="670" y="135" fill="#f39c12">🌿 Boswellia frereana (Somalia)</text>
              <text x="670" y="155" fill="#8b98ab" font-size="11" font-weight="400">Lupeol / Epilupeol</text>

              <!-- B. serrata -->
              <text x="670" y="195" fill="#3498db">🌿 Boswellia serrata (India)</text>
              <text x="670" y="215" fill="#8b98ab" font-size="11" font-weight="400">High O-acetyl-11-keto-β-boswellic acid</text>

              <!-- B. papyrifera -->
              <text x="670" y="295" fill="#8b98ab">🌿 Boswellia papyrifera (Ethiopia)</text>
              <text x="670" y="315" fill="#8b98ab" font-size="11" font-weight="400">Incensole Acetate Dominant</text>
            </g>
          </svg>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · POPULATION IMPACT
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-population" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#f39c12">
      <div class="modal-head-left">
        <span class="me">📊</span>
        <div><h3>Population Impact &amp; Conservation Assessment</h3><div class="kick">Johnson et al. (2025) · Journal of Arid Environments 229:105368</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Johnson, Said, Vahalík, et al. (Researchers)</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Rapid conservation assessment of <em>B. sacra</em> in Oman</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Dhofar Mountains, Oman</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Published 2025</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">To determine if the species faces widespread collapse</div></div>
      </div>

      <div class="info" style="--pop-color:#f39c12;">
        <h4>📉 Reassessing the "Collapse" Narrative</h4>
        <p>Recent research has indicated population declines and unsustainable exploitation of multiple <em>Boswellia</em> species, including the Somalian <em>B. sacra</em> populations. However, information on the Arabian populations was previously minimal and contradictory.</p>
        <p style="margin-top:10px;">The 2025 rapid assessment, covering at least <strong>3,465 km²</strong> of the Dhofar mountains, was conducted to predict if the same pattern of population collapse seen in other species is occurring in Oman.</p>
      </div>

      <div class="grid-2" style="margin-top:20px;">
        <div class="info" style="--pop-color:#2ecc71;">
          <h4>✅ Key Finding: Regeneration is Occurring</h4>
          <p>The study observed regeneration across almost all populations, with <strong>97% of transects including at least 10% small trees or saplings</strong>. The data <strong>do not currently indicate significant or widespread declines</strong> in <em>B. sacra</em> in Oman, as seen in other species. Population structures were variable, with both reverse-J shaped (healthy regeneration) and bell-shaped (declining) distributions observed locally.</p>
        </div>

        <div class="info" style="--pop-color:#e74c3c;">
          <h4>⚠️ Localized Threats Identified</h4>
          <p>Despite the overall healthy picture, threats varied geographically and included:</p>
          <ul style="padding-left:16px; font-size:.86rem; color:var(--muted);">
            <li><strong>Overgrazing:</strong> Especially by camels, prevalent across many populations.</li>
            <li><strong>Resin Overharvesting:</strong> Concentrated in specific heavily tapped areas.</li>
            <li><strong>Mining &amp; Infrastructure:</strong> Localized habitat disturbance.</li>
            <li><strong>Insect/Pest Attacks:</strong> Particularly on stressed trees.</li>
            <li><strong>Wind/Flooding:</strong> Extreme weather events.</li>
          </ul>
        </div>
      </div>

      <div class="info" style="margin-top:20px; --pop-color:#3498db;">
        <h4>🛡️ Management Recommendations</h4>
        <p>The authors conclude that while the situation is not catastrophic, improved socio-ecological management systems are needed to maintain this status. Key priorities include: <strong>research to elucidate drivers of population patterns</strong>, improved rangeland management, enhanced monitoring and management of resin tapping, and identification of potential additional reserves.</p>
        <p class="srcline">Source: Johnson, S., Bait Said, A., Vahalík, P., Karas, L., Sarrouf Willson, M., &amp; Bongers, F. (2025). <a href="https://doi.org/10.1016/j.jaridenv.2025.105368" target="_blank" rel="noopener">doi:10.1016/j.jaridenv.2025.105368</a> <span class="vf">verified</span></p>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · CLIMATE THREAT & RED LIST
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-climate" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#e74c3c">
      <div class="modal-head-left">
        <span class="me">🌡️</span>
        <div><h3>Threats, Evidence &amp; Conservation Status</h3><div class="kick">What is shown for <em>B. sacra</em> vs. related species · IUCN status</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Johnson et al. (2025) · Rijkers et al. (2006) · IUCN / RBGE summaries</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Tapping, grazing, pests, climate · and what is (not) yet shown</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Dhofar (Oman) · related species in the Horn of Africa</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Literature 1998–2025</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Keep Oman-specific findings separate from findings on other species</div></div>
      </div>

      <div class="grid-2" style="margin-bottom:20px">
        <div class="info" style="--pop-color:#2ecc71">
          <h4>🔎 What the Oman assessment found</h4>
          <p>Johnson et al. (2025) surveyed at least 3,465 km² of the Dhofar mountains and found regeneration in nearly all populations and <strong>no evidence of significant or widespread decline</strong>. They documented local threats: overgrazing (especially by camels), resin over-harvesting in heavily tapped areas, mining and infrastructure, pests on stressed trees, and wind or flood events. Management of grazing and tapping is recommended. See the Population Impact module. <span class="vf">verified</span></p>
        </div>

        <div class="info" style="--pop-color:#f39c12">
          <h4>🌿 Evidence from a related species (<em>B. papyrifera</em>)</h4>
          <p>In Eritrea, intensive tapping of <em>B. papyrifera</em> lowered seed quality. At one site, germination was about 90% for untapped trees, 60% for normally tapped trees and 40% for heavily tapped trees; at three annually tapped sites it was 13–16%, versus 80–94% at two untapped sites (Rijkers et al., 2006). <strong>These are findings for <em>B. papyrifera</em>.</strong> Whether Dhofari <em>B. sacra</em> responds the same way is not shown here. <span class="vf">verified</span></p>
        </div>
      </div>

      <div class="grid-3">
        <div class="info" style="--pop-color:#e74c3c">
          <h4>📋 Red List status</h4>
          <p><em>B. sacra</em> is listed <strong>Near Threatened</strong> (IUCN assessment from 1998, now dated). Draft assessments from 2024, still pending review, rate <em>B. papyrifera</em> and <em>B. frereana</em> as Vulnerable. Endangered ratings apply to some other <em>Boswellia</em> species, mostly Socotran endemics (under review). Source: RBGE review of <em>Boswellia</em> conservation status. <span class="vf">verified</span></p>
        </div>

        <div class="info" style="--pop-color:#3498db">
          <h4>☀️ Monsoon &amp; climate</h4>
          <p>Dhofar’s summer monsoon fog (Khareef) shapes local habitats, and changing rainfall could matter for the species. This atlas does <strong>not</strong> cite a quantified climate effect on <em>B. sacra</em> <span class="nv">no source cited</span>.</p>
        </div>

        <div class="info" style="--pop-color:#2ecc71">
          <h4>🛡️ Management options</h4>
          <p>The Oman assessment recommends better rangeland management, monitoring and management of resin tapping, and additional reserves. Fenced nurseries and tapping rest periods are commonly proposed, but the rest period <em>B. sacra</em> needs is not established in the sources cited here.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · SCRIPTURAL
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-scriptural" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#9b59b6">
      <div class="modal-head-left">
        <span class="me">📖</span>
        <div><h3>Scriptural &amp; Prophetic Matrix</h3><div class="kick">Torah · Bible · Islamic tradition</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Moses (Musa) · Solomon (Sulaiman) &amp; Sheba · the Magi · Jewish, Christian &amp; Muslim communities</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Scriptural, liturgical, royal and medicinal use</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Sinai · Jerusalem · Southern Arabia · Bethlehem</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Traditional biblical dates → present</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Worship, kingship, purification</div></div>
      </div>
      <div class="grid-3">
        <div class="info">
          <h4>🕎 In the Torah</h4>
          <p>Hebrew <strong>levonah</strong>. Exodus 30:34–38 instructs Moses (<em>Musa</em> in Islamic tradition) to prepare a sacred incense (<em>ketoret</em>) from stacte, onycha, galbanum and pure frankincense, reserved for the Tabernacle. Leviticus 2:1–2 places frankincense on grain offerings. <a href="https://www.biblegateway.com/passage/?search=Exodus+30%3A34-38&amp;version=NIV" target="_blank" rel="noopener" class="cite">[Ex 30]</a> <a href="#ref-bible" class="cite">[1]</a></p>
        </div>
        <div class="info">
          <h4>✝️ In the New Testament</h4>
          <p>Matthew 2:11 says the Magi brought <strong>gold, frankincense and myrrh</strong> to the child Jesus (<em>‘Isa</em> in Islamic tradition). The familiar readings (gold for kingship, frankincense for divinity or priesthood, myrrh for mortality) come from later Christian interpretation, not from the verse itself. <a href="https://www.biblegateway.com/passage/?search=Matthew+2%3A11&amp;version=NIV" target="_blank" rel="noopener" class="cite">[Mt 2:11]</a> <a href="#ref-bible" class="cite">[1]</a></p>
        </div>
        <div class="info">
          <h4>☪️ In Islamic Tradition</h4>
          <p>Frankincense (<em>luban</em>) is <strong>not named in the Qur’an</strong>. The Qur’an mentions a gift sent by the Queen of Sheba to Sulaiman (Solomon) without naming its contents (<a href="https://quran.com/27/35" target="_blank" rel="noopener" class="cite">27:35</a>). Burning <em>bakhoor</em> is a widespread custom in Muslim households, and classical Islamic medical writing, including Prophetic-medicine texts such as Ibn al-Qayyim’s, discusses frankincense as a remedy <span class="nv">cite exact passage</span> <a href="#ref-ibn" class="cite">[2]</a></p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · ETYMOLOGY
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-etymology" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#f39c12">
      <div class="modal-head-left">
        <span class="me">💎</span>
        <div><h3>Etymology &amp; “Worth More Than Gold”</h3><div class="kick">Naming origins &amp; Roman economics</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Old French &amp; Latin speakers · Semitic traders</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Name from franc + incens; L-B-N root for “milky white”</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Europe · Arabia · Levant</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">1st c. BCE → modern English</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">How the name arose; why the resin was so prized</div></div>
      </div>
      <div class="grid-2">
        <div class="info">
          <h4>📝 Origin of the Name</h4>
          <p><strong>Frankincense</strong> — Old French <em>franc encens</em>, meaning “noble incense” or “pure incense.”</p>
          <p><strong>Luban (Arabic) / Levonah (Hebrew)</strong> — from the ancient Semitic root <strong>L-B-N</strong>, meaning “milky white,” referring to the fresh milky sap oozing from bark cuts.</p>
        </div>
        <div class="info">
          <h4>💰 Why “Worth More Than Gold”?</h4>
          <ul>
            <li><strong>Limited sources</strong> — concentrated in southern Arabia and the Horn of Africa.</li>
            <li><strong>Heavy ritual demand</strong> — burned in Egyptian, Greek, Roman and Jewish temple rites.</li>
            <li><strong>Long, taxed caravan route</strong> — Pliny describes 65 stages from Thomna to Gaza, with tithes and charges along the way (NH 12.32).</li>
            <li><strong>Prices in perspective</strong> — Pliny lists frankincense at 3–6 denarii per pound by quality (NH 12.65) and makes no comparison with gold, so “worth more than gold” is better read as a statement of sacred prestige than of market price.</li>
            <li><strong>Funeral extravagance</strong> — Pliny says Nero burned more perfume in one day at Poppaea’s funeral than Arabia produces in a year (NH 12.83; perfumes in general, not frankincense specifically).</li>
          </ul>
          <p style="margin-top:8px"><em>(Pliny, Natural History 12.32, 12.65, 12.83; Groom, 1981)</em></p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · TIMELINE
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-timeline" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#27ae60">
      <div class="modal-head-left">
        <span class="me">⏳</span>
        <div><h3>Interactive Chronology</h3><div class="kick">6000 BCE → 2026 · click any era</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Nomads · priests · kings · merchants · scientists</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Thirteen eras from c. 6000 BCE to 2026</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Dhofar → Mesopotamia → Rome → today’s export hubs</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">c. 6000 BCE → 2026</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Every era has its own 5W summary below</div></div>
      </div>
      <div class="tl-strip" id="tlStrip" role="tablist"></div>
      <div class="tl-detail" id="tlDetail" aria-live="polite"></div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · HISTORY
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-history" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#d4af37">
      <div class="modal-head-left">
        <span class="me">📜</span>
        <div><h3>Historical Trade Route</h3><div class="kick">Dhofar → Petra → Gaza</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Nomads · southern Arabic states · Hadramis · Nabataeans</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Overland caravan route from Dhofar to the Mediterranean</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Dhofar → Shisr → Shabwa → Marib → Petra → Gaza</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">1st millennium BCE – 2nd c. CE (earlier use debated)</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Prized for worship and medicine; a high-value luxury commodity</div></div>
      </div>
      <div class="grid-2">
        <div class="info">
          <h4>👥 Who was involved?</h4>
          <p>The identity of the earliest traders is not fully known; distinctive flint types have been linked to Dhofar <span class="nv">needs source</span>. Later, the Hadrami state of Shabwa (Khor Rori/Sumhuram), indigenous Dhofari communities, Omani Arabs moving north-east from Yemen, and Parthian Persians all participated.</p>
          <h4 style="margin-top:12px">📦 What moved?</h4>
          <p>Frankincense and myrrh moved north; spices, textiles and silk arrived by ship from India and China. Shisr, in the desert interior north of Dhofar and often identified with the legendary city of Ubar, may have been a caravan hub.</p>
        </div>
        <div class="info">
          <h4>⭐ Why it mattered</h4>
          <p>Frankincense was prized for worship and medicine. Egyptian texts are often cited as calling incense the “sweat of the gods” <span class="nv">cite text</span>. Pliny’s own price list puts it well below gold.</p>
          <p>How large the earliest trade was is uncertain; the written evidence is much later. Pliny (NH 12.32) describes the route from Thomna, capital of the Gebbanitae, to Gaza as <strong>65 stages</strong> with halts for camels (about 1,487 Roman miles).</p>
          <h4 style="margin-top:12px">📍 Where it landed</h4>
          <p>Caravans reached Shabwa, Marib, Petra and Gaza, with Alexandria as a maritime outlet.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · TRADE TODAY
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-trade" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#3498db">
      <div class="modal-head-left">
        <span class="me">🚢</span>
        <div><h3>Present-Day Trade Matrix · 2025–2026</h3><div class="kick">RO 471,400 in Oman exports</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Omani exporters · Saudi, Somali, UAE importers</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">RO 471,400 in frankincense exports (2025)</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Oman → Saudi Arabia · Somalia · UAE</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">2025 – 2026</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Regional perfume, ritual and wellness demand</div></div>
      </div>
      <div class="stats-grid">
        <div class="stat"><div class="num">RO 471.4k</div><div class="lbl">Total Oman exports · 2025</div><div class="src">Oman Observer, 2026</div></div>
        <div class="stat"><div class="num">RO 150.9k</div><div class="lbl">Saudi Arabia · #1</div><div class="src">Oman Observer, 2026</div></div>
        <div class="stat"><div class="num">RO 99.2k</div><div class="lbl">Somalia · #2</div><div class="src">Oman Observer, 2026</div></div>
        <div class="stat"><div class="num">RO 78.6k</div><div class="lbl">UAE · #3</div><div class="src">Oman Observer, 2026</div></div>
      </div>
      <div class="info" style="margin-top:18px">
        <h4>🌍 Global supply realities</h4>
        <p>Somalia, Ethiopia, and Oman dominate global supply. Somaliland exports lower grades of <em>B. sacra</em> (“beyo”) to Djibouti, Ethiopia and the Middle East, while higher grades (“meydi”, <em>B. frereana</em>) move to Saudi Arabia, the UAE and Yemen. Production remains labour-intensive and some populations face pressure from over-harvesting. On the IUCN Red List, <em>B. sacra</em> is Near Threatened (1998 assessment); draft assessments rate <em>B. papyrifera</em> and <em>B. frereana</em> Vulnerable. Trade-name details (“beyo”, “meydi”) are retained from the earlier draft <span class="nv">needs source</span>.</p>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · USES & HEALTH
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-uses" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#e74c3c">
      <div class="modal-head-left">
        <span class="me">⚕️</span>
        <div><h3>Human &amp; Veterinary Health Profiles</h3><div class="kick">Clinical Trials, Traditional Applications, &amp; Animal Health</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Human &amp; Veterinary Clinicians · Traditional Healers</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Boswellic acids (AKBA, KBA) · essential oils · extracts</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Global Veterinary Clinics · Human Hospitals · Arabia</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Antiquity → Modern Veterinary &amp; Human Medicine</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Traditional uses and proposed mechanisms (e.g., 5-LOX inhibition)</div></div>
      </div>

      <p style="color:var(--muted);font-size:.9rem;margin-bottom:20px;line-height:1.7">
        Each card pairs a traditional use with what research shows. <strong>Most clinical studies use <em>Boswellia serrata</em> (Indian frankincense) extracts, not <em>B. sacra</em> resin or incense smoke</strong>, so results should not be assumed to transfer. Evidence ratings are the atlas author’s summary of study design and quality, not clinical guidance.
      </p>

      <div class="health-grid">

        <div class="health-card" style="--hc:#a855f7">
          <div class="health-header">
            <div class="health-icon">🐾</div>
            <div>
              <h4>Veterinary &amp; Animal Health</h4>
              <div class="sub">Canine joint disease · Livestock wounds · Camel care</div>
            </div>
          </div>
          <div class="health-body">
            <div class="health-row">
              <div class="health-label trad">🏺 Traditional use</div>
              <p>Pastoralist communities are reported to have used resin on animal wounds and in remedies for camels <span class="nv">needs ethnographic source</span>.</p>
            </div>
            <div class="health-row">
              <div class="health-label mod">🔬 What research shows</div>
              <p><strong>Dogs:</strong> an open-label (uncontrolled) clinical study of <em>B. serrata</em> resin in dogs with joint and spinal disease reported improvement in clinical signs. Controlled evidence is limited. <strong>Horses &amp; livestock:</strong> Boswellia supplements are marketed for these animals, but controlled efficacy data are limited <span class="nv">needs source</span>.</p>
            </div>
            <div class="health-src">Species studied: <em>B. serrata</em>. Source: Reichling et al. (2004), <em>Schweiz. Arch. Tierheilkd.</em> <span class="nv">re-check details</span></div>
            <span class="evidence-badge preliminary">Evidence: Preliminary (open-label study)</span>
          </div>
        </div>

        <div class="health-card" style="--hc:#2ecc71">
          <div class="health-header">
            <div class="health-icon">🫁</div>
            <div>
              <h4>Respiratory &amp; Airways</h4>
              <div class="sub">Asthma · bronchitis · airway inflammation</div>
            </div>
          </div>
          <div class="health-body">
            <div class="health-row">
              <div class="health-label trad">🏺 Traditional use</div>
              <p>Frankincense resin burned or inhaled for <strong>cough, bronchial congestion and asthma</strong>. Used in Unani and Ayurvedic practice as a lung tonic.</p>
            </div>
            <div class="health-row">
              <div class="health-label mod">🔬 What research shows</div>
              <p>Boswellic acids inhibit <strong>5-lipoxygenase (5-LOX)</strong> in laboratory studies, an enzyme in leukotriene pathways relevant to airway inflammation. Small clinical studies of <em>B. serrata</em> extract in asthma have been reported, but they are limited in size and quality, and the effect on lung function remains unconfirmed.</p>
            </div>
            <div class="health-src">Species studied: <em>B. serrata</em>. Sources: Safayhi et al. (1992) (5-LOX mechanism); Moussaieff &amp; Mechoulam (2009) (review).</div>
            <span class="evidence-badge preliminary">Evidence: Preliminary (mechanistic + small trials)</span>
          </div>
        </div>

        <div class="health-card" style="--hc:#3498db">
          <div class="health-header">
            <div class="health-icon">🦷</div>
            <div>
              <h4>Oral &amp; Dental Health</h4>
              <div class="sub">Gingivitis · oral hygiene</div>
            </div>
          </div>
          <div class="health-body">
            <div class="health-row">
              <div class="health-label trad">🏺 Traditional use</div>
              <p>Resin is traditionally chewed or steeped in water for oral hygiene and gum complaints.</p>
            </div>
            <div class="health-row">
              <div class="health-label mod">🔬 What research shows</div>
              <p>A 2022 three-arm clinical study (60 adults with plaque-induced gingivitis, all given scaling and polishing) compared topical <em>B. serrata</em> <strong>gel</strong>, chlorhexidine gel and placebo gel over 21 days. Plaque, gingival and bleeding indices improved with both active gels versus placebo, with no significant difference between <em>B. serrata</em> and chlorhexidine. It was a small study of a <strong>gel, not a mouthwash</strong>, and the abstract does not describe randomization or blinding.</p>
            </div>
            <div class="health-src">Species studied: <em>B. serrata</em>. Source: Sonkusle et al. (2022), <em>World J Dent</em> 13(6):641–646, doi:10.5005/jp-journals-10015-2113 <span class="vf">verified</span></div>
            <span class="evidence-badge emerging">Evidence: Emerging (single small clinical study)</span>
          </div>
        </div>

        <div class="health-card" style="--hc:#f39c12">
          <div class="health-header">
            <div class="health-icon">🦴</div>
            <div>
              <h4>Inflammatory &amp; Joint Conditions</h4>
              <div class="sub">Osteoarthritis · joint stiffness</div>
            </div>
          </div>
          <div class="health-body">
            <div class="health-row">
              <div class="health-label trad">🏺 Traditional use</div>
              <p>Used for <strong>joint pain, rheumatic complaints and inflammatory conditions</strong>. Mentioned in classical Unani and Ayurvedic texts for joint stiffness.</p>
            </div>
            <div class="health-row">
              <div class="health-label mod">🔬 What research shows</div>
              <p>A 2020 systematic review and meta-analysis of <strong>7 randomized trials (545 participants)</strong> of Boswellia / <em>B. serrata</em> extracts in osteoarthritis found larger reductions in pain (VAS and WOMAC) and better function than control. The authors rated trial quality as generally medium to low, noted high heterogeneity, and advised caution. Proprietary <em>B. serrata</em> extracts such as 5-Loxin® and Aflapin® appear in the literature. AKBA is one of the suspected active constituents.</p>
            </div>
            <div class="health-src">Species studied: mostly <em>B. serrata</em>. Source: Yu et al. (2020), <em>BMC Complement Med Ther</em> 20:225, doi:10.1186/s12906-020-02985-6 <span class="vf">verified</span></div>
            <span class="evidence-badge moderate">Evidence: Moderate (RCTs; low–medium quality)</span>
          </div>
        </div>

        <div class="health-card" style="--hc:#9b59b6">
          <div class="health-header">
            <div class="health-icon">🎗️</div>
            <div>
              <h4>Oncology &amp; Cytotoxic Activity</h4>
              <div class="sub">Laboratory research only</div>
            </div>
          </div>
          <div class="health-body">
            <div class="health-row">
              <div class="health-label trad">🏺 Traditional use</div>
              <p>Incense smoke used in some traditional contexts as a protective and purifying agent; associated with spiritual healing.</p>
            </div>
            <div class="health-row">
              <div class="health-label mod">🔬 What research shows</div>
              <p>In cell-culture studies, AKBA and related boswellic acids induced apoptosis in several cancer cell lines (including glioblastoma, colon and bladder models) and affected NF-κB signalling. These are <strong>laboratory findings only</strong>. A few small clinical studies have examined brain-tumour oedema during radiotherapy, with inconclusive results. Boswellia is not an established cancer treatment.</p>
            </div>
            <div class="health-src">Species: <em>B. serrata</em> and <em>B. sacra</em> extracts (varies by study). Source: Moussaieff &amp; Mechoulam (2009) (review).</div>
            <span class="evidence-badge preliminary">Evidence: Preliminary (laboratory studies)</span>
          </div>
        </div>

        <div class="health-card" style="--hc:#e74c3c">
          <div class="health-header">
            <div class="health-icon">🧬</div>
            <div>
              <h4>Antimicrobial &amp; Antiseptic</h4>
              <div class="sub">Bacterial · fungal · wound care</div>
            </div>
          </div>
          <div class="health-body">
            <div class="health-row">
              <div class="health-label trad">🏺 Traditional use</div>
              <p>Resin applied to <strong>wounds, cuts and skin infections</strong>; burned to purify air in sickrooms; used as a gargle.</p>
            </div>
            <div class="health-row">
              <div class="health-label mod">🔬 What research shows</div>
              <p>Laboratory studies report antibacterial activity of frankincense oils and extracts, with results varying by species, oil composition and method. A study of <strong><em>B. sacra</em></strong> oil and smoke tested activity against pathogenic and airborne microbes (PubMed 37761150). Some animal studies report improved wound healing; human evidence is lacking.</p>
            </div>
            <div class="health-src">Species: <em>B. sacra</em> (oil and smoke study) and others. Sources: PubMed 37761150; Moussaieff &amp; Mechoulam (2009).</div>
            <span class="evidence-badge preliminary">Evidence: Preliminary (in-vitro + animal)</span>
          </div>
        </div>

      </div>

      <div class="caution">
        <strong>⚠️ Not medical or veterinary advice.</strong> Frankincense products can cause side effects and may not suit everyone, including people who are pregnant or taking other medicines. They do not replace diagnosis or treatment. Consult a qualified clinician or veterinarian before use.
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · BOTANICAL (UPDATED WITH PNG IMAGES)
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-botanical" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#27ae60">
      <div class="modal-head-left">
        <span class="me">🌿</span>
        <div><h3>Botanical Plates &amp; Resin Specimens</h3><div class="kick">Morphological &amp; Grading Profiling</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Miller &amp; Morris · Dhofari harvesters</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Tree habit · bark exudate · four grade specimens</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Dhofar plateau and escarpment</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Documented 1988 · ongoing observation</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Visual identification underpins grading and conservation</div></div>
      </div>

      <div class="info" style="margin-bottom:20px; --pop-color:#2ecc71;">
        <h4>🌳 Boswellia Sacra Morphology &amp; Resin Resinology</h4>
        <p><em>Boswellia sacra</em> Flueck. is a small, resin-bearing tree native to the Dhofar region of Oman. Below, tilt-enabled image cards illustrate its tree form, papery bark, resin exudation and trade grades. Images are secondary reproductions; confirm permissions and original sources before reuse.</p>
      </div>

      <!-- 4 BALANCED 3D CARDS USING LOCAL PNG IMAGES (5, 6, 7/7.1, 8) -->
      <div class="grid-2" style="margin-bottom:24px">
        
        <!-- CARD 5: THE TREE -->
        <div class="gal-card">
          <div class="frame holographic-3d-card">
            <span class="badge-i">Morphology 5 · Whole Tree</span>
            <img src="5.png" alt="Boswellia sacra tree at Wadi Dowkah" onerror="this.onerror=null; this.src='https://placehold.co/600x400/111318/d4af37?text=Image+5+Missing';" />
          </div>
          <div class="info-body">
            <div>
              <h5>🌳 5. Boswellia sacra Tree</h5>
              <p>A mature <em>Boswellia sacra</em> tree standing at Wadi Dowkah Natural Park in Dhofar, Oman. The species exhibits a thick trunk and a dense, sprawling canopy adapted to hyper-arid desert conditions.</p>
            </div>
            <div class="actions">
              <a href="https://www.gardendesign.com/holiday/frankincense.html" target="_blank" rel="noopener">Image source (secondary)</a>
            </div>
          </div>
        </div>

        <!-- CARD 6: BARK CLOSE-UP -->
        <div class="gal-card">
          <div class="frame holographic-3d-card">
            <span class="badge-i">Morphology 6 · Papery Bark &amp; Incision</span>
            <img src="6.png" alt="Close-up of Boswellia sacra bark" onerror="this.onerror=null; this.src='https://placehold.co/600x400/111318/d4af37?text=Image+6+Missing';" />
          </div>
          <div class="info-body">
            <div>
              <h5>📜 6. Bark Structure &amp; Resin Ducts</h5>
              <p>Close-up view of the smooth, papery, peeling bark of <em>Boswellia sacra</em>. Traditional incisions reveal the underlying cambium where resin ducts release protective oleo-gum-resin upon wounding.</p>
            </div>
            <div class="actions">
              <a href="https://www.gardendesign.com/holiday/frankincense.html" target="_blank" rel="noopener">Image source (secondary)</a>
            </div>
          </div>
        </div>

        <!-- CARD 7 & 7.1: DUAL RESIN EXUDATION -->
        <div class="gal-card">
          <div class="frame holographic-3d-card">
            <span class="badge-i">Resin 7 &amp; 7.1 · Exudation &amp; Tears</span>
            <div style="display:flex; width:100%; height:100%;">
              <img src="7.png" alt="Resin Exudation Close-up" style="width:50%; height:100%; object-fit:cover; border-right:1px solid var(--border);" onerror="this.onerror=null; this.src='https://placehold.co/600x400/111318/d4af37?text=7';" />
              <img src="7.1.png" alt="Frankincense Tears Dripping" style="width:50%; height:100%; object-fit:cover;" onerror="this.onerror=null; this.src='https://placehold.co/600x400/111318/d4af37?text=7.1';" />
            </div>
          </div>
          <div class="info-body">
            <div>
              <h5>💧 7 &amp; 7.1 Resin Exudation &amp; Tears</h5>
              <p>Close-up depiction of milky resin weeping from fresh tree incisions, followed by the hardening phase where droplets form translucent, aromatic frankincense "tears" along the bark.</p>
            </div>
            <div class="actions">
              <a href="https://www.researchgate.net/figure/Harvest-and-grading-of-B-sacra-gum-resins-a-Frankincense-tree-incision-and-tears-b_fig1_270529855" target="_blank" rel="noopener">Image source (ResearchGate)</a>
            </div>
          </div>
        </div>

        <!-- CARD 8: 4 RESIN GRADES -->
        <div class="gal-card">
          <div class="frame holographic-3d-card">
            <span class="badge-i">Grading 8 · 4 Harvest Grades</span>
            <img src="8.png" alt="Harvest and grading of B. sacra gum resins" onerror="this.onerror=null; this.src='https://placehold.co/600x400/111318/d4af37?text=Image+8+Missing';" />
          </div>
          <div class="info-body">
            <div>
              <h5>💎 8. Harvest Grades of B. sacra</h5>
              <p>Two classification schemes appear in the literature. This atlas uses the four regional trade categories (<strong>Hojari, Najdi, Shathari, Shaabi</strong>). The source figure labels its panels (b)–(e) with a different set of names (“Hougari Royal”, “Superior”, “Regular”, “Sha’bi”), where “Hougari” is a spelling of Hojari. Treat the panels as illustrating grades of resin, <strong>not</strong> as a one-to-one match with this atlas’s four categories <span class="nv">check original caption</span>.</p>
            </div>
            <div class="actions">
              <a href="https://www.researchgate.net/figure/Harvest-and-grading-of-B-sacra-gum-resins-a-Frankincense-tree-incision-and-tears-b_fig1_270529855" target="_blank" rel="noopener">Image source (ResearchGate)</a>
            </div>
          </div>
        </div>

      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · GENOMICS LAB (NEW)
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-genomics" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#a855f7">
      <div class="modal-head-left">
        <span class="me">🧬</span>
        <div><h3>Genomics Laboratory · DNA Matrix</h3><div class="kick">667.8 Mb Assembly · 18,564 Genes · Gypsy Retroelements</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Botanical geneticists · Bioinformatics teams</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">De novo genome assembly · gene-family analysis</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Arabian Peninsula · Horn of Africa · Global labs</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Genome published 2022 (<em>iScience</em>)</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Decode drought resilience &amp; resin biosynthesis</div></div>
      </div>

      <div class="info" style="margin-bottom:20px; --pop-color:#a855f7;">
        <h4>🧬 Genome Architecture &amp; Stress Adaptation
          <span class="layman-badge" onclick="openLayman('genomics')">
            <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2L14.5 9H22L16 13.5L18.5 21L12 16.5L5.5 21L8 13.5L2 9H9.5L12 2Z" fill="#a855f7" stroke="#d8b4fe" stroke-width="0.8"/></svg>
            Simple Summary
          </span>
        </h4>
        <p>The <em>Boswellia sacra</em> genome assembly spans <strong>667.8 Mb</strong> with <strong>18,564</strong> high-confidence protein-coding genes (Khan et al., 2022, <em>iScience</em> 25:104574) <span class="vf">verified</span>. The authors report a major expansion of <strong>Gypsy retroelements</strong> in roughly the last 2 million years; mobile DNA elements of this kind can reshape gene regulation. Claims that terpene-synthase and cytochrome P450 gene families are heavily duplicated, and that this drives resin chemistry, are retained from the earlier draft <span class="nv">check against paper</span>.</p>
      </div>

      <div class="gal-card" style="margin-bottom:20px;">
        <div class="frame" style="aspect-ratio:16/8; background:#05070a; position:relative; overflow:hidden;">
          <span class="badge-i">Plate VII · Genome concept diagram · Illustrative (not a real chromosome map)</span>
          <svg class="data-svg" viewBox="0 0 1000 400" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
            <defs>
              <linearGradient id="dnaGrad" x1="0%" y1="0%" x2="100%" y2="0%">
                <stop offset="0%" stop-color="#a855f7"/>
                <stop offset="50%" stop-color="#2ecc71"/>
                <stop offset="100%" stop-color="#3498db"/>
              </linearGradient>
            </defs>
            <rect width="1000" height="400" fill="#0a0c10"/>
            <g stroke="rgba(168,85,247,0.1)" stroke-width="1">
              <line x1="100" y1="40" x2="100" y2="360"/>
              <line x1="300" y1="40" x2="300" y2="360"/>
              <line x1="500" y1="40" x2="500" y2="360"/>
              <line x1="700" y1="40" x2="700" y2="360"/>
              <line x1="900" y1="40" x2="900" y2="360"/>
            </g>
            <text x="500" y="25" fill="#a855f7" font-size="14" text-anchor="middle" letter-spacing="2" font-weight="700">BOSWELLIA SACRA · 667.8 Mb · SCHEMATIC</text>
            <path d="M100 200 Q200 120 300 200 T500 200 T700 200 T900 200" fill="none" stroke="url(#dnaGrad)" stroke-width="4" filter="url(#neonGlowGreen)"/>
            <path d="M100 200 Q200 280 300 200 T500 200 T700 200 T900 200" fill="none" stroke="url(#dnaGrad)" stroke-width="4" opacity="0.6"/>
            <circle cx="300" cy="200" r="8" fill="#a855f7" class="node"/>
            <text x="300" y="170" fill="#a855f7" font-size="11" text-anchor="middle" font-weight="700">TPS Gene Cluster</text>
            <circle cx="500" cy="200" r="8" fill="#2ecc71" class="node"/>
            <text x="500" y="170" fill="#2ecc71" font-size="11" text-anchor="middle" font-weight="700">P450 Cytochromes</text>
            <circle cx="700" cy="200" r="8" fill="#3498db" class="node"/>
            <text x="700" y="170" fill="#3498db" font-size="11" text-anchor="middle" font-weight="700">Gypsy Retroelements</text>
            <text x="100" y="340" fill="#8b98ab" font-size="10">Region 1</text>
            <text x="300" y="340" fill="#8b98ab" font-size="10">Region 2</text>
            <text x="500" y="340" fill="#8b98ab" font-size="10">Region 3</text>
            <text x="700" y="340" fill="#8b98ab" font-size="10">Region 4</text>
            <text x="900" y="340" fill="#8b98ab" font-size="10">Region 5</text>
          </svg>
        </div>
      </div>

      <div class="grid-3">
        <div class="info" style="--pop-color:#a855f7">
          <h4>🧪 Terpene Synthase (TPS) Family</h4>
          <p>Terpene synthases (TPS) build the terpene molecules (such as α-pinene, myrcene and limonene) that contribute to resin aroma. Which TPS genes are expanded in <em>B. sacra</em> should be taken from the genome paper <span class="nv">needs source</span>.</p>
        </div>
        <div class="info" style="--pop-color:#2ecc71">
          <h4>🌡️ Drought-Responsive Genes</h4>
          <p>Drought tolerance is a theme of the genome analysis, but which gene families show signatures of selection should be taken from the paper itself <span class="nv">earlier DREB/NAC claim unverified</span>.</p>
        </div>
        <div class="info" style="--pop-color:#3498db">
          <h4>🔄 Gypsy Retroelement Legacy</h4>
          <p>Gypsy elements make up about 119.1 Mb of the assembly, and most intact copies were inserted within roughly the last 1.5 million years (Khan et al., 2022). Any link to arid adaptation is the authors’ interpretation <span class="vf">verified</span>.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · MICROBIOME (NEW)
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-microbiome" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#2ecc71">
      <div class="modal-head-left">
        <span class="me">🦠</span>
        <div><h3>Rhizosphere Microbiome Matrix</h3><div class="kick">Wild vs cultivated trees · fungal &amp; bacterial communities</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Soil microbiologists · Plant ecologists</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Bacterial &amp; fungal communities in root zone</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Wild and cultivated populations in Oman</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Study published 2017 (<em>PLOS ONE</em>)</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Compare root-zone communities of wild and cultivated trees</div></div>
      </div>

      <div class="info" style="margin-bottom:20px; --pop-color:#2ecc71;">
        <h4>🦠 Wild vs Cultivated Microbiome Divergence
          <span class="layman-badge" onclick="openLayman('microbiome')">
            <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2L14.5 9H22L16 13.5L18.5 21L12 16.5L5.5 21L8 13.5L2 9H9.5L12 2Z" fill="#a855f7" stroke="#d8b4fe" stroke-width="0.8"/></svg>
            Simple Summary
          </span>
        </h4>
        <p>Khan et al. (2017, <em>PLOS ONE</em>) found that the root zone of <strong>wild</strong> <em>B. sacra</em> is dominated by <strong>Ascomycota</strong> fungi (about 60%) and has higher <strong>Actinobacteria</strong> (about 27%), while <strong>cultivated</strong> trees shift toward <strong>Basidiomycota</strong> (about 52% in one population) with abundant <strong>Proteobacteria</strong> and <strong>Acidobacteria</strong>. The study measured <strong>higher glucosidase, cellulase and indole-3-acetic acid (IAA)</strong> in the rhizospheres of <strong>cultivated</strong> trees. What these differences mean for tree health is not established <span class="vf">verified</span>.</p>
      </div>

      <div class="gal-card" style="margin-bottom:20px;">
        <div class="frame" style="aspect-ratio:16/8; background:#05070a; position:relative; overflow:hidden;">
          <span class="badge-i">Plate VIII · Rhizosphere composition · Illustrative wedges</span>
          <svg class="data-svg" viewBox="0 0 1000 400" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
            <rect width="1000" height="400" fill="#0a0c10"/>
            <text x="250" y="40" fill="#2ecc71" font-size="16" text-anchor="middle" font-weight="700">WILD TREES</text>
            <text x="750" y="40" fill="#3498db" font-size="16" text-anchor="middle" font-weight="700">CULTIVATED TREES</text>
            <g transform="translate(250,220)">
              <circle r="120" fill="none" stroke="#2ecc71" stroke-width="2" opacity="0.4"/>
              <path d="M0,0 L0,-120 A120,120 0 0,1 103.9,60 Z" fill="#2ecc71" opacity="0.7"/>
              <path d="M0,0 L103.9,60 A120,120 0 0,1 -103.9,60 Z" fill="#f39c12" opacity="0.7"/>
              <path d="M0,0 L-103.9,60 A120,120 0 0,1 0,-120 Z" fill="#9b59b6" opacity="0.7"/>
              <text x="0" y="0" fill="#fff" font-size="14" text-anchor="middle" font-weight="700">Ascomycota 60%</text>
            </g>
            <g transform="translate(750,220)">
              <circle r="120" fill="none" stroke="#3498db" stroke-width="2" opacity="0.4"/>
              <path d="M0,0 L0,-120 A120,120 0 0,1 103.9,60 Z" fill="#3498db" opacity="0.7"/>
              <path d="M0,0 L103.9,60 A120,120 0 0,1 -103.9,60 Z" fill="#e74c3c" opacity="0.7"/>
              <path d="M0,0 L-103.9,60 A120,120 0 0,1 0,-120 Z" fill="#2ecc71" opacity="0.7"/>
              <text x="0" y="0" fill="#fff" font-size="14" text-anchor="middle" font-weight="700">Basidiomycota 52%</text>
            </g>
            <text x="500" y="380" fill="#8b98ab" font-size="11" text-anchor="middle">Wild: Ascomycota ~60%, more Actinobacteria · Cultivated: Basidiomycota ~52%, Proteobacteria &amp; Acidobacteria abundant · wedge sizes are schematic</text>
          </svg>
        </div>
      </div>

      <div class="grid-3">
        <div class="info" style="--pop-color:#2ecc71">
          <h4>🌱 IAA levels</h4>
          <p>IAA, a plant growth hormone also made by microbes, was higher in the rhizospheres of <strong>cultivated</strong> trees than wild ones (Khan et al., 2017).</p>
        </div>
        <div class="info" style="--pop-color:#f39c12">
          <h4>🔬 Enzyme Activity</h4>
          <p>Glucosidase and cellulase activities, which relate to the breakdown of plant material in soil, were also higher in <strong>cultivated</strong> rhizospheres (Khan et al., 2017).</p>
        </div>
        <div class="info" style="--pop-color:#3498db">
          <h4>🌍 Possible applications</h4>
          <p>Whether adding wild-type microbes could help nursery seedlings is a hypothesis; it has not been tested in the sources cited here.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · AI SATELLITE (NEW)
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-satellite" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#3498db">
      <div class="modal-head-left">
        <span class="me">🛰️</span>
        <div><h3>Satellite Mapping of Frankincense Trees</h3><div class="kick">WorldView-3 · spectral classification &amp; deep-learning detection</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Y. Al-Mulla (remote sensing, Oman)</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Spectral signature mapping + deep-learning tree detection</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Wadi Dawkah, Dhofar</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Published 2026 (<em>PLOS ONE</em>)</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Test whether satellite data can map and count the species</div></div>
      </div>

      <div class="info" style="margin-bottom:20px; --pop-color:#3498db;">
        <h4>🛰️ What the study did
          <span class="layman-badge" onclick="openLayman('satellite')">
            <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2L14.5 9H22L16 13.5L18.5 21L12 16.5L5.5 21L8 13.5L2 9H9.5L12 2Z" fill="#a855f7" stroke="#d8b4fe" stroke-width="0.8"/></svg>
            Simple Summary
          </span>
        </h4>
        <p>Al-Mulla (2026) measured the spectral signature of <em>B. sacra</em> in the field (350–2,500 nm), resampled it to <strong>WorldView-3</strong> bands, and classified imagery of Wadi Dawkah with the Spectral Angle Mapper (SAM), reaching <strong>93.7% overall accuracy (Kappa 0.87)</strong>. SAM clearly outperformed NDVI thresholding. Three deep-learning detectors were also tested for finding individual trees; the best (SSD) reached <strong>precision 0.83 and recall 0.93</strong> and matched 701 trees in validation, a count of validated detections and not a census. <strong>The 93.7% figure belongs to the SAM classification, not to deep learning.</strong> <span class="vf">verified</span></p>
      </div>

      <div class="gal-card" style="margin-bottom:20px;">
        <div class="frame" style="aspect-ratio:16/8; background:#05070a; position:relative; overflow:hidden;">
          <span class="badge-i">Plate IX · Detection overlay concept · Illustrative</span>
          <svg class="data-svg" viewBox="0 0 1000 400" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
            <rect width="1000" height="400" fill="#0a0c10"/>
            <g stroke="rgba(52,152,219,0.15)" stroke-width="1">
              <line x1="0" y1="100" x2="1000" y2="100"/>
              <line x1="0" y1="200" x2="1000" y2="200"/>
              <line x1="0" y1="300" x2="1000" y2="300"/>
              <line x1="200" y1="0" x2="200" y2="400"/>
              <line x1="400" y1="0" x2="400" y2="400"/>
              <line x1="600" y1="0" x2="600" y2="400"/>
              <line x1="800" y1="0" x2="800" y2="400"/>
            </g>
            <g>
              <circle cx="150" cy="120" r="30" fill="none" stroke="#2ecc71" stroke-width="2"/>
              <circle cx="150" cy="120" r="3" fill="#2ecc71"/>
              <text x="150" y="170" fill="#2ecc71" font-size="10" text-anchor="middle">Healthy</text>
              <circle cx="320" cy="180" r="28" fill="none" stroke="#2ecc71" stroke-width="2"/>
              <circle cx="320" cy="180" r="3" fill="#2ecc71"/>
              <circle cx="520" cy="140" r="35" fill="none" stroke="#f39c12" stroke-width="2"/>
              <circle cx="520" cy="140" r="3" fill="#f39c12"/>
              <text x="520" y="200" fill="#f39c12" font-size="10" text-anchor="middle">Stressed</text>
              <circle cx="720" cy="220" r="32" fill="none" stroke="#2ecc71" stroke-width="2"/>
              <circle cx="720" cy="220" r="3" fill="#2ecc71"/>
              <circle cx="880" cy="160" r="25" fill="none" stroke="#e74c3c" stroke-width="2"/>
              <circle cx="880" cy="160" r="3" fill="#e74c3c"/>
              <text x="880" y="210" fill="#e74c3c" font-size="10" text-anchor="middle">Dead</text>
              <circle cx="250" cy="300" r="26" fill="none" stroke="#2ecc71" stroke-width="2"/>
              <circle cx="250" cy="300" r="3" fill="#2ecc71"/>
              <circle cx="600" cy="320" r="30" fill="none" stroke="#2ecc71" stroke-width="2"/>
              <circle cx="600" cy="320" r="3" fill="#2ecc71"/>
            </g>
            <text x="500" y="30" fill="#3498db" font-size="14" text-anchor="middle" font-weight="700">ILLUSTRATIVE OVERLAY · NOT STUDY OUTPUT</text>
          </svg>
        </div>
      </div>

      <div class="grid-3">
        <div class="info" style="--pop-color:#2ecc71">
          <h4>🎯 What 93.7% means</h4>
          <p>Overall accuracy of the SAM classification (user’s accuracy 88.0%, producer’s accuracy 99.2%, Kappa 0.87). It is not the accuracy of the deep-learning detector.</p>
        </div>
        <div class="info" style="--pop-color:#3498db">
          <h4>📡 WorldView-3 Resolution</h4>
          <p>WorldView-3 panchromatic imagery is about 31 cm per pixel (sensor specification), fine enough to see crowns of larger trees. Species discrimination in the study relied on the spectral signature.</p>
        </div>
        <div class="info" style="--pop-color:#f39c12">
          <h4>🔭 Possible uses</h4>
          <p>The author concludes that field spectroscopy, high-resolution imagery and deep learning together could support monitoring in arid areas. Tree-health classes and repeat-pass change detection are possible future uses, not results reported here.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · CARBON BALANCE (NEW)
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-carbon" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#e67e22">
      <div class="modal-head-left">
        <span class="me">💨</span>
        <div><h3>Carbon Balance &amp; Physiological Ecology</h3><div class="kick">TNC Depletion · Stomatal Stress · Tapping Cost</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Plant physiologists · Ecophysiologists</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Total non-structural carbohydrates (TNC) dynamics</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">General plant physiology (B. sacra data to be cited)</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Concept summary</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Explain why tapping intensity and timing matter</div></div>
      </div>

      <div class="info" style="margin-bottom:20px; --pop-color:#e67e22;">
        <h4>💨 Resin Tapping Imposes a Carbon Cost
          <span class="layman-badge" onclick="openLayman('carbon')">
            <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2L14.5 9H22L16 13.5L18.5 21L12 16.5L5.5 21L8 13.5L2 9H9.5L12 2Z" fill="#a855f7" stroke="#d8b4fe" stroke-width="0.8"/></svg>
            Simple Summary
          </span>
        </h4>
        <p>Making resin and healing wounds costs the tree resources, and its stored carbohydrate reserves (<strong>total non-structural carbohydrates, TNC</strong>) can be drawn down. In hot, dry air, stomata close and photosynthesis slows, so recovery may be slower. These are general plant-physiology ideas. Measured TNC data for tapped and untapped <em>B. sacra</em> are <strong>not cited here</strong>, and the chart below is a concept sketch <span class="nv">B. sacra TNC data needed</span>. For a related species, intensive tapping reduced seed quality (Rijkers et al., 2006, <em>B. papyrifera</em>) <span class="vf">verified</span>.</p>
      </div>

      <div class="gal-card" style="margin-bottom:20px;">
        <div class="frame" style="aspect-ratio:16/8; background:#05070a; position:relative; overflow:hidden;">
          <span class="badge-i">Plate X · Reserve-depletion concept · Illustrative</span>
          <svg class="data-svg" viewBox="0 0 1000 400" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
            <rect width="1000" height="400" fill="#0a0c10"/>
            <g stroke="rgba(230,126,34,0.15)" stroke-width="1">
              <line x1="80" y1="50" x2="80" y2="350"/>
              <line x1="80" y1="350" x2="950" y2="350"/>
              <line x1="80" y1="250" x2="950" y2="250" stroke-dasharray="5 5"/>
              <line x1="80" y1="150" x2="950" y2="150" stroke-dasharray="5 5"/>
            </g>
            <text x="500" y="30" fill="#e67e22" font-size="14" text-anchor="middle" font-weight="700">ILLUSTRATIVE CONCEPT · NOT MEASURED DATA</text>
            <text x="40" y="200" fill="#8b98ab" font-size="12" text-anchor="middle" transform="rotate(-90 40 200)">TNC (relative)</text>
            <path d="M100 200 L200 195 L300 190 L400 188 L500 185 L600 183 L700 180 L800 178 L900 175" fill="none" stroke="#2ecc71" stroke-width="3" filter="url(#neonGlowGreen)"/>
            <text x="920" y="170" fill="#2ecc71" font-size="11">Untapped</text>
            <path d="M100 200 L200 220 L300 240 L400 255 L500 270 L600 285 L700 300 L800 310 L900 320" fill="none" stroke="#e74c3c" stroke-width="3" filter="url(#neonGlowCyan)"/>
            <text x="920" y="335" fill="#e74c3c" font-size="11">Tapped</text>
            <text x="100" y="375" fill="#8b98ab" font-size="10">Mar</text>
            <text x="300" y="375" fill="#8b98ab" font-size="10">May</text>
            <text x="500" y="375" fill="#8b98ab" font-size="10">Jul</text>
            <text x="700" y="375" fill="#8b98ab" font-size="10">Sep</text>
            <text x="900" y="375" fill="#8b98ab" font-size="10">Nov</text>
          </svg>
        </div>
      </div>

      <div class="grid-3">
        <div class="info" style="--pop-color:#e74c3c">
          <h4>🌡️ Atmospheric Drought</h4>
          <p>High vapor pressure deficit (VPD) forces stomatal closure, limiting photosynthesis regardless of soil moisture.</p>
        </div>
        <div class="info" style="--pop-color:#f39c12">
          <h4>🍂 Carbon-starvation hypothesis</h4>
          <p>Repeated tapping in hot, dry periods could deplete reserves faster than they are replenished. This is a hypothesis and has not been tested for <em>B. sacra</em> in the sources cited here.</p>
        </div>
        <div class="info" style="--pop-color:#2ecc71">
          <h4>⏳ Rest periods</h4>
          <p>How long <em>B. sacra</em> needs to recover between tapping cycles is not established in the sources cited here. For <em>B. papyrifera</em>, seed quality fell as tapping intensity rose (Rijkers et al., 2006).</p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · PROVENANCE AI (NEW)
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-provenance" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#d4af37">
      <div class="modal-head-left">
        <span class="me">🔍</span>
        <div><h3>Chemical Provenance &amp; Authentication</h3><div class="kick">Isoincensole Acetate · Species Fingerprinting · Origin Tracing</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Analytical chemists · Customs authorities · Perfumers</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Terpenic fingerprinting for origin &amp; species ID</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Global trade networks · Archaeological samples</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Methods under development</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Combat adulteration &amp; verify sacred provenance</div></div>
      </div>

      <div class="info" style="margin-bottom:20px; --pop-color:#d4af37;">
        <h4>🔍 Species-Specific Chemical Fingerprints
          <span class="layman-badge" onclick="openLayman('provenance')">
            <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2L14.5 9H22L16 13.5L18.5 21L12 16.5L5.5 21L8 13.5L2 9H9.5L12 2Z" fill="#a855f7" stroke="#d8b4fe" stroke-width="0.8"/></svg>
            Simple Summary
          </span>
        </h4>
        <p>Each <em>Boswellia</em> species has a characteristic terpenoid profile. <strong>Isoincensole acetate</strong> is reported as a marker shared by <em>B. sacra</em> and <em>B. carteri</em> (a name often treated as a synonym of <em>B. sacra</em>), while <strong>incensole</strong> and incensole acetate are especially abundant in <em>B. papyrifera</em> <span class="nv">cite</span>. Chemometric and machine-learning methods applied to GC-MS data are being explored for species and origin identification; accuracy depends on reference libraries and sample type.</p>
      </div>

      <div class="gal-card" style="margin-bottom:20px;">
        <div class="frame" style="aspect-ratio:16/8; background:#05070a; position:relative; overflow:hidden;">
          <span class="badge-i">Plate XI · Fingerprint concept diagram · Illustrative</span>
          <svg class="data-svg" viewBox="0 0 1000 400" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
            <rect width="1000" height="400" fill="#0a0c10"/>
            <text x="500" y="30" fill="#d4af37" font-size="14" text-anchor="middle" font-weight="700">ILLUSTRATIVE CONCEPT DIAGRAM</text>
            <g transform="translate(250,220)">
              <circle r="100" fill="none" stroke="#d4af37" stroke-width="2" opacity="0.4"/>
              <text x="0" y="-115" fill="#d4af37" font-size="12" text-anchor="middle" font-weight="700">B. sacra</text>
              <circle cx="0" cy="0" r="8" fill="#d4af37" class="node"/>
            </g>
            <g transform="translate(750,220)">
              <circle r="100" fill="none" stroke="#9b59b6" stroke-width="2" opacity="0.4"/>
              <text x="0" y="-115" fill="#9b59b6" font-size="12" text-anchor="middle" font-weight="700">B. papyrifera</text>
              <circle cx="0" cy="0" r="8" fill="#9b59b6" class="node"/>
            </g>
            <line x1="350" y1="220" x2="650" y2="220" stroke="#3498db" stroke-width="2" stroke-dasharray="8 6"/>
            <text x="500" y="205" fill="#3498db" font-size="11" text-anchor="middle">ML classifier</text>
            <text x="500" y="255" fill="#8b98ab" font-size="10" text-anchor="middle">Isoincensole acetate ↑</text>
            <text x="500" y="275" fill="#8b98ab" font-size="10" text-anchor="middle">Incensole ↑</text>
          </svg>
        </div>
      </div>

      <div class="grid-3">
        <div class="info" style="--pop-color:#d4af37">
          <h4>🧪 Isoincensole Acetate</h4>
          <p>Reported shared marker for <em>B. sacra</em> and <em>B. carteri</em>. A marker for the species, not by itself proof of Dhofari origin.</p>
        </div>
        <div class="info" style="--pop-color:#9b59b6">
          <h4>🧬 Incensole Marker</h4>
          <p>Abundant in <em>B. papyrifera</em>, which helps separate it from Arabian resins in many analyses; mixed or adulterated samples need more than one marker.</p>
        </div>
        <div class="info" style="--pop-color:#3498db">
          <h4>🤖 AI Classification</h4>
          <p>Machine-learning classifiers on GC-MS data are an active research area. No accuracy figure is cited here <span class="nv">needs source</span>.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · FUTURE LAB (NEW)
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-future" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#a855f7">
      <div class="modal-head-left">
        <span class="me">🚀</span>
        <div><h3>Future Research Frontiers</h3><div class="kick">Synthetic Biology · CRISPR · Climate-Adaptive Breeding</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Synthetic biologists · Conservation geneticists</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">CRISPR-edited drought tolerance · Yeast-based resin production</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Oman · global biotech labs</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">Speculative outlook, not a published roadmap</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Protect wild populations while meeting demand</div></div>
      </div>

      <div class="grid-3" style="margin-bottom:20px">
        <div class="info" style="--pop-color:#a855f7">
          <h4>🧬 CRISPR Drought Engineering
            <span class="layman-badge" onclick="openLayman('crispr')">
              <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2L14.5 9H22L16 13.5L18.5 21L12 16.5L5.5 21L8 13.5L2 9H9.5L12 2Z" fill="#a855f7" stroke="#d8b4fe" stroke-width="0.8"/></svg>
              Simple Summary
            </span>
          </h4>
          <p>Editing DREB and NAC transcription factor genes could enhance stomatal control and water-use efficiency in nursery seedlings before reintroduction to wild habitats.</p>
        </div>
        <div class="info" style="--pop-color:#2ecc71">
          <h4>🍞 Yeast-Based Resin Fermentation
            <span class="layman-badge" onclick="openLayman('fermentation')">
              <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2L14.5 9H22L16 13.5L18.5 21L12 16.5L5.5 21L8 13.5L2 9H9.5L12 2Z" fill="#a855f7" stroke="#d8b4fe" stroke-width="0.8"/></svg>
              Simple Summary
            </span>
          </h4>
          <p>Synthetic biology could engineer yeast to produce boswellic acids and incensole acetate, reducing pressure on wild trees while supplying pharmaceutical demand.</p>
        </div>
        <div class="info" style="--pop-color:#3498db">
          <h4>🌱 Climate-Adaptive Breeding
            <span class="layman-badge" onclick="openLayman('breeding')">
              <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M12 2L14.5 9H22L16 13.5L18.5 21L12 16.5L5.5 21L8 13.5L2 9H9.5L12 2Z" fill="#a855f7" stroke="#d8b4fe" stroke-width="0.8"/></svg>
              Simple Summary
            </span>
          </h4>
          <p>Marker-assisted selection for heat-tolerant genotypes could future-proof reforestation efforts as monsoon patterns shift under climate change.</p>
        </div>
      </div>

      <div class="gal-card">
        <div class="frame" style="aspect-ratio:16/8; background:#05070a; position:relative; overflow:hidden;">
          <span class="badge-i">Plate XII · Speculative research outlook · Illustrative</span>
          <svg class="data-svg" viewBox="0 0 1000 400" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
            <rect width="1000" height="400" fill="#0a0c10"/>
            <line x1="50" y1="200" x2="950" y2="200" stroke="#a855f7" stroke-width="3" opacity="0.4"/>
            <g>
              <circle cx="150" cy="200" r="12" fill="#2ecc71" class="node"/>
              <text x="150" y="170" fill="#2ecc71" font-size="12" text-anchor="middle" font-weight="700">2025</text>
              <text x="150" y="240" fill="#8b98ab" font-size="10" text-anchor="middle">Genome-wide SNP chip</text>
              <circle cx="350" cy="200" r="12" fill="#3498db" class="node"/>
              <text x="350" y="170" fill="#3498db" font-size="12" text-anchor="middle" font-weight="700">2027</text>
              <text x="350" y="240" fill="#8b98ab" font-size="10" text-anchor="middle">CRISPR field trials</text>
              <circle cx="550" cy="200" r="12" fill="#a855f7" class="node"/>
              <text x="550" y="170" fill="#a855f7" font-size="12" text-anchor="middle" font-weight="700">2030</text>
              <text x="550" y="240" fill="#8b98ab" font-size="10" text-anchor="middle">Yeast resin production</text>
              <circle cx="750" cy="200" r="12" fill="#f39c12" class="node"/>
              <text x="750" y="170" fill="#f39c12" font-size="12" text-anchor="middle" font-weight="700">2033</text>
              <text x="750" y="240" fill="#8b98ab" font-size="10" text-anchor="middle">Climate-adapted reforestation</text>
              <circle cx="920" cy="200" r="12" fill="#e74c3c" class="node"/>
              <text x="920" y="170" fill="#e74c3c" font-size="12" text-anchor="middle" font-weight="700">2035</text>
              <text x="920" y="240" fill="#8b98ab" font-size="10" text-anchor="middle">Sustainable trade certification</text>
            </g>
          </svg>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · REFERENCES
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-refs" aria-hidden="true">
  <div class="modal-card" role="dialog" aria-modal="true">
    <div class="modal-head" style="--pop-color:#8b98ab">
      <div class="modal-head-left">
        <span class="me">📚</span>
        <div><h3>APA 7th Sources &amp; Archaeological Citations</h3><div class="kick">Sources &amp; evidence notes</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body">
      <div class="fivew">
        <div class="w"><div class="wk">Who</div><div class="wv">Primary texts · peer-reviewed papers · UNESCO · Archaeological Reports</div></div>
        <div class="w"><div class="wk">What</div><div class="wv">Comprehensive Reference Index</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">Global academic &amp; heritage institutions</div></div>
        <div class="w"><div class="wk">When</div><div class="wv">1981 – 2026</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">Let readers check each claim; unverified items are flagged</div></div>
      </div>
      <p class="srcline" style="margin-bottom:14px">Legend: <span class="vf">verified</span> checked against the original record while preparing this version · <span class="ill">illustrative</span> conceptual graphic · <span class="nv">needs source</span> retained but not yet traced to a primary source.</p>

      <h4 class="ref-h">Peer-reviewed &amp; official sources</h4>
      <ol class="refs">
        <li>Johnson, S., Bait Said, A., Vahalík, P., Karas, L., Sarrouf Willson, M., &amp; Bongers, F. (2025). Rapid conservation assessment of <em>Boswellia sacra</em> in Oman reveals complex threat and population patterns. <em>Journal of Arid Environments, 229</em>, 105368. <a href="https://doi.org/10.1016/j.jaridenv.2025.105368" target="_blank" rel="noopener">https://doi.org/10.1016/j.jaridenv.2025.105368</a> <span class="vf">verified</span></li>
        <li>Khan, A. L., Al-Harrasi, A., Wang, J.-P., et al. (2022). Genome structure and evolutionary history of frankincense producing <em>Boswellia sacra</em>. <em>iScience, 25</em>(7), 104574. <a href="https://doi.org/10.1016/j.isci.2022.104574" target="_blank" rel="noopener">https://doi.org/10.1016/j.isci.2022.104574</a> <span class="vf">verified</span></li>
        <li>Khan, A. L., Asaf, S., Al-Rawahi, A., Lee, I.-J., &amp; Al-Harrasi, A. (2017). Rhizospheric microbial communities associated with wild and cultivated frankincense producing <em>Boswellia sacra</em> tree. <em>PLOS ONE, 12</em>(10), e0186939. <a href="https://doi.org/10.1371/journal.pone.0186939" target="_blank" rel="noopener">https://doi.org/10.1371/journal.pone.0186939</a> <span class="vf">verified</span></li>
        <li>Al-Mulla, Y. (2026). Spectral signature mapping and deep learning detection of Frankincense (<em>Boswellia sacra</em>) using WorldView-3 imagery. <em>PLOS ONE, 21</em>(8). <a href="https://doi.org/10.1371/journal.pone.0356056" target="_blank" rel="noopener">https://doi.org/10.1371/journal.pone.0356056</a> <span class="vf">verified</span></li>
        <li>Rijkers, T., Ogbazghi, W., Wessel, M., &amp; Bongers, F. (2006). The effect of tapping for frankincense on sexual reproduction in <em>Boswellia papyrifera</em>. <em>Journal of Applied Ecology, 43</em>, 1188–1195. <span class="vf">verified</span></li>
        <li>Yu, G., Xiang, W., Zhang, T., et al. (2020). Effectiveness of Boswellia and Boswellia extract for osteoarthritis patients: a systematic review and meta-analysis. <em>BMC Complementary Medicine and Therapies, 20</em>, 225. <a href="https://doi.org/10.1186/s12906-020-02985-6" target="_blank" rel="noopener">https://doi.org/10.1186/s12906-020-02985-6</a> <span class="vf">verified</span></li>
        <li>Sonkusle, S., Pattanashetti, J. I., Kalburgi, N. B., Patil, K. A., &amp; Singh, V. (2022). Comparative evaluation of topical application of <em>Boswellia serrata</em> gel with chlorhexidine gel in management of gingivitis: A clinical study. <em>World Journal of Dentistry, 13</em>(6), 641–646. <a href="https://doi.org/10.5005/jp-journals-10015-2113" target="_blank" rel="noopener">https://doi.org/10.5005/jp-journals-10015-2113</a> <span class="vf">verified</span></li>
        <li>Royal Botanic Garden Edinburgh. (n.d.). <em>Boswellia conservation status</em> (PADME project). <a href="https://padme.rbge.org.uk/boswellia/files/04%20Boswellia%20CONSERVATION%20STATUS.pdf" target="_blank" rel="noopener">padme.rbge.org.uk</a> <span class="vf">verified</span></li>
        <li>Oman Observer. (2026). <em>Satellite method identifies Dhofar frankincense with 93.7% accuracy</em>. <a href="https://www.omanobserver.om/article/1195355/oman/satellite-method-identifies-dhofar-frankincense-with-937-accuracy" target="_blank" rel="noopener">omanobserver.om</a> <span class="vf">verified</span></li>
        <li>Oman Observer. (2026, April 27). <em>Oman’s frankincense exports reach RO 471,400 in 2025</em>. <a href="https://www.omanobserver.om/article/1188620/" target="_blank" rel="noopener">https://www.omanobserver.om/article/1188620/</a></li>
        <li>UNESCO World Heritage Centre. (2000). <em>Land of Frankincense</em> (World Heritage List No. 1010). <a href="https://whc.unesco.org/en/list/1010/" target="_blank" rel="noopener">https://whc.unesco.org/en/list/1010/</a></li>
        <li>Al-Harrasi, A., Al-Rawahi, A., &amp; Khan, A. L. (2019). <em>Biology of Genus Boswellia</em>. Springer Nature.</li>
        <li>Moussaieff, A., &amp; Mechoulam, R. (2009). Boswellia resin: From religious ceremonies to medical uses; a review of in-vitro and in-vivo studies. <em>Journal of Pharmacy and Pharmacology, 61</em>(10), 1281–1293.</li>
        <li>Safayhi, H., Mack, T., Sabieraj, J., Anazodo, M. I., Subramanian, L. R., &amp; Ammon, H. P. T. (1992). Boswellic acids: Novel, specific, nonredox inhibitors of 5-lipoxygenase. <em>Journal of Pharmacology and Experimental Therapeutics, 261</em>(3), 1143–1146.</li>
        <li>Reichling, J., et al. (2004). Dietary support with Boswellia resin in canine inflammatory joint and spinal disease. <em>Schweizer Archiv für Tierheilkunde, 146</em>, 71–79. <span class="nv">re-check details</span></li>
        <li>Arie, E., Rosen, B., &amp; Namdar, D. (2020). Cannabis and frankincense at the Judahite shrine of Arad. <em>Tel Aviv, 47</em>(1), 5–28. <span class="nv">re-check details</span></li>
        <li><em>Antimicrobial activity of frankincense (Boswellia sacra) oil and smoke against pathogenic and airborne microbes.</em> PubMed ID 37761150. <a href="https://pubmed.ncbi.nlm.nih.gov/37761150/" target="_blank" rel="noopener">pubmed.ncbi.nlm.nih.gov/37761150</a></li>
      </ol>

      <h4 class="ref-h">Classical, scriptural &amp; historical works</h4>
      <ol class="refs" start="19">
        <li>Pliny the Elder. <em>Natural History</em>, Book XII (chs. 32, 65, 83). English translation as hosted at <a href="https://www.attalus.org/pliny/hn12b.html" target="_blank" rel="noopener">attalus.org</a> <span class="vf">verified</span></li>
        <li>Herodotus. <em>Histories</em>, Book III (on Arabian frankincense and the winged serpents).</li>
        <li>Casson, L. (1989). <em>The Periplus Maris Erythraei</em>. Princeton University Press.</li>
        <li id="ref-bible"><em>The Holy Bible</em> (New International Version). (2011). Zondervan. (Exodus 30:34–38; Leviticus 2:1–2; 1 Kings 10:1–10; Matthew 2:11.) Online: <a href="https://www.biblegateway.com/" target="_blank" rel="noopener">BibleGateway</a>.</li>
        <li id="ref-ibn">Ibn al-Qayyim al-Jawziyya. (1998). <em>Healing with the Medicine of the Prophet (Tibb al-Nabawi)</em> (A. A. al-Razi, Trans.). Dar al-Ghad al-Arabi. <span class="nv">cite exact passage on frankincense</span></li>
        <li>Groom, N. (1981). <em>Frankincense and Myrrh: A Study of the Arabian Incense Trade</em>. Longman.</li>
        <li>Miller, A. G., &amp; Morris, M. (1988). <em>Plants of Dhofar: The Southern Region of Oman</em>. Office of the Adviser for Conservation of the Environment, Diwan of Royal Court, Oman.</li>
      </ol>

      <h4 class="ref-h">Secondary &amp; context sources (images and background only)</h4>
      <ol class="refs" start="26">
        <li>Nabataea.net. (n.d.). <em>Al Balid Mosque</em>. <a href="https://nabataea.net/explore/cities_and_sites/al-balid-mosque/" target="_blank" rel="noopener">nabataea.net</a></li>
        <li>Acaia 61 Studio. (n.d.). <em>Baleed Fortress (Husn) conservation project</em>. <a href="https://www.a61s.it/en/lavori/projects/baleed-fortress-husn/sym_589" target="_blank" rel="noopener">a61s.it</a></li>
        <li>Garden Design. (n.d.). <em>Frankincense</em>. <a href="https://www.gardendesign.com/holiday/frankincense.html" target="_blank" rel="noopener">gardendesign.com</a> (source of tree and bark images; confirm permissions).</li>
        <li>Figure “Harvest and grading of <em>B. sacra</em> gum resins”. <a href="https://www.researchgate.net/figure/Harvest-and-grading-of-B-sacra-gum-resins-a-Frankincense-tree-incision-and-tears-b_fig1_270529855" target="_blank" rel="noopener">ResearchGate</a> <span class="nv">identify original publication</span></li>
      </ol>
    </div>
  </div>
</div>

<!-- GRADE INFO (secondary popup) -->
<div class="modal" id="m-grade-info" aria-hidden="true" style="z-index:2100">
  <div class="modal-card" role="dialog" aria-modal="true" style="max-width:680px">
    <div class="modal-head" id="gradeInfoHead">
      <div class="modal-head-left">
        <span class="me" id="gradeInfoEmoji">🔶</span>
        <div><h3 id="gradeInfoTitle">Grade</h3><div class="kick">Full profile</div></div>
      </div>
      <button class="modal-close" data-close>✕</button>
    </div>
    <div class="modal-body" id="gradeInfoBody"></div>
  </div>
</div>

<!-- ══════════════════════════════════════════════
     MODAL · LAYMAN SIMPLE SUMMARY (PURPLE STAR)
     ══════════════════════════════════════════════ -->
<div class="modal" id="m-layman" aria-hidden="true">
  <div class="modal-card layman-card" role="dialog" aria-modal="true">
    <div class="modal-head">
      <div class="modal-head-left">
        <span class="me" style="border-color:#a855f7;">⭐</span>
        <div>
          <h3 style="color:#c084fc;">Simple Summary</h3>
          <div class="kick" style="color:#a855f7;">Plain-language translation of the science</div>
        </div>
      </div>
      <button class="modal-close" onclick="closeLayman()">✕</button>
    </div>
    <div class="modal-body">
      <div class="layman-content" id="laymanContent">
        <!-- Content will be injected -->
      </div>
    </div>
  </div>
</div>

<script>
const REDUCED_MOTION = !!(window.matchMedia && window.matchMedia('(prefers-reduced-motion: reduce)').matches);
const FINE_POINTER = !!(window.matchMedia && window.matchMedia('(pointer:fine)').matches);

/* ============================================================
   0 · LAYMAN SIMPLE SUMMARY SYSTEM (PURPLE STAR)
   ============================================================ */
const LAYMAN_DATA = {
  origin: {
    title: "🔍 Origin & Discovery — Plain English",
    body: `
      <p><strong>What's the big deal?</strong> People in southern Arabia have used frankincense for a very long time. Exactly <em>when</em> it began is not firmly known; a date around 6000 BCE is often quoted, but it is an estimate.</p>
      <p><strong>What do we know for sure?</strong> Ancient Egyptians sent an expedition to a land called <strong>Punt</strong> (its location is debated) and carved pictures of incense trees being carried in baskets on Queen Hatshepsut's temple. Later, ports such as Sumhuram (Khor Rori) and Al-Baleed in Dhofar exported frankincense across the Indian Ocean.</p>
      <p><strong>Who wrote about it?</strong> The Roman writer Pliny the Elder described a camel route of <strong>65 stages</strong> from Thomna to Gaza and listed frankincense prices of 3–6 denarii per pound. "Worth more than gold" is a popular saying; Pliny himself does not compare the two.</p>
      <p><em>In short:</em> Frankincense is one of the oldest and most prized aromatics in history, and Dhofar in Oman is one of its famous sources.</p>
    `
  },
  resin: {
    title: "🌳 One Species, Four Grades — Plain English",
    body: `
      <p><strong>The surprising part:</strong> The four trade grades — Hojari, Najdi, Shathari and Shaabi — are all described as coming from the <em>same species</em> (<em>Boswellia sacra</em>). So why do they look and smell different?</p>
      <p><strong>Place, timing and handling all matter.</strong> The microclimate where a tree grows changes its resin chemistry, much as growing region changes wine. Harvest timing, how the tree is tapped, and how the resin is sorted also shape the grade. Whether genetic differences between populations play a part is still an open question.</p>
      <ul>
        <li><strong>Hojari (green):</strong> Associated with high, dry mountain sites. Pale, translucent, green-tinted tears.</li>
        <li><strong>Najdi (amber):</strong> From the hot desert plateau; described as more citrusy.</li>
        <li><strong>Shathari (golden):</strong> From dry valleys in the north-west; golden with bright citrus notes.</li>
        <li><strong>Shaabi (dark):</strong> From the misty coastal escarpment; darker and woodier.</li>
      </ul>
      <p><em>Zone details are indicative summaries, not exact boundaries.</em></p>
    `
  },
  archaeology: {
    title: "🏛️ Al-Baleed — Plain English",
    body: `
      <p><strong>What is Al-Baleed?</strong> It's an ancient port city in Oman (called Zafar back in the day) that was a major hub for the frankincense trade from the 8th to the 16th century CE. It's like the ancient version of a busy international airport — but for incense, spices, and luxury goods.</p>
      <p><strong>What's been found there?</strong> Archaeologists have uncovered four big landmarks:</p>
      <ul>
        <li><strong>🕌 The Grand Mosque:</strong> A huge mosque with 144 octagonal stone columns — one of the biggest in early Islamic Arabia.</li>
        <li><strong>🏰 The Fortress (Husn):</strong> A massive citadel where the governor lived, with secure storerooms for all that valuable resin.</li>
        <li><strong>🧱 The City Walls:</strong> A defensive wall with watchtowers and a moat to protect against desert raiders.</li>
        <li><strong>🌊 The Lagoon &amp; Dhows:</strong> A natural harbor where traditional wooden ships (dhows, including the Sambuk and Ghanja models) loaded frankincense and sailed all the way to India and China.</li>
      </ul>
      <p><strong>Why is it famous?</strong> It's a UNESCO World Heritage Site, and the Museum of the Frankincense Land there shows off scale models of the ancient ships and navigation tools like the <em>Kamal</em> that sailors used to ride the monsoon winds across the Indian Ocean.</p>
      <p><em>Think of Al-Baleed as the "Wall Street" of the ancient frankincense trade — where deals were made, taxes collected, and fortunes built.</em></p>
    `
  },
  biomarkers: {
    title: "🔬 Biomarkers — Plain English",
    body: `
      <p><strong>What are biomarkers?</strong> Chemical "fingerprints". Machines such as GC-MS can detect particular molecules that help show whether a sample is frankincense.</p>
      <p><strong>Which molecules?</strong> <strong>Incensole</strong> and <strong>incensole acetate</strong> are typical of some <em>Boswellia</em> species (especially <em>B. papyrifera</em>). <strong>AKBA</strong> is a boswellic acid studied for its biological activity. Which markers are present depends on the species and the sample.</p>
      <p><strong>Why is this useful?</strong> It can help archaeologists and traders check what a residue or product really contains.</p>
      <p><em>In short: chemical markers are clues, and are strongest when several point the same way.</em></p>
    `
  },
  paleoclimate: {
    title: "🌪️ Paleoclimate Proxies — Plain English",
    body: `
      <p><strong>What's a proxy?</strong> A natural "rain gauge" or "thermometer" that records past conditions.</p>
      <p><strong>How could it work?</strong> Plants take up slightly different forms of carbon and oxygen depending on how dry the air and soil are. Those ratios (δ¹³C and δ¹⁸O) are widely used in other plants to reconstruct past droughts.</p>
      <p><strong>What's the catch?</strong> A published, dated climate record from frankincense resin or wood is not cited in this atlas, so the chart is only a concept sketch.</p>
    `
  },
  thermal: {
    title: "🔥 Thermal Oxidation Products — Plain English",
    body: `
      <p><strong>What happens when you burn resin?</strong> Heat changes some molecules, creating new compounds such as <strong>incensole oxide</strong>.</p>
      <p><strong>Why does it matter?</strong> Finding heat-altered compounds in an ancient incense burner can support the idea that incense was burned there, rather than only stored.</p>
      <p><em>It is supporting evidence, not absolute proof.</em></p>
    `
  },
  genome: {
    title: "🧬 Genome Structure — Plain English",
    body: `
      <p><strong>What is a genome?</strong> It's the complete set of DNA instructions for a living thing — like a giant instruction manual for building and running a tree.</p>
      <p><strong>What did scientists find?</strong> They sequenced the entire genome of <em>Boswellia sacra</em> and found it has about <strong>667.8 million "letters"</strong> of DNA code and 18,564 genes. That's a lot!</p>
      <p><strong>What's interesting about it?</strong> The tree has a huge number of "jumping genes" called <strong>Gypsy retroelements</strong> — these are pieces of DNA that can copy themselves and move around the genome. Over the past 2 million years, these jumping genes have expanded a lot, and they've helped shape how the tree responds to stress (like drought).</p>
      <p><strong>Why does this matter?</strong> Understanding the genome helps scientists figure out which genes are responsible for producing the valuable resin compounds, and maybe even breed or protect trees that produce more or better resin.</p>
      <p><em>In short: the genome is the tree's "recipe book," and scientists are learning to read it.</em></p>
    `
  },
  genomics: {
    title: "🧬 Genomics Lab — Plain English",
    body: `
      <p><strong>What's a genome again?</strong> It's the complete instruction manual for a tree — every piece of DNA that tells it how to grow, make resin, and survive tough conditions.</p>
      <p><strong>What did scientists find?</strong> They sequenced the entire <em>Boswellia sacra</em> genome and found it has about <strong>667.8 million DNA "letters"</strong> and 18,564 genes. That's a big instruction manual!</p>
      <p><strong>The surprising discovery:</strong> Over the past 2 million years, a type of "jumping gene" called <strong>Gypsy retroelements</strong> has been copying and pasting itself all over the genome. This reshuffling helped the tree develop new ways to survive extreme drought.</p>
      <p><strong>Why does this matter?</strong> By knowing which genes control resin production and stress tolerance, scientists could eventually breed or engineer trees that produce more resin or survive harsher conditions — helping conservation and the industry at the same time.</p>
      <p><em>In short: the genome is the tree's recipe book, and we're finally learning to read it.</em></p>
    `
  },
  microbiome: {
    title: "🦠 Microbiome — Plain English",
    body: `
      <p><strong>What's a microbiome?</strong> The community of tiny organisms — bacteria and fungi — living around a tree's roots.</p>
      <p><strong>What did the study find?</strong> A 2017 study compared wild and cultivated frankincense trees in Oman. Wild trees had more of a fungus group called <strong>Ascomycota</strong> (about 60%) and more <strong>Actinobacteria</strong>. Cultivated trees had more <strong>Basidiomycota</strong> (about 52% in one population) and more <strong>Proteobacteria</strong> and <strong>Acidobacteria</strong>.</p>
      <p><strong>What about enzymes and hormones?</strong> The study measured <em>higher</em> activity of two soil enzymes and higher levels of the plant hormone IAA in the <strong>cultivated</strong> trees' root zones.</p>
      <p><em>In short: wild and farmed trees keep different microbial company. What that means for the trees is still unclear.</em></p>
    `
  },
  satellite: {
    title: "🛰️ Satellite Mapping — Plain English",
    body: `
      <p><strong>What's the challenge?</strong> Counting frankincense trees across rugged Dhofar on foot is slow.</p>
      <p><strong>What did the 2026 study do?</strong> It measured how frankincense leaves reflect light and used that "spectral signature" with very high-resolution WorldView-3 satellite images of Wadi Dawkah. A standard method (Spectral Angle Mapper) separated frankincense from other plants with <strong>93.7% overall accuracy</strong>.</p>
      <p><strong>And the AI?</strong> Separately, deep-learning models were tested to spot individual trees. The best one found trees with 83% precision and 93% recall.</p>
      <p><em>In short: satellites plus field measurements could make tree surveys faster. The 93.7% figure comes from the spectral method, not the AI.</em></p>
    `
  },
  carbon: {
    title: "💨 Carbon Balance — Plain English",
    body: `
      <p><strong>The idea:</strong> Making resin and healing cuts costs a tree energy. Trees store energy as carbohydrates, a bit like a savings account.</p>
      <p><strong>The worry:</strong> If tapping is heavy and the weather hot and dry, the tree may not be able to rebuild its reserves quickly. This is a general principle; measured data for <em>B. sacra</em> are not cited here.</p>
      <p><strong>What is known:</strong> In a related species (<em>B. papyrifera</em>), heavy tapping produced seeds that germinated much less often.</p>
      <p><em>How long B. sacra needs to rest between tappings is not established in the sources used here.</em></p>
    `
  },
  provenance: {
    title: "🔍 Provenance — Plain English",
    body: `
      <p><strong>What's provenance?</strong> Where something came from. Buyers often want to know whether resin is genuine and from where.</p>
      <p><strong>How do scientists check?</strong> Different <em>Boswellia</em> species have different mixtures of chemicals. Instruments like GC-MS can measure them.</p>
      <p><strong>What about AI?</strong> Machine-learning tools are being explored to read these chemical patterns. No accuracy figure is cited in this atlas.</p>
      <p><em>In short: chemical fingerprints help, but they are clues, not certificates.</em></p>
    `
  },
  crispr: {
    title: "🧬 CRISPR — Plain English",
    body: `
      <p><strong>What is CRISPR?</strong> It's a gene-editing tool that lets scientists make precise changes to DNA — like editing a typo in a document.</p>
      <p><strong>What could it do for frankincense?</strong> Researchers could edit genes that control how the tree responds to drought stress, potentially making seedlings better able to survive in harsh conditions.</p>
      <p><strong>Why is this important?</strong> Wild frankincense populations are threatened by climate change, over-harvesting, and habitat loss. CRISPR could help create hardier trees for reforestation efforts — but it raises ethical questions about engineering wild species.</p>
      <p><em>In short: a powerful tool that needs careful, responsible use.</em></p>
    `
  },
  fermentation: {
    title: "🍞 Yeast Fermentation — Plain English",
    body: `
      <p><strong>What's the idea?</strong> Instead of tapping wild trees for resin, scientists could engineer yeast — the same microbe used to make bread and beer — to produce the valuable compounds found in frankincense.</p>
      <p><strong>How would it work?</strong> Yeast could be given the genes for making <strong>boswellic acids</strong> (the anti-inflammatory compounds) and <strong>incensole acetate</strong> (the key aroma molecule). The yeast would then brew these compounds in large fermentation tanks.</p>
      <p><strong>Why does this matter?</strong> It could reduce pressure on wild tree populations while supplying the pharmaceutical and perfume industries with consistent, high-quality ingredients.</p>
      <p><em>In short: brewing frankincense in a lab could protect wild trees while meeting global demand.</em></p>
    `
  },
  breeding: {
    title: "🌱 Climate-Adaptive Breeding — Plain English",
    body: `
      <p><strong>What's the goal?</strong> To breed frankincense trees that can better survive the hotter, drier conditions expected under climate change.</p>
      <p><strong>How does it work?</strong> Scientists identify trees that naturally tolerate heat and drought, then use marker-assisted selection to breed those traits into nursery seedlings — without genetic engineering.</p>
      <p><strong>Why is this urgent?</strong> As monsoon patterns shift, traditional frankincense habitats may become unsuitable. Climate-adapted trees could help reforestation efforts succeed in a changing world.</p>
      <p><em>In short: using natural genetic variation to future-proof the frankincense tree.</em></p>
    `
  }
};

function openLayman(key) {
  const data = LAYMAN_DATA[key];
  if (!data) return;
  document.getElementById('laymanContent').innerHTML = `
    <h4 style="color:#c084fc;font-family:var(--font-title);margin-bottom:12px;font-size:1.1rem;">${data.title}</h4>
    ${data.body}
  `;
  const m = document.getElementById('m-layman');
  m.classList.add('show');
  m.setAttribute('aria-hidden', 'false');
  document.body.classList.add('modal-open');
}

function closeLayman() {
  const m = document.getElementById('m-layman');
  m.classList.remove('show');
  m.setAttribute('aria-hidden', 'true');
  if (!document.querySelector('.modal.show')) document.body.classList.remove('modal-open');
}

// Close layman on outside click
document.getElementById('m-layman').addEventListener('click', (e) => {
  if (e.target === document.getElementById('m-layman')) closeLayman();
});

/* ============================================================
   1 · AERIAL GIS MAP — with 3D close-up, tilt, and tree-level zoom
   ============================================================ */
let map;
let mapMarkers = {};

(function initMap(){
  const el = document.getElementById('map');
  if(!el || typeof L === 'undefined'){ if(el) el.innerHTML = '<p style="padding:24px;color:#8b98ab">The satellite map could not load (check your internet connection).</p>'; return; }

  map = L.map(el, { 
    scrollWheelZoom: true, 
    zoomControl: true,
    zoomSnap: 0.5,
    zoomDelta: 0.5
  }).setView([20, 48], 4);

  L.tileLayer('https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}', {
    attribution:'Tiles &copy; Esri — Source: Esri, Maxar, Earthstar Geographics',
    maxZoom: 18
  }).addTo(map);

  // Add a high-res satellite layer for close-up tree viewing
  L.tileLayer('https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}', {
    attribution: 'Esri World Imagery',
    maxZoom: 21,
    maxNativeZoom: 18
  }).addTo(map);

  function getStarSVG(color) {
    return `<svg class="star-svg" style="color:${color}" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
      <path d="M12 2 L14.6 9.2 L22 9.2 L16 13.7 L18.2 21 L12 16.8 L5.8 21 L8 13.7 L2 9.2 L9.4 9.2 Z" fill="${color}" stroke="#fff" stroke-width="1.5"/>
    </svg>`;
  }

  function makeMarkerHTML(color, label) {
    return `<div class="named-star">
      ${getStarSVG(color)}
      <span class="star-label">${label}</span>
    </div>`;
  }

  function namedIcon(color, label) {
    return L.divIcon({
      className: '',
      html: makeMarkerHTML(color, label),
      iconSize: [20, 20],
      iconAnchor: [10, 10],
      popupAnchor: [0, -10]
    });
  }

  // Tree-level markers with close-up popups
  mapMarkers.salalah = L.marker([17.015,54.092],{icon:namedIcon('#2ecc71', 'Salalah · Dhofar')}).addTo(map).bindPopup('<b>⭐ Salalah · Dhofar (Oman)</b><br>Primary habitat · Royal Hojari.<br><em>Zoom in to see individual trees.</em>');
  mapMarkers.wadiDawkah = L.marker([17.50,54.00],{icon:namedIcon('#2ecc71', 'Wadi Dawkah')}).addTo(map).bindPopup('<b>⭐ Wadi Dawkah / Nejd</b><br>Core frankincense park.<br><em>Zoom in for tree-level detail.</em>');
  mapMarkers.khorRori = L.marker([17.03,54.43],{icon:namedIcon('#2ecc71', 'Khor Rori')}).addTo(map).bindPopup('<b>⭐ Khor Rori (Sumhuram)</b><br>Ancient port.');
  mapMarkers.hasik = L.marker([17.75,55.25],{icon:namedIcon('#2ecc71', 'Hasik')}).addTo(map).bindPopup('<b>⭐ Hasik</b><br>Citrusy aroma.');
  mapMarkers.yemen = L.marker([14.5,47.5],{icon:namedIcon('#2ecc71', 'Hadramaut')}).addTo(map).bindPopup('<b>⭐ Hadramaut / Mahra</b><br>Yemen range.');
  mapMarkers.somalia = L.marker([10.4,45.0],{icon:namedIcon('#2ecc71', 'Somalia')}).addTo(map).bindPopup('<b>⭐ Northern Somalia</b><br>Major source.');

  mapMarkers.shisr = L.marker([18.25,53.65],{icon:namedIcon('#9b59b6', 'Shisr (Ubar)')}).addTo(map).bindPopup('<b>🌟 Shisr (Ubar)</b><br>Legendary caravan city.');
  mapMarkers.shabwa = L.marker([14.53,46.83],{icon:namedIcon('#9b59b6', 'Shabwa')}).addTo(map).bindPopup('<b>🌟 Shabwa</b><br>Hadrami state capital.');
  mapMarkers.marib = L.marker([15.46,45.33],{icon:namedIcon('#9b59b6', 'Marib')}).addTo(map).bindPopup('<b>🌟 Marib</b><br>Caravan node to Petra.');
  mapMarkers.petra = L.marker([30.33,35.44],{icon:namedIcon('#9b59b6', 'Petra')}).addTo(map).bindPopup('<b>🌟 Petra</b><br>Nabataean terminus.');
  mapMarkers.gaza = L.marker([31.50,34.47],{icon:namedIcon('#9b59b6', 'Gaza')}).addTo(map).bindPopup('<b>🌟 Gaza</b><br>Mediterranean outlet.');
  mapMarkers.rome = L.marker([41.90,12.50],{icon:namedIcon('#9b59b6', 'Rome')}).addTo(map).bindPopup('<b>🌟 Rome</b><br>Major historical consumer.');

  mapMarkers.saudi = L.marker([24.71,46.68],{icon:namedIcon('#3498db', 'Saudi Arabia')}).addTo(map).bindPopup('<b>🔷 Saudi Arabia</b><br>RO 150.9k in 2025.');
  mapMarkers.uae = L.marker([24.45,54.38],{icon:namedIcon('#3498db', 'UAE')}).addTo(map).bindPopup('<b>🔷 UAE</b><br>RO 78.6k in 2025.');
  
  L.polyline([[17.03,54.43],[18.25,53.65],[15.46,45.33],[14.53,46.83],[30.33,35.44],[31.50,34.47]],
    {color:'#9b59b6',weight:3,dashArray:'10 8',opacity:.9}).addTo(map).bindPopup('Historical Incense Road (Purple).');
  
  L.polyline([[17.015,54.092],[12.8,45.0],[28.0,34.0],[31.2,32.3],[41.90,12.50]],
    {color:'#3498db',weight:2.5,opacity:.8}).addTo(map).bindPopup('Modern maritime export.');

  // Add a "Close-up" control that zooms to tree level
  const closeUpControl = L.Control.extend({
    options: { position: 'topright' },
    onAdd: function() {
      const div = L.DomUtil.create('div', 'leaflet-bar leaflet-control');
      div.innerHTML = '<a href="#" title="Zoom to tree level" style="font-size:18px; display:grid; place-items:center; width:34px; height:34px; background:rgba(8,9,11,.9); color:#2ecc71; border:1px solid #2ecc71; border-radius:4px; text-decoration:none;">🌳</a>';
      div.onclick = (e) => {
        e.preventDefault();
        map.flyTo([17.015, 54.092], 16, { duration: 2 });
      };
      return div;
    }
  });
  map.addControl(new closeUpControl());

  // Add a "Tilt view" control
  const tiltControl = L.Control.extend({
    options: { position: 'topright' },
    onAdd: function() {
      const div = L.DomUtil.create('div', 'leaflet-bar leaflet-control');
      div.innerHTML = '<a href="#" title="Toggle 3D tilt view" style="font-size:18px; display:grid; place-items:center; width:34px; height:34px; background:rgba(8,9,11,.9); color:#d4af37; border:1px solid #d4af37; border-radius:4px; text-decoration:none;">⛰️</a>';
      div.onclick = (e) => {
        e.preventDefault();
        e.stopPropagation();
        const stage = document.getElementById('mapStage');
        stage.classList.toggle('tilted');
        setTimeout(() => map.invalidateSize(), 900);
      };
      return div;
    }
  });
  map.addControl(new tiltControl());

  setTimeout(() => map.invalidateSize(), 250);
})();

/* ============================================================
   1.1 · DHOFAR TERROIR & MICROCLIMATE MAP
   ============================================================ */
let terroirMap = null;
function initTerroirMap() {
  if (terroirMap) {
    terroirMap.invalidateSize();
    return;
  }
  const el = document.getElementById('terroirMap');
  if(!el || typeof L === 'undefined') return;

  terroirMap = L.map(el, {
    scrollWheelZoom: false,
    zoomControl: true,
    zoomSnap: 0.5,
    zoomDelta: 0.5
  }).setView([17.3, 54.1], 8);

  L.tileLayer('https://server.arcgisonline.com/ArcGIS/rest/services/World_Topo_Map/MapServer/tile/{z}/{y}/{x}', {
    attribution: 'Esri, USGS, NOAA'
  }).addTo(terroirMap);

  function zoneIcon(color, label) {
    return L.divIcon({
      className: '',
      html: `<div style="background:${color};color:#000;font-weight:700;font-size:10px;padding:3px 8px;border-radius:12px;border:1px solid #fff;box-shadow:0 0 8px ${color}">${label}</div>`,
      iconSize: [80, 20]
    });
  }

  L.circle([17.18, 54.65], { color: '#2ecc71', fillColor: '#2ecc71', fillOpacity: 0.35, radius: 22000 }).addTo(terroirMap)
    .bindPopup('<b>🟢 Hojari Terroir Zone</b><br>Jebel Samhan (800m-1500m)<br>Arid fog shadow, extreme stress.<br>High α-pinene → Royal Green.');

  L.circle([17.55, 54.05], { color: '#f39c12', fillColor: '#f39c12', fillOpacity: 0.35, radius: 25000 }).addTo(terroirMap)
    .bindPopup('<b>🟠 Najdi Terroir Zone</b><br>Nejd Desert Plateau (500m-900m)<br>Extreme desert heat & low humidity.<br>High myrcene → Amber/pale yellow.');

  L.circle([17.40, 53.40], { color: '#d4af37', fillColor: '#d4af37', fillOpacity: 0.35, radius: 24000 }).addTo(terroirMap)
    .bindPopup('<b>🟡 Shathari Terroir Zone</b><br>NW Dry Wadis (300m-600m)<br>Transitional limestone gravel.<br>High limonene → Golden yellow.');

  L.circle([17.02, 54.10], { color: '#8b98ab', fillColor: '#8b98ab', fillOpacity: 0.35, radius: 20000 }).addTo(terroirMap)
    .bindPopup('<b>⚫ Shaabi Terroir Zone</b><br>Coastal Fog Belt (50m-400m)<br>Heavy monsoon fog (Khareef), high moisture.<br>Large yield → Darker amber.');

  L.marker([17.18, 54.65], { icon: zoneIcon('#2ecc71', 'Hojari Zone') }).addTo(terroirMap);
  L.marker([17.55, 54.05], { icon: zoneIcon('#f39c12', 'Najdi Zone') }).addTo(terroirMap);
  L.marker([17.40, 53.40], { icon: zoneIcon('#d4af37', 'Shathari Zone') }).addTo(terroirMap);
  L.marker([17.02, 54.10], { icon: zoneIcon('#8b98ab', 'Shaabi Zone') }).addTo(terroirMap);
}

/* ============================================================
   2 · MODAL CONTROLLER
   ============================================================ */
const MODAL_TRIGGER = {};

function openModal(id){
  const m = document.getElementById('m-' + id);
  if(!m) return;
  document.querySelectorAll('.modal.show').forEach(x => {
    if(x.id !== 'm-grade-info' && x.id !== 'm-landmark-detail' && x.id !== 'm-layman') x.classList.remove('show');
  });
  m.classList.add('show');
  m.setAttribute('aria-hidden','false');
  document.body.classList.add('modal-open');
  m.scrollTop = 0;
  if(MODAL_TRIGGER[id]) requestAnimationFrame(() => MODAL_TRIGGER[id]());
}

function closeModal(m){
  m.classList.remove('show');
  m.setAttribute('aria-hidden','true');
  if(!document.querySelector('.modal.show')) document.body.classList.remove('modal-open');
}

document.querySelectorAll('[data-open]').forEach(btn => {
  btn.addEventListener('click', () => openModal(btn.dataset.open));
});

document.querySelectorAll('.modal').forEach(m => {
  m.addEventListener('click', e => { if(e.target === m) closeModal(m); });
  m.querySelectorAll('[data-close]').forEach(b => b.addEventListener('click', () => closeModal(m)));
});

document.addEventListener('keydown', e => {
  if(e.key === 'Escape'){
    const showing = document.querySelectorAll('.modal.show');
    if(showing.length){
      const last = showing[showing.length - 1];
      closeModal(last);
    }
  }
});

/* ============================================================
   2.1 · 3D INTERACTIVE TILT FOR ARCHAEOLOGY & BOTANICAL PNG CARDS
   ============================================================ */
document.querySelectorAll('.holographic-3d-card').forEach(card => {
  card.addEventListener('mousemove', (e) => {
    const rect = card.getBoundingClientRect();
    const x = e.clientX - rect.left - rect.width / 2;
    const y = e.clientY - rect.top - rect.height / 2;
    
    const rotateX = (-y / rect.height) * 16;
    const rotateY = (x / rect.width) * 16;
    
    card.style.transform = `perspective(1000px) rotateX(${rotateX}deg) rotateY(${rotateY}deg) scale(1.02)`;
  });

  card.addEventListener('mouseleave', () => {
    card.style.transform = `perspective(1000px) rotateX(0deg) rotateY(0deg) scale(1)`;
  });
});

/* ============================================================
   2.2 · LANDMARK HISTORICAL IMPORTANCE POPUP
   ============================================================ */
const LANDMARK_DETAILS = {
  1: {
    title: '1. The Grand Mosque (Al-Balid) Details',
    emoji: '🕌',
    color: '#d4af37',
    text: `<b>Historical Significance:</b> The Grand Mosque of Al-Baleed is one of Southern Arabia's largest and most significant early Islamic places of worship, spanning a floor plan of 1,732 m².<br><br>
    <b>Architectural Features:</b> Features a vast prayer hall supported by <strong>144 octagonal stone columns</strong>, an open courtyard, and elaborate ablution channels.<br><br>
    <b>Source Reference:</b> <a href="https://nabataea.net/explore/cities_and_sites/al-balid-mosque/" target="_blank" style="color:var(--gold);">Nabataea Archaeological Report</a>.`
  },
  2: {
    title: '2. Al-Baleed Fortress (Husn) Details',
    emoji: '🏰',
    color: '#f39c12',
    text: `<b>Historical Significance:</b> A monumental 3,623 m² multi-story citadel that served as the residence of the royal governor and military command center.<br><br>
    <b>Architectural Features:</b> Features thick stone curtain walls, elevated watchtowers, and secure subterranean storage chambers for high-value frankincense reserves.<br><br>
    <b>Source Reference:</b> <a href="https://www.a61s.it/en/lavori/projects/baleed-fortress-husn/sym_589" target="_blank" style="color:var(--gold);">Acaia 61 Studio Architecture Conservation Project</a>.`
  },
  3: {
    title: '3. Defensive City Walls & Moat Details',
    emoji: '🧱',
    color: '#3498db',
    text: `<b>Historical Significance:</b> Enclosed the landward borders of ancient Zafar to defend against hostile desert raids.<br><br>
    <b>Architectural Features:</b> Built with reinforced limestone blocks, watchtowers, and a flooded moat connected to the Khor lagoon.<br><br>
    <b>Source Reference:</b> UNESCO Land of Frankincense Archives No. 1010.`
  },
  4: {
    title: '4 & 4.1 Khor Lagoon & Omani Dhow Fleet Details',
    emoji: '🌊',
    color: '#2ecc71',
    text: `<b>Historical Significance:</b> Served as the natural sheltered deep-water harbor connecting Southern Arabia to India, China, and Africa.<br><br>
    <b>Maritime Fleet (Including 4.1 Sambuk / Dhow):</b> Accommodated traditional Omani vessels such as the <strong>Ghanja</strong>, <strong>Baghla</strong>, and the <strong>4.1 Sambuk Dhow</strong> which transported sacks of frankincense across the Indian Ocean.<br><br>
    <b>Source Reference:</b> <a href="https://whc.unesco.org/en/list/1010/" target="_blank" style="color:var(--gold);">UNESCO World Heritage Centre — Land of Frankincense</a>.`
  }
};

function openLandmarkDetail(num) {
  const data = LANDMARK_DETAILS[num];
  if(!data) return;
  document.getElementById('landmarkDetailTitle').textContent = data.title;
  document.getElementById('landmarkDetailEmoji').textContent = data.emoji;
  document.getElementById('landmarkDetailHead').style.setProperty('--pop-color', data.color);
  document.getElementById('landmarkDetailBody').innerHTML = `<div style="font-size:0.9rem;line-height:1.6;color:var(--text);">${data.text}</div>`;
  
  const m = document.getElementById('m-landmark-detail');
  m.classList.add('show');
  m.setAttribute('aria-hidden','false');
}

function closeLandmarkDetail() {
  const m = document.getElementById('m-landmark-detail');
  m.classList.remove('show');
  m.setAttribute('aria-hidden','true');
}

/* ============================================================
   3 · THREE.JS RESIN
   ============================================================ */
let resinBuilt = false;
let resinScene = null;

function tryBuildResin(){
  if(resinBuilt) return;
  const container = document.getElementById('resin-3d');
  if(!container) return;

  if(container.clientWidth < 50 || container.clientHeight < 50){
    requestAnimationFrame(tryBuildResin);
    return;
  }

  container.querySelectorAll('canvas').forEach(c => c.remove());

  const scene = new THREE.Scene();
  const camera = new THREE.PerspectiveCamera(42, container.clientWidth / container.clientHeight, 0.1, 100);
  camera.position.set(0, 0.5, 5.5);
  camera.lookAt(0, 0, 0);

  const renderer = new THREE.WebGLRenderer({ antialias:true, alpha:true });
  renderer.setPixelRatio(Math.min(window.devicePixelRatio, 2));
  renderer.setSize(container.clientWidth, container.clientHeight);
  renderer.shadowMap.enabled = true;
  container.appendChild(renderer.domElement);

  const controls = new THREE.OrbitControls(camera, renderer.domElement);
  controls.enableDamping = true;
  controls.dampingFactor = 0.1;
  controls.autoRotate = !REDUCED_MOTION;
  controls.autoRotateSpeed = 1.4;
  controls.minDistance = 3;
  controls.maxDistance = 9;
  controls.enablePan = false;

  scene.add(new THREE.AmbientLight(0xffffff, 0.55));
  const key = new THREE.DirectionalLight(0xf3e5ab, 2.2); key.position.set(4,6,5); scene.add(key);
  const rim = new THREE.DirectionalLight(0x88bbff, 1.1); rim.position.set(-5,2,-4); scene.add(rim);
  const fill = new THREE.PointLight(0xffd9a0, 0.9, 25); fill.position.set(0,-2,3); scene.add(fill);

  const geo = new THREE.IcosahedronGeometry(1.15, 4);
  const pos = geo.attributes.position;
  const v = new THREE.Vector3();
  for(let i = 0; i < pos.count; i++){
    v.fromBufferAttribute(pos, i);
    let y = v.y;
    if(y > 0) y *= 1.45;
    const noise = 1 + 0.13 * Math.sin(v.x*3.1) * Math.cos(v.z*2.7) + 0.07 * Math.sin(v.y*5.2 + v.x*2.4);
    pos.setXYZ(i, v.x*noise*0.95, y*noise*0.95, v.z*noise*0.95);
  }
  geo.computeVertexNormals();

  const mat = new THREE.MeshPhysicalMaterial({
    color:0x2ecc71, roughness:0.18, metalness:0,
    transmission:0.85, thickness:1.3, ior:1.52,
    clearcoat:0.9, clearcoatRoughness:0.15,
    emissive:0x2ecc71, emissiveIntensity:0.14
  });

  const mesh = new THREE.Mesh(geo, mat);
  scene.add(mesh);

  const glowGeo = new THREE.CircleGeometry(2.4, 48);
  const glowMat = new THREE.MeshBasicMaterial({ color:0x2ecc71, transparent:true, opacity:0.06 });
  const glow = new THREE.Mesh(glowGeo, glowMat);
  glow.position.z = -2;
  scene.add(glow);

  let t = 0;
  (function animate(){
    requestAnimationFrame(animate);
    t += 0.01;
    mesh.rotation.y += 0.006;
    mesh.rotation.x = Math.sin(t*0.5) * 0.08;
    mesh.position.y = Math.sin(t*0.7) * 0.06;
    controls.update();
    renderer.render(scene, camera);
  })();

  const colors = {
    hojari:   { hex:0x2ecc71, rough:0.15 },
    najdi:    { hex:0xf39c12, rough:0.22 },
    shathari: { hex:0xd4af37, rough:0.38 },
    shaabi:   { hex:0x8b98ab, rough:0.58 }
  };

  document.querySelectorAll('.grade-btn').forEach(btn => {
    btn.addEventListener('click', () => {
      document.querySelectorAll('.grade-btn').forEach(b => b.classList.remove('active'));
      btn.classList.add('active');
      const g = colors[btn.dataset.grade];
      if(!g) return;
      mat.roughness = g.rough;
      glow.material.color.setHex(g.hex);
      const start = mat.color.clone();
      const end = new THREE.Color(g.hex);
      let p = 0;
      const step = () => {
        p += 0.08;
        if(p >= 1){ mat.color.copy(end); mat.emissive.copy(end); return; }
        mat.color.copy(start).lerp(end, p);
        mat.emissive.copy(end).multiplyScalar(p * 0.15);
        requestAnimationFrame(step);
      };
      step();
    });
  });

  const onResize = () => {
    const w = container.clientWidth || 600;
    const h = container.clientHeight || 400;
    if(w < 10 || h < 10) return;
    camera.aspect = w / h;
    camera.updateProjectionMatrix();
    renderer.setSize(w, h);
  };
  window.addEventListener('resize', onResize);
  setTimeout(onResize, 100);
  setTimeout(onResize, 400);

  resinBuilt = true;
  resinScene = { resize: onResize };
}

MODAL_TRIGGER.resin = () => {
  requestAnimationFrame(() => {
    requestAnimationFrame(() => {
      tryBuildResin();
      initTerroirMap();
      buildTerroir3D();
      if(resinScene) setTimeout(() => resinScene.resize(), 150);
    });
  });
  setTimeout(() => {
    tryBuildResin();
    if(resinScene) resinScene.resize();
  }, 500);
};

/* ============================================================
   4 · TIMELINE — with interactive 3D map & symbolism
   ============================================================ */
const EVENTS = [
  { emoji:'🌿', when:'Earliest use (debated)', short:'Prehistory', color:'#8b98ab',
    who:'Prehistoric communities of southern Arabia',
    what:'Frankincense use begins in prehistory. The often-quoted c. 6000 BCE is an estimate, not an established date.',
    where:'Dhofar → southern Arabia',
    why:'Ritual, medicinal and elite demand.', cite:'Date estimates vary; see Sources',
    mapCenter:[17.0,54.1], mapZoom:7,
    symbolism:'🌿🌍', symbolLabel:'Prehistoric use',
    mapLabel:'Earliest use · date debated',
    mapLabelColor:'#8b98ab' },
  { emoji:'✍️', when:'c. 3200 BCE', short:'Writing appears', color:'#7f8c8d',
    who:'Early Mesopotamian scribes and traders',
    what:'Writing appears in Mesopotamia. How large any contemporary incense trade from Arabia was is uncertain.',
    where:'Southern Mesopotamia',
    why:'Context: later written sources document incense use.', cite:'Interpretive context; source needed',
    mapCenter:[25.0,50.0], mapZoom:5,
    symbolism:'✍️🏛️', symbolLabel:'Early writing',
    mapLabel:'Early writing · c. 3200 BCE',
    mapLabelColor:'#7f8c8d' },
  { emoji:'🕎', when:'c. 1440 BCE (traditional)', short:'Ketoret', color:'#9b59b6',
    who:'Moses (Musa); the Israelites',
    what:'A sacred incense containing pure frankincense is commanded for the Tabernacle.',
    where:'Sinai · Tabernacle',
    why:'Worship reserved to God alone; frankincense set apart as holy.', cite:'Exodus 30:34–38 (traditional dating)',
    mapCenter:[28.5,34.0], mapZoom:7,
    symbolism:'🕎✨', symbolLabel:'Sacred Ketoret incense',
    mapLabel:'Sacred Ketoret Incense · c. 1440 BCE',
    mapLabelColor:'#9b59b6' },
  { emoji:'👑', when:'c. 950 BCE (traditional)', short:'Sheba', color:'#8e44ad',
    who:'Queen of Sheba; King Solomon (Sulaiman)',
    what:'Royal gifts of frankincense and spices travel from Southern Arabia to Jerusalem.',
    where:'Southern Arabia → Jerusalem',
    why:'Diplomacy and prestige.', cite:'1 Kings 10:1–10',
    mapCenter:[20.0,44.0], mapZoom:6,
    symbolism:'👑🐪', symbolLabel:'Queen of Sheba\'s caravan',
    mapLabel:'Queen of Sheba\'s Caravan · c. 950 BCE',
    mapLabelColor:'#8e44ad' },
  { emoji:'⚓', when:'c. 300 BCE–2nd c. CE', short:'Ports flourish', color:'#d4af37',
    who:'Hadrami state of Shabwa; Sumhuram traders',
    what:'Sumhuram (Khor Rori) is founded and operates as a frankincense port; caravans reach Petra and Gaza.',
    where:'Khor Rori · Shabwa · Petra · Gaza',
    why:'Mediterranean temple and funerary demand.', cite:'UNESCO, 2000',
    mapCenter:[20.0,45.0], mapZoom:5,
    symbolism:'⚓🚢', symbolLabel:'Maritime incense ports',
    mapLabel:'Maritime Incense Ports · c. 300 BCE–2nd c. CE',
    mapLabelColor:'#d4af37' },
  { emoji:'⭐', when:'c. 5 BCE (traditional)', short:'Magi', color:'#e74c3c',
    who:'Wise Men from the East; the child Jesus (‘Isa)',
    what:'Gold, frankincense and myrrh are brought to Bethlehem.',
    where:'Bethlehem, Judaea',
    why:'Kingship, divine priesthood, and sacrifice.', cite:'Matthew 2:11',
    mapCenter:[31.7,35.2], mapZoom:8,
    symbolism:'⭐👶', symbolLabel:'The Magi\'s gifts',
    mapLabel:'The Magi\'s Gifts · c. 5 BCE',
    mapLabelColor:'#e74c3c' },
  { emoji:'🔥', when:'1st c. CE', short:'More than gold', color:'#c0392b',
    who:'Roman Empire; Nabataean and South Arabian traders',
    what:'Frankincense is a prized luxury in Rome. Pliny lists prices of 3–6 denarii per pound and describes a 65-stage route from Thomna to Gaza.',
    where:'Rome · Arabia',
    why:'Scarcity, tolls along a long caravan route, and heavy ritual demand.', cite:'Pliny, Natural History 12.32, 12.65',
    mapCenter:[38.0,25.0], mapZoom:4,
    symbolism:'🔥🏛️', symbolLabel:'A prized luxury',
    mapLabel:'A Prized Luxury · 1st c. CE',
    mapLabelColor:'#c0392b' },
  { emoji:'🕌', when:'8th–16th c. CE', short:'Al-Baleed', color:'#2ecc71',
    who:'Omani and Indian Ocean merchants',
    what:'Al-Baleed (Zafar) flourishes as a frankincense port.',
    where:'Al-Baleed, Dhofar',
    why:'Monsoon trade; Islamic ritual and perfume demand.', cite:'UNESCO, 2000',
    mapCenter:[17.0,54.1], mapZoom:9,
    symbolism:'🕌🌙', symbolLabel:'Islamic maritime trade',
    mapLabel:'Islamic Maritime Trade · 8th–16th c. CE',
    mapLabelColor:'#2ecc71' },
  { emoji:'📏', when:'20th century (date needs source)', short:'Trade grades', color:'#3498db',
    who:'Dhofari harvesting families; Salalah traders',
    what:'Traditional trade categories (Hojari, Najdi, Shathari, Shaabi) are described in the modern literature. When they were formalised is not sourced here.',
    where:'Salalah · Samhan · Nejd',
    why:'Market price differentiation.', cite:'Al-Harrasi et al., 2019',
    mapCenter:[17.0,54.1], mapZoom:9,
    symbolism:'📏💎', symbolLabel:'Commercial grading',
    mapLabel:'Trade Grades · 20th c.',
    mapLabelColor:'#3498db' },
  { emoji:'🏛️', when:'2000', short:'UNESCO listing', color:'#16a085',
    who:'UNESCO and the Sultanate of Oman',
    what:'Land of Frankincense inscribed as a World Heritage Site.',
    where:'Wadi Dawkah · Shisr · Khor Rori · Al-Baleed',
    why:'Heritage protection; conservation.', cite:'UNESCO, 2000',
    mapCenter:[17.5,54.0], mapZoom:8,
    symbolism:'🏛️🌍', symbolLabel:'UNESCO World Heritage',
    mapLabel:'UNESCO World Heritage Listing · 2000',
    mapLabelColor:'#16a085' },
  { emoji:'🔬', when:'2010s–2020s', short:'Science', color:'#2980b9',
    who:'Researchers (Al-Harrasi, Moussaieff et al.)',
    what:'GC-MS profiling and clinical trials on boswellic acids.',
    where:'Oman · Somalia · global laboratories',
    why:'Validate pharmacology.', cite:'Moussaieff & Mechoulam, 2009',
    mapCenter:[22.0,58.0], mapZoom:4,
    symbolism:'🔬🧪', symbolLabel:'Modern scientific validation',
    mapLabel:'Modern Scientific Validation · 2010s–2020s',
    mapLabelColor:'#2980b9' },
  { emoji:'⚠️', when:'1998 · 2024 drafts · 2025', short:'Conservation', color:'#e67e22',
    who:'IUCN; researchers in Oman',
    what:'B. sacra is listed Near Threatened (1998). Draft assessments rate B. papyrifera and B. frereana Vulnerable. A 2025 Oman survey found regeneration and no widespread decline.',
    where:'Horn of Africa · southern Arabia',
    why:'Over-harvesting, grazing and habitat pressure vary by place.', cite:'RBGE review; Johnson et al., 2025',
    mapCenter:[10.0,45.0], mapZoom:5,
    symbolism:'⚠️🌡️', symbolLabel:'Conservation status',
    mapLabel:'Conservation Status',
    mapLabelColor:'#e67e22' },
  { emoji:'🚢', when:'2025–2026', short:'RO 471,400', color:'#27ae60',
    who:'Omani exporters',
    what:'Exports reach RO 471,400; Saudi Arabia is top destination.',
    where:'Oman → Saudi Arabia · Somalia · UAE',
    why:'Regional demand across perfume, ritual, wellness.', cite:'Oman Observer, 2026',
    mapCenter:[22.0,50.0], mapZoom:5,
    symbolism:'🚢💰', symbolLabel:'Modern export economy',
    mapLabel:'Modern Export Economy · 2025–2026',
    mapLabelColor:'#27ae60' }
];

(function initTimeline(){
  const strip = document.getElementById('tlStrip');
  const detail = document.getElementById('tlDetail');
  if(!strip || !detail) return;

  EVENTS.forEach((ev, i) => {
    const b = document.createElement('button');
    b.type = 'button';
    b.className = 'tl-chip';
    b.setAttribute('role','tab');
    b.style.setProperty('--era', ev.color);
    b.innerHTML = `<span class="te">${ev.emoji}</span><span class="yr">${ev.when}</span><span class="sh">${ev.short}</span>`;
    b.addEventListener('click', () => select(i));
    strip.appendChild(b);
  });

  function select(i){
    Array.prototype.forEach.call(strip.children, (c,j) => {
      c.classList.toggle('active', j === i);
      c.setAttribute('aria-selected', j === i ? 'true' : 'false');
    });
    const ev = EVENTS[i];
    detail.style.setProperty('--era', ev.color);
    
    // Build the detail with an interactive mini-map and a labeled wrapper
    detail.innerHTML = `
      <div class="when"><span class="de">${ev.emoji}</span>${ev.when}</div>
      <div class="who">${ev.who}</div>
      <div class="tl-5w">
        <div class="w"><div class="wk">What</div><div class="wv">${ev.what}</div></div>
        <div class="w"><div class="wk">Where</div><div class="wv">${ev.where}</div></div>
        <div class="w"><div class="wk">Why</div><div class="wv">${ev.why}</div></div>
      </div>
      <div style="display:flex; align-items:center; gap:16px; margin:14px 0; flex-wrap:wrap;">
        <div style="display:flex; align-items:center; gap:10px; background:rgba(0,0,0,.3); border:1px solid var(--border); border-radius:12px; padding:8px 16px;">
          <span style="font-size:2.2rem; filter:drop-shadow(0 0 12px ${ev.color});">${ev.symbolism}</span>
          <span style="font-size:.85rem; color:${ev.color}; font-weight:600;">${ev.symbolLabel}</span>
        </div>
        <div class="tl-map-wrapper">
          <div class="tl-map-label">
            <span class="lbl-dot" style="background:${ev.mapLabelColor}; box-shadow:0 0 6px ${ev.mapLabelColor};"></span>
            ${ev.mapLabel}
          </div>
          <div id="tlMap-${i}" style="width:100%; height:100%;"></div>
        </div>
      </div>
      <p style="font-size:.74rem;color:var(--muted);font-style:italic;margin:0">(${ev.cite})</p>
    `;

    // Create the mini-map after the DOM is updated
    setTimeout(() => {
      const mapEl = document.getElementById('tlMap-' + i);
      if (!mapEl) return;
      // Remove any existing map
      if (mapEl._leaflet_id) {
        const oldMap = mapEl._leaflet_map;
        if (oldMap) {
          oldMap.flyTo(ev.mapCenter, ev.mapZoom, { duration: 1.5 });
          oldMap.invalidateSize();
          return;
        }
      }
      if (typeof L === 'undefined') return;
      const miniMap = L.map(mapEl, {
        zoomControl: false,
        attributionControl: false,
        scrollWheelZoom: false,
        dragging: true,
        touchZoom: true,
        doubleClickZoom: true,
        boxZoom: false,
        keyboard: false,
        zoomSnap: 0.5,
        zoomDelta: 0.5
      }).setView(ev.mapCenter, ev.mapZoom);

      // Satellite base
      L.tileLayer('https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}', {
        maxZoom: 18
      }).addTo(miniMap);

      // Add a glowing circle at the center
      L.circle(ev.mapCenter, {
        color: ev.color,
        fillColor: ev.color,
        fillOpacity: 0.15,
        radius: 80000,
        weight: 2,
        dashArray: '6 4'
      }).addTo(miniMap);

      // Add a star marker at the center
      const starIcon = L.divIcon({
        className: '',
        html: `<div style="font-size:28px; filter:drop-shadow(0 0 10px ${ev.color}); text-align:center;">${ev.emoji}</div>`,
        iconSize: [30, 30],
        iconAnchor: [15, 15]
      });
      L.marker(ev.mapCenter, { icon: starIcon }).addTo(miniMap);

      // Store reference
      mapEl._leaflet_map = miniMap;

      // Invalidate size after a short delay
      setTimeout(() => miniMap.invalidateSize(), 100);
    }, 50);
  }
  select(0);
})();

/* ============================================================
   5 · CHART.JS SMELL RADAR & ISOTOPE CHART
   ============================================================ */
let smellChart = null;
function buildSmellChart(){
  if(smellChart) return;
  const el = document.getElementById('smellChart');
  if(!el || typeof Chart === 'undefined') return;
  if(el.clientWidth < 50) { requestAnimationFrame(buildSmellChart); return; }
  smellChart = new Chart(el.getContext('2d'), {
    type: 'radar',
    data: {
      labels: ['Resinous / incense','Citrus','Minty-turpentine','Woody','Sweet / balsamic','Spicy / herb-like'],
      datasets: [
        { label:'Hojari',   data:[9,6,7,4,5,3], borderColor:'#2ecc71', backgroundColor:'rgba(46,204,113,.18)', borderWidth:2.5, pointBackgroundColor:'#2ecc71', pointRadius:4 },
        { label:'Najdi',    data:[8,8,5,5,6,4], borderColor:'#f39c12', backgroundColor:'rgba(243,156,18,.14)',  borderWidth:2.5, pointBackgroundColor:'#f39c12', pointRadius:4 },
        { label:'Shathari', data:[7,8,4,6,6,4], borderColor:'#d4af37', backgroundColor:'rgba(212,175,55,.14)',  borderWidth:2.5, pointBackgroundColor:'#d4af37', pointRadius:4 },
        { label:'Shaabi',   data:[8,4,3,7,5,4], borderColor:'#8b98ab', backgroundColor:'rgba(139,152,171,.14)', borderWidth:2.5, pointBackgroundColor:'#8b98ab', pointRadius:4 }
      ]
    },
    options: {
      responsive: true, maintainAspectRatio: false,
      plugins: {
        legend: { position:'bottom', labels:{ font:{ family:"'Plus Jakarta Sans',sans-serif", size:11 }, boxWidth:12, padding:14, color:'#e2e8f0', usePointStyle:true } },
        title: { display:true, text:'Illustrative sensory profile — not measured data', color:'#8b98ab', font:{ size:11 } },
        tooltip: { callbacks: { label: c => c.dataset.label + ': ' + c.raw + '/10 (illustrative)' } }
      },
      scales: {
        r: {
          beginAtZero:true, max:10,
          ticks:{ stepSize:2, backdropColor:'transparent', color:'#8b98ab', font:{ size:10 } },
          pointLabels:{ color:'#e2e8f0', font:{ family:"'Plus Jakarta Sans',sans-serif", size:11 } },
          grid:{ color:'rgba(139,152,171,.2)' },
          angleLines:{ color:'rgba(139,152,171,.2)' }
        }
      }
    }
  });
}
MODAL_TRIGGER.smell = () => {
  requestAnimationFrame(() => {
    requestAnimationFrame(() => {
      buildSmellChart();
      if(smellChart) setTimeout(() => smellChart.resize(), 100);
    });
  });
};

let isotopeChart = null;
function buildIsotopeChart(){
  if(isotopeChart) return;
  const el = document.getElementById('isotopeChart');
  if(!el || typeof Chart === 'undefined') return;
  if(el.clientWidth < 50) { requestAnimationFrame(buildIsotopeChart); return; }
  isotopeChart = new Chart(el.getContext('2d'), {
    type: 'line',
    data: {
      labels: ['6000 BCE', '4000 BCE', '2000 BCE', '0 CE', '1000 CE', '2026 CE'],
      datasets: [
        { label: 'δ13C (illustrative values)', data: [-26.2, -25.5, -24.1, -23.8, -24.5, -23.2], borderColor: '#3498db', tension: 0.3, fill: false },
        { label: 'δ18O (illustrative values)', data: [22.1, 23.4, 25.8, 26.2, 25.1, 27.4], borderColor: '#e74c3c', tension: 0.3, fill: false }
      ]
    },
    options: {
      responsive: true, maintainAspectRatio: false,
      plugins: { legend: { position: 'bottom', labels: { color: '#e2e8f0' } }, title: { display:true, text:'Concept sketch — not measured data', color:'#8b98ab', font:{ size:11 } } },
      scales: {
        x: { grid: { color: 'rgba(255,255,255,0.1)' }, ticks: { color: '#8b98ab' } },
        y: { grid: { color: 'rgba(255,255,255,0.1)' }, ticks: { color: '#8b98ab' } }
      }
    }
  });
}
MODAL_TRIGGER.biomarkers = () => {
  requestAnimationFrame(() => {
    requestAnimationFrame(() => {
      buildIsotopeChart();
      if(isotopeChart) setTimeout(() => isotopeChart.resize(), 100);
    });
  });
};

/* ============================================================
   6 · GRADE INFO POPUP
   ============================================================ */
const GRADE_INFO = {
  hojari: {
    emoji:'🟢', color:'#2ecc71', title:'Hojari (Hoojri) · Grade 1',
    rows: [
      { k:'Rank', v:'<strong>First grade</strong> — considered the reference quality.' },
      { k:'Naming', v:'Also spelled <em>Hojari</em>, <em>Hougari</em> or <em>Hoojri</em>. Some sources use “Hojari” for a family of quality tiers (Royal, Superior, Regular) rather than a single regional category.' },
      { k:'Microclimate & Terroir', v:'High altitude (800m–1500m) in Jebel Samhan. Extremely dry fog-shadow desert environment with intense sun stress and cold winter nights.' },
      { k:'Appearance', v:'Pale, translucent, green-tinted tears; large clumps.' },
      { k:'Where harvested', v:'Samhan mountains north of Dhofar, Oman.' },
      { k:'Chemistry', v:'High (+)-α-pinene → minty-turpentine lift; moderate limonene for citrus.' },
      { k:'Aroma profile', v:'Resinous / incense (dominant, clean, sacred) · minty-turpentine · moderate citrus · restrained woody-sweet.' },
      { k:'Uses', v:'Royalty · medicinal teas · high-end essential oils · temple-grade incense.' },
      { k:'Sources', v:'Al-Harrasi et al. (2019); Groom (1981); UNESCO (2000).' }
    ]
  },
  najdi: {
    emoji:'🟠', color:'#f39c12', title:'Najdi · Grade 2',
    rows: [
      { k:'Rank', v:'<strong>Second grade</strong> — slightly darker than Hojari.' },
      { k:'Microclimate & Terroir', v:'High Nejd desert plateau (500m–900m). Far inland behind mountain ridges where dry desert winds bake the trees.' },
      { k:'Appearance', v:'Pale yellow clumps; from the plateau behind the Dhofar mountains.' },
      { k:'Where harvested', v:'Nejd plateau, behind the Dhofar mountains.' },
      { k:'Chemistry', v:'Chemically distinct: high <strong>myrcene</strong> content.' },
      { k:'Aroma profile', v:'Pronounced citrus / fruity · full balsamic · softer mint · moderate woody-spicy.' },
      { k:'Uses', v:'Fine perfumes · traditional aromatherapy · high-end bakhoor blends.' },
      { k:'Sources', v:'Al-Harrasi et al. (2019); Groom (1981).' }
    ]
  },
  shathari: {
    emoji:'🟡', color:'#d4af37', title:'Shathari (Shazri) · Grade 3',
    rows: [
      { k:'Rank', v:'<strong>Third grade</strong> — darker than Najdi.' },
      { k:'Microclimate & Terroir', v:'North-western dry wadis (300m–600m). Warm limestone gravel plains with low, variable rainfall.' },
      { k:'Appearance', v:'Golden yellow; collected in north-western Dhofar.' },
      { k:'Where harvested', v:'North-west Dhofar, Oman.' },
      { k:'Chemistry', v:'Characterised by high <strong>limonene</strong> content.' },
      { k:'Aroma profile', v:'Bright citrus / orange · warm rounded resin · noticeable woody · mild sweet-spicy.' },
      { k:'Uses', v:'Daily home bakhoor · mosque incense · mid-range perfumery.' },
      { k:'Sources', v:'Al-Harrasi et al. (2019); Groom (1981).' }
    ]
  },
  shaabi: {
    emoji:'⚫', color:'#8b98ab', title:'Shaabi · Grade 4',
    rows: [
      { k:'Rank', v:'<strong>Fourth grade</strong> — darker and more affordable.' },
      { k:'Microclimate & Terroir', v:'Lowland coastal escarpment (50m–400m). Directly absorbs the heavy summer monsoon fog (Khareef), resulting in fast tree growth and abundant fluid resin.' },
      { k:'Appearance', v:'Darker amber clumps; everyday / local grade.' },
      { k:'Where harvested', v:'Dhofar escarpment, Oman — general commercial supply.' },
      { k:'Chemistry', v:'Essential-oil composition, yield and physicochemical characteristics closely resemble Hojari — the difference is mainly colour and texture due to higher moisture.' },
      { k:'Aroma profile', v:'Deeper woody / resinous · lower citrus · present sweet-balsamic · strong incense when burned.' },
      { k:'Uses', v:'Industrial extracts · herbal soaps · incense sticks · everyday home fragrance.' },
      { k:'Sources', v:'Al-Harrasi et al. (2019); Moussaieff &amp; Mechoulam (2009).' }
    ]
  }
};

function openGradeInfo(key){
  const d = GRADE_INFO[key];
  if(!d) return;
  document.getElementById('gradeInfoEmoji').textContent = d.emoji;
  document.getElementById('gradeInfoTitle').textContent = d.title;
  document.getElementById('gradeInfoHead').style.setProperty('--pop-color', d.color);
  document.getElementById('gradeInfoBody').innerHTML = d.rows.map(r =>
    `<div style="margin-bottom:14px">
      <div style="font-family:var(--font-title);font-size:.6rem;letter-spacing:.14em;text-transform:uppercase;color:${d.color};margin-bottom:3px">${r.k}</div>
      <div style="font-size:.88rem;color:var(--text);line-height:1.55">${r.v}</div>
    </div>`
  ).join('');
  const modal = document.getElementById('m-grade-info');
  modal.classList.add('show');
  modal.setAttribute('aria-hidden','false');
  document.body.classList.add('modal-open');
}

document.querySelectorAll('.grade-card[data-info]').forEach(c => {
  c.addEventListener('click', () => openGradeInfo(c.dataset.info));
});

/* ============================================================
   7 · v2 ADDITIONS — themed navigation & 3D effects
   ============================================================ */

/* 7.2 Pointer-driven 3D tilt on cards (mouse / pen only) */
(function initTilt(){
  if(REDUCED_MOTION || !FINE_POINTER) return;
  const SEL = '.opt-btn,.grade-card,.stat,.health-card,.info,.climate-card';
  let cur = null, raf = 0, last = null;
  function reset(el){ if(el){ el.style.transform = ''; el.style.transition = ''; } }
  document.addEventListener('pointermove', e => {
    if(e.pointerType === 'touch') return;
    const el = e.target.closest ? e.target.closest(SEL) : null;
    if(el !== cur){ reset(cur); cur = el; if(el) el.style.transition = 'transform .12s ease-out, box-shadow .3s, border-color .3s, background .3s'; }
    if(!el) return;
    last = e;
    if(raf) return;
    raf = requestAnimationFrame(() => {
      raf = 0;
      if(!cur || !last) return;
      const r = cur.getBoundingClientRect();
      const px = (last.clientX - r.left) / r.width - .5;
      const py = (last.clientY - r.top) / r.height - .5;
      const max = cur.matches('.opt-btn,.stat') ? 11 : 4.5;
      cur.style.transform = `perspective(900px) rotateX(${(-py*max).toFixed(2)}deg) rotateY(${(px*max).toFixed(2)}deg) translateY(-3px)`;
    });
  }, {passive:true});
  document.documentElement.addEventListener('mouseleave', () => { reset(cur); cur = null; });
})();

/* 7.3 Hero: drifting incense smoke (Three.js points) */
(function initHeroSmoke(){
  const cv = document.getElementById('heroSmoke');
  if(!cv || REDUCED_MOTION || typeof THREE === 'undefined') return;
  let renderer;
  try{ renderer = new THREE.WebGLRenderer({ canvas: cv, alpha: true, antialias: false }); }catch(e){ cv.style.display = 'none'; return; }
  renderer.setPixelRatio(Math.min(window.devicePixelRatio || 1, 1.5));
  const scene = new THREE.Scene();
  const cam = new THREE.PerspectiveCamera(50, 2, 0.1, 50);
  cam.position.z = 8;
  const c = document.createElement('canvas'); c.width = c.height = 64;
  const g = c.getContext('2d');
  const gr = g.createRadialGradient(32,32,0,32,32,32);
  gr.addColorStop(0,'rgba(255,240,200,.95)'); gr.addColorStop(.4,'rgba(230,198,102,.35)'); gr.addColorStop(1,'rgba(230,198,102,0)');
  g.fillStyle = gr; g.fillRect(0,0,64,64);
  const tex = new THREE.CanvasTexture(c);
  const N = window.innerWidth < 700 ? 55 : 120;
  const pos = new Float32Array(N*3), seed = new Float32Array(N);
  for(let i=0;i<N;i++){ pos[i*3]=(Math.random()-.5)*14; pos[i*3+1]=(Math.random()-.5)*8; pos[i*3+2]=(Math.random()-.5)*4; seed[i]=Math.random(); }
  const geo = new THREE.BufferGeometry();
  geo.setAttribute('position', new THREE.BufferAttribute(pos,3));
  const mat = new THREE.PointsMaterial({ map: tex, size: 1.7, transparent: true, opacity: .26, depthWrite: false, blending: THREE.AdditiveBlending });
  const pts = new THREE.Points(geo, mat);
  scene.add(pts);
  function size(){
    const w = cv.clientWidth, h = cv.clientHeight;
    if(!w || !h) return;
    renderer.setSize(w, h, false);
    cam.aspect = w / h; cam.updateProjectionMatrix();
  }
  size(); window.addEventListener('resize', size);
  let vis = true;
  if('IntersectionObserver' in window) new IntersectionObserver(es => { vis = es[0].isIntersecting; }).observe(cv);
  let t = 0;
  (function loop(){
    requestAnimationFrame(loop);
    if(!vis || document.hidden) return;
    t += .008;
    const p = geo.attributes.position.array;
    for(let i=0;i<N;i++){
      p[i*3+1] += .006 + seed[i]*.006;
      p[i*3]   += Math.sin(t*1.3 + seed[i]*20) * .003;
      if(p[i*3+1] > 4.2){ p[i*3+1] = -4.2; p[i*3] = (Math.random()-.5)*14; }
    }
    geo.attributes.position.needsUpdate = true;
    pts.rotation.y = Math.sin(t*.3) * .15;
    renderer.render(scene, cam);
  })();
})();

/* 7.4 Schematic 3D terroir relief */
let terroir3d = null;
function buildTerroir3D(){
  const box = document.getElementById('terroir3d');
  if(!box || typeof THREE === 'undefined') return;
  if(terroir3d){ terroir3d.resize(); return; }
  if(box.clientWidth < 50){ requestAnimationFrame(buildTerroir3D); return; }

  let renderer;
  try{ renderer = new THREE.WebGLRenderer({ antialias: true, alpha: true }); }
  catch(e){ box.innerHTML = '<div class="resin-hint" style="position:static;transform:none;margin:20px">3D view needs WebGL, which is not available in this browser.</div>'; return; }
  renderer.setPixelRatio(Math.min(window.devicePixelRatio || 1, 2));
  renderer.setSize(box.clientWidth, box.clientHeight);
  box.appendChild(renderer.domElement);

  const scene = new THREE.Scene();
  const camera = new THREE.PerspectiveCamera(42, box.clientWidth / box.clientHeight, 0.1, 100);
  const HOME = { pos: new THREE.Vector3(0.0, 3.4, 5.6), target: new THREE.Vector3(0, 0.25, -0.2) };
  camera.position.copy(HOME.pos);

  const controls = new THREE.OrbitControls(camera, renderer.domElement);
  controls.target.copy(HOME.target);
  controls.enableDamping = true; controls.dampingFactor = 0.08;
  controls.enablePan = true; controls.screenSpacePanning = false;
  controls.minDistance = 3; controls.maxDistance = 11;
  controls.maxPolarAngle = Math.PI * 0.47;
  controls.update();

  scene.add(new THREE.HemisphereLight(0xcfe4ff, 0x4a3b22, 0.85));
  const sun = new THREE.DirectionalLight(0xfff0cc, 1.25); sun.position.set(-4, 6, 4); scene.add(sun);

  /* geography -> scene coordinates (schematic) */
  const LON0 = 54.05, LAT0 = 17.35, XS = 3.2 / 0.85, ZS = 1.8 / 0.5;
  const toX = lon => (lon - LON0) * XS;
  const toZ = lat => -((lat - LAT0) * ZS);
  const sm = (a,b,x) => { const t = Math.min(1, Math.max(0, (x-a)/(b-a))); return t*t*(3-2*t); };
  function height(lat, lon){
    let h = 0.04;
    h -= 0.15 * (1 - sm(16.85, 16.98, lat));                                   // sea floor
    h += 0.95 * sm(17.02, 17.22, lat);                                          // escarpment
    h -= 0.55 * sm(17.30, 17.75, lat);                                          // slope to plateau
    h += 0.22 * sm(54.1, 54.8, lon) * sm(17.05, 17.25, lat) * (1 - sm(17.4, 17.6, lat)); // Samhan higher
    h += 0.05 * Math.sin(lon*38) * Math.cos(lat*45) + 0.03 * Math.sin(lon*91 + lat*70);
    return h;
  }
  const ZONES = [
    { key:'hojari',   name:'Hojari',   lat:17.18, lon:54.65, color:0x2ecc71 },
    { key:'najdi',    name:'Najdi',    lat:17.55, lon:54.05, color:0xf39c12 },
    { key:'shathari', name:'Shathari', lat:17.40, lon:53.40, color:0xd4af37 },
    { key:'shaabi',   name:'Shaabi',   lat:17.02, lon:54.10, color:0x9fb3c8 }
  ];

  /* terrain */
  const W = 6.4, D = 3.6, SX = 150, SZ = 90;
  const geo = new THREE.PlaneGeometry(W, D, SX, SZ);
  const pos = geo.attributes.position;
  const colors = new Float32Array(pos.count * 3);
  const cLow = new THREE.Color(0xc9b27a), cGreen = new THREE.Color(0x6f8f4f), cRock = new THREE.Color(0x8a6f4a), cDesert = new THREE.Color(0xd8c08a), cSea = new THREE.Color(0x24607f);
  const tmp = new THREE.Color();
  for(let i=0;i<pos.count;i++){
    const px = pos.getX(i), py = pos.getY(i);
    const lon = LON0 + (px / 3.2) * 0.85;
    const lat = LAT0 + (py / 1.8) * 0.5;
    const h = height(lat, lon);
    pos.setZ(i, h);
    if(h < 0.02) tmp.copy(cSea).lerp(cLow, Math.max(0, (h + 0.12) / 0.14));
    else if(lat < 17.28) tmp.copy(cLow).lerp(cGreen, sm(17.02, 17.14, lat)).lerp(cRock, sm(17.18, 17.28, lat) * 0.7);
    else tmp.copy(cRock).lerp(cDesert, sm(17.3, 17.7, lat));
    ZONES.forEach(z => {
      const d2 = (lat - z.lat) ** 2 + (lon - z.lon) ** 2;
      const w = Math.exp(-d2 / (2 * 0.1 * 0.1)) * 0.55;
      if(w > 0.01) tmp.lerp(new THREE.Color(z.color), w);
    });
    colors[i*3] = tmp.r; colors[i*3+1] = tmp.g; colors[i*3+2] = tmp.b;
  }
  geo.setAttribute('color', new THREE.BufferAttribute(colors, 3));
  geo.computeVertexNormals();
  const terrain = new THREE.Mesh(geo, new THREE.MeshStandardMaterial({ vertexColors: true, roughness: 0.95, metalness: 0, flatShading: false }));
  terrain.rotation.x = -Math.PI / 2;
  scene.add(terrain);

  const sea = new THREE.Mesh(new THREE.PlaneGeometry(W, D), new THREE.MeshStandardMaterial({ color: 0x1f6f95, transparent: true, opacity: 0.72, roughness: 0.25 }));
  sea.rotation.x = -Math.PI / 2; sea.position.y = 0.0; scene.add(sea);

  /* labels */
  function label(text, color, scale){
    const c = document.createElement('canvas'); c.width = 512; c.height = 128;
    const g = c.getContext('2d');
    g.font = '700 54px "Plus Jakarta Sans", sans-serif'; g.textAlign = 'center'; g.textBaseline = 'middle';
    g.lineWidth = 10; g.strokeStyle = 'rgba(5,7,10,.9)'; g.strokeText(text, 256, 64);
    g.fillStyle = color; g.fillText(text, 256, 64);
    const sp = new THREE.Sprite(new THREE.SpriteMaterial({ map: new THREE.CanvasTexture(c), transparent: true, depthTest: false }));
    sp.scale.set(scale * 2.2, scale * 0.55, 1);
    sp.renderOrder = 10;
    return sp;
  }
  const hits = [];
  const rings = [];
  ZONES.forEach(z => {
    const x = toX(z.lon), zz = toZ(z.lat), h = Math.max(height(z.lat, z.lon), 0.04);
    const ring = new THREE.Mesh(new THREE.TorusGeometry(0.26, 0.028, 12, 48), new THREE.MeshBasicMaterial({ color: z.color }));
    ring.rotation.x = Math.PI / 2; ring.position.set(x, h + 0.03, zz);
    ring.userData.zone = z.key; scene.add(ring); rings.push(ring); hits.push(ring);
    const disc = new THREE.Mesh(new THREE.CircleGeometry(0.26, 40), new THREE.MeshBasicMaterial({ color: z.color, transparent: true, opacity: 0.25, depthWrite: false }));
    disc.rotation.x = -Math.PI / 2; disc.position.set(x, h + 0.025, zz); disc.userData.zone = z.key; scene.add(disc); hits.push(disc);
    const sp = label(z.name, '#' + z.color.toString(16).padStart(6, '0'), 0.75);
    sp.position.set(x, h + 0.55, zz); sp.userData.zone = z.key; scene.add(sp); hits.push(sp);
    const line = new THREE.Line(new THREE.BufferGeometry().setFromPoints([new THREE.Vector3(x, h + 0.03, zz), new THREE.Vector3(x, h + 0.42, zz)]), new THREE.LineBasicMaterial({ color: z.color }));
    scene.add(line);
  });
  const seaLbl = label('Arabian Sea', '#9fd3ee', 0.8); seaLbl.position.set(-1.9, 0.18, toZ(16.9)); scene.add(seaLbl);
  const salalah = label('Salalah', '#ffffff', 0.55); salalah.position.set(toX(54.09), 0.3, toZ(17.0)); scene.add(salalah);
  const plateau = label('Nejd plateau → Empty Quarter', '#f3e5ab', 0.9); plateau.position.set(1.6, 0.85, toZ(17.8)); scene.add(plateau);

  /* Khareef fog */
  const fc = document.createElement('canvas'); fc.width = fc.height = 64;
  const fg = fc.getContext('2d'); const fgr = fg.createRadialGradient(32,32,0,32,32,32);
  fgr.addColorStop(0,'rgba(235,245,255,.9)'); fgr.addColorStop(1,'rgba(235,245,255,0)'); fg.fillStyle = fgr; fg.fillRect(0,0,64,64);
  const FN = window.innerWidth < 700 ? 90 : 220;
  const fpos = new Float32Array(FN * 3), fseed = new Float32Array(FN);
  const fogZ0 = toZ(17.3), fogZ1 = toZ(16.95);
  function seedFog(i, anywhere){
    fpos[i*3]   = (Math.random() - .5) * W;
    fpos[i*3+1] = 0.15 + Math.random() * 0.8;
    fpos[i*3+2] = anywhere ? fogZ0 + Math.random() * (fogZ1 - fogZ0) : fogZ1;
  }
  for(let i=0;i<FN;i++){ seedFog(i, true); fseed[i] = Math.random(); }
  const fgeo = new THREE.BufferGeometry(); fgeo.setAttribute('position', new THREE.BufferAttribute(fpos, 3));
  const fog = new THREE.Points(fgeo, new THREE.PointsMaterial({ map: new THREE.CanvasTexture(fc), size: 0.75, transparent: true, opacity: 0.4, depthWrite: false }));
  scene.add(fog);
  let fogOn = true;
  const fogBtn = document.getElementById('t3dFog');
  if(fogBtn) fogBtn.addEventListener('click', () => {
    fogOn = !fogOn; fog.visible = fogOn;
    fogBtn.setAttribute('aria-pressed', String(fogOn));
    fogBtn.textContent = '☁️ Khareef fog: ' + (fogOn ? 'on' : 'off');
  });
  const resetBtn = document.getElementById('t3dReset');
  if(resetBtn) resetBtn.addEventListener('click', () => { camera.position.copy(HOME.pos); controls.target.copy(HOME.target); controls.update(); });

  /* click / tap a zone */
  const ray = new THREE.Raycaster(), mouse = new THREE.Vector2();
  let down = null;
  function pick(e){
    const r = renderer.domElement.getBoundingClientRect();
    mouse.set(((e.clientX - r.left) / r.width) * 2 - 1, -((e.clientY - r.top) / r.height) * 2 + 1);
    ray.setFromCamera(mouse, camera);
    const hit = ray.intersectObjects(hits, false)[0];
    return hit ? hit.object.userData.zone : null;
  }
  renderer.domElement.addEventListener('pointerdown', e => { down = { x: e.clientX, y: e.clientY }; });
  renderer.domElement.addEventListener('pointerup', e => {
    if(!down) return;
    const moved = Math.hypot(e.clientX - down.x, e.clientY - down.y); down = null;
    if(moved > 6) return;
    const z = pick(e);
    if(z) openGradeInfo(z);
  });
  renderer.domElement.addEventListener('pointermove', e => { if(e.pointerType !== 'touch') renderer.domElement.style.cursor = pick(e) ? 'pointer' : ''; });

  function resize(){
    const w = box.clientWidth, h = box.clientHeight;
    if(w < 10 || h < 10) return;
    camera.aspect = w / h; camera.updateProjectionMatrix(); renderer.setSize(w, h);
  }
  if('ResizeObserver' in window) new ResizeObserver(resize).observe(box); else window.addEventListener('resize', resize);

  let t = 0;
  (function loop(){
    requestAnimationFrame(loop);
    if(document.hidden || !box.offsetParent) return;
    t += 0.01;
    if(fogOn && !REDUCED_MOTION){
      const p = fgeo.attributes.position.array;
      for(let i=0;i<FN;i++){
        p[i*3+2] -= 0.0035 + fseed[i] * 0.003;
        p[i*3]   += Math.sin(t + fseed[i] * 12) * 0.0015;
        p[i*3+1] += 0.0006;
        if(p[i*3+2] < fogZ0 - 0.1 || p[i*3+1] > 1.1){ seedFog(i, false); }
      }
      fgeo.attributes.position.needsUpdate = true;
    }
    rings.forEach((r, i) => { const s = 1 + 0.06 * Math.sin(t * 2 + i); r.scale.set(s, s, s); });
    controls.update();
    renderer.render(scene, camera);
  })();

  terroir3d = { resize };
}
</script>
</body>
</html>
