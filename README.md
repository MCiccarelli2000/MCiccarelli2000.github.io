<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1"/>
<meta name="description" content="Chef privado a domicilio en Madrid. Cocina mediterránea con alma argentina desde 65€/persona."/>
<title>Mauro Ciccarelli · Chef Privado Madrid</title>
<link rel="preconnect" href="https://fonts.googleapis.com"/>
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin/>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;1,300;1,400&family=Inter:wght@300;400;500&display=swap" rel="stylesheet"/>
<style>
:root{
  --ink:#0e1e2e;--ink2:#1a2f44;--sand:#f5f0e8;--sand2:#ece5d5;
  --gold:#b8935a;--goldp:#d4b483;--white:#fafaf8;--body:#3a3028;
  --fd:'Cormorant Garamond',Georgia,serif;--fb:'Inter',system-ui,sans-serif;
  --ease:cubic-bezier(.4,0,.2,1);
}
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{background:var(--white);color:var(--body);font-family:var(--fb);font-weight:300;line-height:1.7;-webkit-font-smoothing:antialiased}
img{display:block;max-width:100%}
a{color:inherit;text-decoration:none}

/* NAV */
nav{position:fixed;top:0;left:0;right:0;z-index:100;display:flex;align-items:center;justify-content:space-between;padding:1.2rem 3rem;transition:background .4s,padding .3s}
nav.s{background:rgba(14,30,46,.97);padding:.9rem 3rem}
.nl{font-family:var(--fd);font-size:1.05rem;color:var(--white);letter-spacing:.15em;text-transform:uppercase}
.nl span{color:var(--goldp)}
.nm{display:flex;gap:2rem;list-style:none}
.nm a{font-size:.7rem;letter-spacing:.13em;text-transform:uppercase;color:rgba(255,255,255,.7);transition:color .2s}
.nm a:hover{color:var(--goldp)}
.nc{font-size:.7rem;letter-spacing:.12em;text-transform:uppercase;padding:.5rem 1.3rem;border:1px solid var(--gold);color:var(--goldp);transition:background .2s,color .2s}
.nc:hover{background:var(--gold);color:var(--ink)}
.hbg{display:none;flex-direction:column;gap:5px;background:none;border:none;cursor:pointer;padding:4px}
.hbg span{display:block;width:24px;height:1.5px;background:var(--white)}
.mob{display:none;position:fixed;inset:0;z-index:99;background:var(--ink);flex-direction:column;align-items:center;justify-content:center;gap:2.5rem}
.mob.o{display:flex}
.mob a{font-family:var(--fd);font-size:2rem;color:var(--white)}
.mob a:hover{color:var(--goldp)}
.mbc{position:absolute;top:1.5rem;right:2rem;background:none;border:none;color:var(--white);font-size:2rem;cursor:pointer}

/* HERO */
.hero{position:relative;height:100vh;min-height:640px;display:flex;align-items:flex-end;overflow:hidden}
.hbg2{position:absolute;inset:0;background:url('https://mciccarelli2000.github.io/assets/hero-chef-plato.jpg') center/cover}
.hbg2::after{content:'';position:absolute;inset:0;background:linear-gradient(to bottom,rgba(14,30,46,.1) 0%,rgba(14,30,46,.35) 50%,rgba(14,30,46,.85) 100%)}
.hc{position:relative;z-index:1;padding:0 3rem 5rem;max-width:820px}
.hc .ey{font-size:.7rem;letter-spacing:.22em;text-transform:uppercase;color:var(--goldp);margin-bottom:1.2rem}
.hc h1{font-family:var(--fd);font-size:clamp(3rem,6vw,5.5rem);font-weight:300;line-height:1.08;color:var(--white);margin-bottom:1.2rem}
.hc h1 em{font-style:italic;color:var(--goldp)}
.hc p{font-size:.95rem;color:rgba(255,255,255,.7);margin-bottom:.8rem;max-width:480px}
.hc .pr{font-family:var(--fd);font-size:1.1rem;color:var(--goldp);margin-bottom:2rem}
.acts{display:flex;gap:1rem;flex-wrap:wrap}
.bp{display:inline-block;padding:.75rem 2rem;background:var(--gold);color:var(--ink);font-size:.72rem;letter-spacing:.12em;text-transform:uppercase;font-weight:500;transition:background .2s,transform .15s}
.bp:hover{background:var(--goldp);transform:translateY(-1px)}
.bo{display:inline-flex;align-items:center;gap:.5rem;padding:.75rem 1.8rem;border:1px solid rgba(255,255,255,.35);color:var(--white);font-size:.72rem;letter-spacing:.12em;text-transform:uppercase;transition:border-color .2s,background .2s}
.bo:hover{border-color:var(--white);background:rgba(255,255,255,.08)}
.bo svg{width:16px;height:16px}

/* SECTIONS */
section{padding:6rem 3rem}
.sl{font-size:.68rem;letter-spacing:.22em;text-transform:uppercase;color:var(--gold);margin-bottom:.8rem}
.st{font-family:var(--fd);font-size:clamp(2rem,4vw,3rem);font-weight:300;line-height:1.15;color:var(--ink);margin-bottom:1.4rem}
.st em{font-style:italic;color:var(--gold)}
.dv{width:40px;height:1px;background:var(--gold);margin:0 auto 3.5rem}

/* SOBRE */
#sobre{background:var(--white)}
.si{max-width:1100px;margin:0 auto;display:grid;grid-template-columns:1fr 1fr;gap:5rem;align-items:center}
.sg{display:grid;grid-template-columns:1fr 1fr;grid-template-rows:200px 200px;gap:10px}
.sg img{width:100%;height:100%;object-fit:cover}
.sg img:first-child{grid-column:1/3;height:180px}
.st2 p{font-size:.93rem;color:#4a4038;margin-bottom:1.1rem}

/* MENUS */
#menus{background:var(--ink)}
#menus .sl{color:var(--goldp)}
#menus .st{color:var(--white)}
.mg{max-width:1000px;margin:0 auto;display:grid;grid-template-columns:repeat(3,1fr);gap:2px}
.mc{padding:2.8rem 2.2rem;background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.07);transition:background .25s}
.mc:hover{background:rgba(255,255,255,.09)}
.mi{font-size:1.4rem;margin-bottom:1rem}
.mn{font-family:var(--fd);font-size:1.5rem;font-weight:300;color:var(--white);margin-bottom:.3rem}
.mp{font-family:var(--fd);font-size:1.1rem;color:var(--goldp);margin-bottom:.8rem}
.md{font-size:.83rem;color:rgba(255,255,255,.48);line-height:1.6}
.mn2{text-align:center;margin-top:2rem;font-size:.78rem;color:rgba(255,255,255,.3)}

/* GALERIA */
#galeria{background:var(--sand)}
.gg{max-width:1200px;margin:0 auto;display:grid;grid-template-columns:repeat(3,1fr);gap:8px}
.gi{position:relative;overflow:hidden;aspect-ratio:4/3}
.gi:nth-child(1){grid-column:1/3;aspect-ratio:16/7}
.gi img{width:100%;height:100%;object-fit:cover;transition:transform .5s var(--ease)}
.gi:hover img{transform:scale(1.05)}
.gc{position:absolute;bottom:0;left:0;right:0;padding:.7rem 1rem;background:linear-gradient(transparent,rgba(14,30,46,.75));color:var(--white);font-size:.7rem;letter-spacing:.1em;text-transform:uppercase;opacity:0;transform:translateY(4px);transition:opacity .3s,transform .3s}
.gi:hover .gc{opacity:1;transform:translateY(0)}

/* TRAYECTORIA */
#tray{background:var(--white)}
.ti{max-width:800px;margin:0 auto}
.ti p{font-size:.93rem;color:#4a4038;margin-bottom:1.1rem}
.tls{display:flex;gap:1rem;flex-wrap:wrap;margin-top:2rem}
.tl{font-size:.7rem;letter-spacing:.13em;text-transform:uppercase;padding:.5rem 1.2rem;border:1px solid var(--gold);color:var(--gold);transition:background .2s,color .2s}
.tl:hover{background:var(--gold);color:var(--white)}

/* PROCESO */
#proceso{background:var(--sand2)}
.pg{max-width:900px;margin:0 auto;display:grid;grid-template-columns:repeat(3,1fr);gap:2.5rem}
.ps{border-top:1px solid var(--gold);padding-top:1.4rem}
.pn{font-family:var(--fd);font-size:2.5rem;font-weight:300;color:var(--goldp);margin-bottom:.6rem}
.pt{font-size:.75rem;letter-spacing:.12em;text-transform:uppercase;color:var(--ink);font-weight:500;margin-bottom:.5rem}
.pd{font-size:.87rem;color:#5a4e44;line-height:1.65}

/* ═══════════════════════════════════════════════
   BOOKING SYSTEM
═══════════════════════════════════════════════ */
#reserva{background:var(--ink)}
#reserva .sl{color:var(--goldp)}
#reserva .st{color:var(--white)}

.booking-wrap{max-width:1000px;margin:0 auto;display:grid;grid-template-columns:1fr 1.4fr;gap:4rem;align-items:start}

/* Info lateral */
.bk-info h3{font-family:var(--fd);font-size:1.05rem;font-weight:300;color:var(--white);margin-bottom:1.8rem;line-height:1.5}
.bk-dato{display:flex;align-items:flex-start;gap:.9rem;margin-bottom:1.3rem}
.bk-ico{width:34px;height:34px;flex-shrink:0;display:flex;align-items:center;justify-content:center;border:1px solid rgba(255,255,255,.14)}
.bk-ico svg{width:15px;height:15px;stroke:var(--goldp);fill:none;stroke-width:1.5}
.bk-txt{font-size:.83rem;color:rgba(255,255,255,.52);line-height:1.6}
.bk-txt strong{display:block;color:var(--white);font-weight:400;margin-bottom:.1rem}
.bk-txt a{color:var(--goldp);transition:color .2s}
.bk-txt a:hover{color:var(--white)}

/* Estado del sistema */
.bk-status{margin-top:2rem;padding:1rem 1.2rem;background:rgba(255,255,255,.04);border-left:2px solid var(--gold)}
.bk-status-title{font-size:.65rem;letter-spacing:.15em;text-transform:uppercase;color:var(--goldp);margin-bottom:.4rem}
.bk-status-msg{font-size:.8rem;color:rgba(255,255,255,.5);line-height:1.5}

/* Calendario visual */
.cal-header{display:flex;align-items:center;justify-content:space-between;margin-bottom:1rem}
.cal-title{font-family:var(--fd);font-size:1.1rem;font-weight:300;color:var(--white)}
.cal-nav{background:none;border:1px solid rgba(255,255,255,.15);color:rgba(255,255,255,.6);width:28px;height:28px;cursor:pointer;font-size:.9rem;transition:border-color .2s,color .2s}
.cal-nav:hover{border-color:var(--gold);color:var(--goldp)}
.cal-grid{display:grid;grid-template-columns:repeat(7,1fr);gap:2px;margin-bottom:.8rem}
.cal-day-name{font-size:.62rem;letter-spacing:.1em;text-transform:uppercase;color:rgba(255,255,255,.3);text-align:center;padding:.4rem 0}
.cal-day{aspect-ratio:1;display:flex;align-items:center;justify-content:center;font-size:.8rem;color:rgba(255,255,255,.4);cursor:default;border-radius:1px;transition:background .2s,color .2s;position:relative}
.cal-day.empty{pointer-events:none}
.cal-day.past{color:rgba(255,255,255,.18);cursor:not-allowed}
.cal-day.booked{background:rgba(184,147,90,.15);color:var(--goldp);cursor:not-allowed}
.cal-day.booked::after{content:'';position:absolute;bottom:3px;left:50%;transform:translateX(-50%);width:4px;height:4px;border-radius:50%;background:var(--gold)}
.cal-day.available{color:rgba(255,255,255,.75);cursor:pointer}
.cal-day.available:hover{background:rgba(255,255,255,.1);color:var(--white)}
.cal-day.selected{background:var(--gold);color:var(--ink);font-weight:500}
.cal-day.today{outline:1px solid rgba(255,255,255,.25)}
.cal-legend{display:flex;gap:1.2rem;margin-bottom:1.4rem}
.cal-leg{display:flex;align-items:center;gap:.4rem;font-size:.68rem;color:rgba(255,255,255,.35)}
.cal-leg span{width:8px;height:8px;border-radius:50%}
.cal-leg .l-free{background:rgba(255,255,255,.4)}
.cal-leg .l-busy{background:var(--gold)}

/* Formulario reserva */
.rf{display:flex;flex-direction:column;gap:2px;background:rgba(255,255,255,.06)}
.rf-field{background:rgba(255,255,255,.03);padding:.9rem 1.1rem}
.rf-field label{display:block;font-size:.63rem;letter-spacing:.13em;text-transform:uppercase;color:rgba(255,255,255,.38);margin-bottom:.4rem}
.rf-field input,.rf-field select,.rf-field textarea{width:100%;background:none;border:none;outline:none;font-family:var(--fb);font-size:.88rem;font-weight:300;color:var(--white)}
.rf-field input::placeholder,.rf-field textarea::placeholder{color:rgba(255,255,255,.18)}
.rf-field select option{background:var(--ink2);color:var(--white)}
.rf-row{display:grid;grid-template-columns:1fr 1fr;gap:2px}
.rf-selected-date{background:rgba(184,147,90,.12);padding:.9rem 1.1rem;font-size:.85rem;color:var(--goldp)}
.rf-selected-date strong{display:block;font-size:.63rem;letter-spacing:.13em;text-transform:uppercase;color:rgba(255,255,255,.35);margin-bottom:.3rem;font-weight:400}
.rf-footer{display:flex;justify-content:space-between;align-items:center;padding:1rem 1.1rem;background:rgba(255,255,255,.03);border-top:1px solid rgba(255,255,255,.07)}
.rf-note{font-size:.72rem;color:rgba(255,255,255,.25)}
.btn-book{padding:.7rem 2rem;background:var(--gold);color:var(--ink);font-size:.7rem;letter-spacing:.13em;text-transform:uppercase;font-weight:500;border:none;cursor:pointer;transition:background .2s,transform .15s}
.btn-book:hover{background:var(--goldp);transform:translateY(-1px)}
.btn-book:disabled{opacity:.4;cursor:not-allowed;transform:none}

/* ── RESPUESTA AUTOMÁTICA ── */
.auto-panel{display:none;padding:2rem;background:rgba(255,255,255,.04);border:1px solid rgba(255,255,255,.1);margin-top:3rem;max-width:1000px;margin-left:auto;margin-right:auto}
.auto-panel.show{display:block}
.auto-steps{display:grid;grid-template-columns:repeat(3,1fr);gap:1.5rem;margin-top:1.5rem}
.auto-step{padding:1.2rem;background:rgba(255,255,255,.03);border-top:1px solid var(--gold)}
.auto-num{font-family:var(--fd);font-size:2rem;color:var(--goldp);margin-bottom:.5rem}
.auto-title{font-size:.7rem;letter-spacing:.1em;text-transform:uppercase;color:var(--white);margin-bottom:.4rem}
.auto-desc{font-size:.8rem;color:rgba(255,255,255,.45);line-height:1.55}

/* CONFIRMACIÓN */
.confirm-modal{display:none;position:fixed;inset:0;z-index:200;background:rgba(14,30,46,.9);align-items:center;justify-content:center;padding:2rem}
.confirm-modal.show{display:flex}
.confirm-box{background:var(--ink2);max-width:520px;width:100%;padding:3rem 2.5rem;position:relative;border:1px solid rgba(255,255,255,.1)}
.confirm-close{position:absolute;top:1rem;right:1.2rem;background:none;border:none;color:rgba(255,255,255,.4);font-size:1.3rem;cursor:pointer}
.confirm-close:hover{color:var(--white)}
.confirm-icon{font-size:2.5rem;margin-bottom:1.2rem}
.confirm-title{font-family:var(--fd);font-size:1.8rem;font-weight:300;color:var(--white);margin-bottom:.8rem}
.confirm-msg{font-size:.88rem;color:rgba(255,255,255,.55);line-height:1.7;margin-bottom:1.6rem}
.confirm-detail{background:rgba(255,255,255,.05);padding:1rem 1.2rem;margin-bottom:1.6rem}
.confirm-detail p{font-size:.82rem;color:rgba(255,255,255,.6);line-height:1.7}
.confirm-detail strong{color:var(--goldp)}
.confirm-actions{display:flex;gap:.8rem;flex-wrap:wrap}
.confirm-wa{display:inline-flex;align-items:center;gap:.5rem;padding:.65rem 1.5rem;background:var(--gold);color:var(--ink);font-size:.7rem;letter-spacing:.12em;text-transform:uppercase;font-weight:500;cursor:pointer;border:none;transition:background .2s}
.confirm-wa:hover{background:var(--goldp)}
.confirm-close2{padding:.65rem 1.5rem;border:1px solid rgba(255,255,255,.2);color:rgba(255,255,255,.5);font-size:.7rem;letter-spacing:.12em;text-transform:uppercase;background:none;cursor:pointer;transition:border-color .2s}
.confirm-close2:hover{border-color:var(--white);color:var(--white)}

/* TOAST */
.toast{position:fixed;bottom:2rem;right:2rem;z-index:300;padding:.9rem 1.5rem;background:var(--gold);color:var(--ink);font-size:.82rem;font-weight:500;transform:translateY(10px);opacity:0;transition:opacity .3s,transform .3s;pointer-events:none}
.toast.show{opacity:1;transform:translateY(0)}

/* FOOTER */
footer{background:#07101a;padding:2rem 3rem;display:flex;align-items:center;justify-content:space-between;gap:1rem;flex-wrap:wrap}
.fl{font-family:var(--fd);font-size:.9rem;color:rgba(255,255,255,.35);letter-spacing:.1em}
.fc{font-size:.7rem;color:rgba(255,255,255,.22)}
.fw{display:inline-flex;align-items:center;gap:.4rem;font-size:.7rem;letter-spacing:.1em;text-transform:uppercase;color:var(--goldp);transition:color .2s}
.fw:hover{color:var(--white)}

/* FADE IN */
.fi{opacity:0;transform:translateY(20px);transition:opacity .65s var(--ease),transform .65s var(--ease)}
.fi.v{opacity:1;transform:translateY(0)}

/* RESPONSIVE */
@media(max-width:900px){
  nav{padding:1.2rem 1.5rem}
  nav.s{padding:.9rem 1.5rem}
  .nm,.nc{display:none}
  .hbg{display:flex}
  section{padding:4rem 1.5rem}
  .hc{padding:0 1.5rem 3.5rem}
  .si{grid-template-columns:1fr;gap:2.5rem}
  .sg{grid-template-rows:180px 180px}
  .sg img:first-child{height:160px}
  .mg{grid-template-columns:1fr}
  .gg{grid-template-columns:1fr 1fr}
  .gi:nth-child(1){grid-column:1/3;aspect-ratio:16/8}
  .pg{grid-template-columns:1fr;gap:2rem}
  .booking-wrap{grid-template-columns:1fr;gap:2.5rem}
  .auto-steps{grid-template-columns:1fr;gap:1rem}
  footer{flex-direction:column;text-align:center;padding:1.8rem 1.5rem}
}
@media(prefers-reduced-motion:reduce){*,.fi{transition:none!important}}
</style>
</head>
<body>

<!-- NAV -->
<nav id="nav">
  <div class="nl">Mauro <span>Ciccarelli</span></div>
  <ul class="nm">
    <li><a href="#sobre">Sobre mí</a></li>
    <li><a href="#menus">Menús</a></li>
    <li><a href="#galeria">Galería</a></li>
    <li><a href="#tray">Trayectoria</a></li>
    <li><a href="#reserva">Reservar</a></li>
  </ul>
  <a href="#reserva" class="nc">Reservar fecha</a>
  <button class="hbg" id="hbg" aria-label="Menú"><span></span><span></span><span></span></button>
</nav>
<div class="mob" id="mob">
  <button class="mbc" id="mbc">✕</button>
  <a href="#sobre" class="ml">Sobre mí</a>
  <a href="#menus" class="ml">Menús</a>
  <a href="#galeria" class="ml">Galería</a>
  <a href="#tray" class="ml">Trayectoria</a>
  <a href="#reserva" class="ml">Reservar</a>
</div>

<!-- HERO -->
<section class="hero" id="inicio">
  <div class="hbg2"></div>
  <div class="hc fi">
    <p class="ey">Chef privado · Madrid</p>
    <h1>Cocina de autor<br>en <em>tu propia mesa</em></h1>
    <p>Experiencias gastronómicas personalizadas para comidas, cenas y celebraciones privadas en casa, finca o villa.</p>
    <p class="pr">Desde 65 € por persona</p>
    <div class="acts">
      <a href="#reserva" class="bp">Consultar disponibilidad</a>
      <a href="https://wa.me/34630386059?text=Hola%20Mauro%2C%20quiero%20consultar%20disponibilidad." target="_blank" rel="noopener" class="bo">
        <svg viewBox="0 0 24 24" fill="currentColor"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347zM12 0C5.373 0 0 5.373 0 12c0 2.124.554 4.118 1.526 5.847L.057 23.882l6.198-1.455A11.934 11.934 0 0012 24c6.627 0 12-5.373 12-12S18.627 0 12 0zm0 21.818a9.796 9.796 0 01-5.034-1.386l-.359-.214-3.68.964.983-3.595-.234-.369A9.818 9.818 0 012.182 12C2.182 6.575 6.575 2.182 12 2.182c5.424 0 9.818 4.393 9.818 9.818 0 5.424-4.394 9.818-9.818 9.818z"/></svg>
        WhatsApp
      </a>
    </div>
  </div>
</section>

<!-- SOBRE -->
<section id="sobre">
  <div class="si">
    <div class="sg fi">
      <img src="https://mciccarelli2000.github.io/assets/mauro-brasa-real.jpg" alt="Mauro a la brasa" loading="lazy"/>
      <img src="https://mciccarelli2000.github.io/assets/mauro-pasta-creada.jpg" alt="Pasta fresca" loading="lazy"/>
      <img src="https://mciccarelli2000.github.io/assets/galeria-pasta-chef.jpg" alt="Cocina" loading="lazy"/>
    </div>
    <div class="st2 fi">
      <p class="sl">Sobre mí</p>
      <h2 class="st">Cocina, cercanía<br>y <em>experiencia</em></h2>
      <p>Soy Mauro Ciccarelli, chef argentino afincado en España. Mi cocina une producto, técnica y cercanía para crear experiencias gastronómicas personalizadas en casas, fincas, villas y eventos privados.</p>
      <p>Trabajo desde el sabor y el oficio: pasta fresca, brasa, crudos, pescados, carnes y platos pensados para cada mesa.</p>
      <p>El objetivo es que disfrutes de una comida privada con cocina de restaurante, sin perder la naturalidad de una celebración en casa.</p>
    </div>
  </div>
</section>

<!-- MENUS -->
<section id="menus">
  <div class="fi" style="text-align:center;margin-bottom:3.5rem">
    <p class="sl">Menús</p>
    <h2 class="st" style="color:var(--white)">Tres formatos <em style="color:var(--goldp)">orientativos</em></h2>
    <div class="dv"></div>
  </div>
  <div class="mg fi">
    <div class="mc"><div class="mi">❦</div><div class="mn">Selección</div><div class="mp">Desde 65 €</div><p class="md">Aperitivo, dos entrantes, plato principal y postre. Ideal para cenas íntimas o comidas en familia.</p></div>
    <div class="mc"><div class="mi">🐟</div><div class="mn">Experiencia</div><div class="mp">Desde 75 €</div><p class="md">Aperitivo, tres entrantes, principal y postre. Para quienes quieren recorrer el menú con calma.</p></div>
    <div class="mc"><div class="mi">◈</div><div class="mn">Celebración</div><div class="mp">Desde 95 €</div><p class="md">Producto premium, brasa, platos de temporada y postre. El servicio más completo.</p></div>
  </div>
  <p class="mn2 fi">El precio final depende del número de personas, producto, ubicación y necesidades de servicio.</p>
</section>

<!-- GALERIA -->
<section id="galeria">
  <div class="fi" style="text-align:center;margin-bottom:3rem">
    <p class="sl">Galería</p>
    <h2 class="st">Platos y <em>momentos</em></h2>
    <div class="dv"></div>
  </div>
  <div class="gg fi">
    <div class="gi"><img src="https://mciccarelli2000.github.io/assets/galeria-pasta-chef.jpg" alt="Pasta" loading="lazy"/><div class="gc">Pasta fresca</div></div>
    <div class="gi"><img src="https://mciccarelli2000.github.io/assets/galeria-pescado-dorado.jpg" alt="Pescado" loading="lazy"/><div class="gc">Pescado dorado</div></div>
    <div class="gi"><img src="https://mciccarelli2000.github.io/assets/galeria-carne-cordero.jpg" alt="Cordero" loading="lazy"/><div class="gc">Carne y jugo</div></div>
    <div class="gi"><img src="https://mciccarelli2000.github.io/assets/galeria-pasta-trufa.jpg" alt="Trufa" loading="lazy"/><div class="gc">Pasta y trufa</div></div>
    <div class="gi"><img src="https://mciccarelli2000.github.io/assets/galeria-crudo-verde.jpg" alt="Crudo" loading="lazy"/><div class="gc">Crudos</div></div>
    <div class="gi"><img src="https://mciccarelli2000.github.io/assets/contacto-pasta-real.jpg" alt="Prep" loading="lazy"/><div class="gc">Preparación</div></div>
  </div>
</section>

<!-- TRAYECTORIA -->
<section id="tray">
  <div class="ti">
    <p class="sl fi">Trayectoria</p>
    <h2 class="st fi">Experiencia que se nota<br>en cada <em>detalle</em></h2>
    <div class="fi">
      <p>Mi recorrido profesional me ha llevado por cocinas exigentes, servicios de catering y proyectos gastronómicos donde la organización, el producto y el punto de cocción son tan importantes como el plato final.</p>
      <p>En Barcelona trabajé en el entorno Arola del Hotel Arts; más tarde dirigí cocina de catering en Le Chef. En Madrid estuve vinculado a HER, propuesta mediterránea con influencia mexicana de referencia en la ciudad.</p>
      <div class="tls">
        <a href="https://observaciongastronomica.com/2013/05/11/arola-hotel-arts-2/" target="_blank" rel="noopener" class="tl">Arola / Hotel Arts</a>
        <a href="https://theluxonomist.20minutos.es/gastronomia/restaurantes/le-chef-catering-laura-pi-y-sus-amorosos-bocados" target="_blank" rel="noopener" class="tl">Le Chef</a>
        <a href="https://www.neo2.com/restaurante-her/" target="_blank" rel="noopener" class="tl">HER Madrid</a>
      </div>
    </div>
  </div>
</section>

<!-- PROCESO -->
<section id="proceso">
  <div class="fi" style="text-align:center;margin-bottom:3rem">
    <p class="sl">El proceso</p>
    <h2 class="st">Menú cerrado, compra,<br>cocina y <em>servicio</em></h2>
    <div class="dv"></div>
  </div>
  <div class="pg fi">
    <div class="ps"><div class="pn">01</div><div class="pt">Consulta y propuesta</div><p class="pd">Definimos fecha, número de personas, estilo de menú y alergias. Recibes propuesta clara con precio y platos.</p></div>
    <div class="ps"><div class="pn">02</div><div class="pt">Compra y preparación</div><p class="pd">Me encargo de la selección de producto de temporada y la mise en place. Llego con todo organizado.</p></div>
    <div class="ps"><div class="pn">03</div><div class="pt">Cocina y recogida</div><p class="pd">Termino los platos en tu cocina y sirvo en mesa. Al finalizar dejo el área limpia y recogida.</p></div>
  </div>
</section>

<!-- ═══════════════════════════════════════
     SISTEMA DE RESERVAS + CALENDARIO
════════════════════════════════════════ -->
<section id="reserva">
  <div class="fi" style="text-align:center;margin-bottom:3.5rem">
    <p class="sl">Reservas</p>
    <h2 class="st">Elige tu fecha y<br><em style="color:var(--goldp)">solicita disponibilidad</em></h2>
    <div class="dv"></div>
  </div>

  <div class="booking-wrap">

    <!-- INFO + ESTADO -->
    <div class="fi">
      <div class="bk-info">
        <h3>Selecciona la fecha en el calendario y rellena el formulario. Te confirmo disponibilidad en menos de 2 horas.</h3>
        <div class="bk-dato">
          <div class="bk-ico"><svg viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M2.25 6.75c0 8.284 6.716 15 15 15h2.25a2.25 2.25 0 002.25-2.25v-1.372c0-.516-.351-.966-.852-1.091l-4.423-1.106c-.44-.11-.902.055-1.173.417l-.97 1.293c-.282.376-.769.542-1.21.38a12.035 12.035 0 01-7.143-7.143c-.162-.441.004-.928.38-1.21l1.293-.97c.363-.271.527-.734.417-1.173L6.963 3.102a1.125 1.125 0 00-1.091-.852H4.5A2.25 2.25 0 002.25 4.5v2.25z"/></svg></div>
          <div class="bk-txt"><strong>WhatsApp directo</strong><a href="https://wa.me/34630386059" target="_blank" rel="noopener">+34 630 386 059</a></div>
        </div>
        <div class="bk-dato">
          <div class="bk-ico"><svg viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 11-6 0 3 3 0 016 0z"/><path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1115 0z"/></svg></div>
          <div class="bk-txt"><strong>Zona de trabajo</strong>Madrid y alrededores</div>
        </div>
        <div class="bk-status">
          <div class="bk-status-title">Estado del sistema</div>
          <div class="bk-status-msg" id="sysStatus">Cargando disponibilidad…</div>
        </div>
      </div>
    </div>

    <!-- CALENDARIO + FORM -->
    <div class="fi">
      <!-- Calendario -->
      <div style="margin-bottom:1.4rem">
        <div class="cal-header">
          <button class="cal-nav" id="calPrev">‹</button>
          <div class="cal-title" id="calTitle"></div>
          <button class="cal-nav" id="calNext">›</button>
        </div>
        <div class="cal-grid" id="calDayNames"></div>
        <div class="cal-grid" id="calDays"></div>
        <div class="cal-legend">
          <div class="cal-leg"><span class="l-free"></span>Disponible</div>
          <div class="cal-leg"><span class="l-busy"></span>Reservado</div>
        </div>
      </div>

      <!-- Formulario -->
      <div class="rf" id="bookForm">
        <div class="rf-selected-date" id="selectedDateDisplay">
          <strong>Fecha seleccionada</strong>
          <span id="selDateText">— Elige una fecha en el calendario —</span>
        </div>
        <div class="rf-row">
          <div class="rf-field"><label>Nombre *</label><input id="bNombre" type="text" placeholder="Tu nombre"/></div>
          <div class="rf-field"><label>Teléfono *</label><input id="bTel" type="tel" placeholder="+34 600 000 000"/></div>
        </div>
        <div class="rf-row">
          <div class="rf-field"><label>Personas *</label><input id="bPax" type="number" min="2" max="50" placeholder="8"/></div>
          <div class="rf-field">
            <label>Tipo de evento *</label>
            <select id="bTipo">
              <option value="">Selecciona…</option>
              <option>Cena privada</option>
              <option>Comida privada</option>
              <option>Celebración</option>
              <option>Evento en finca</option>
              <option>Otro</option>
            </select>
          </div>
        </div>
        <div class="rf-field"><label>Menú preferido</label>
          <select id="bMenu">
            <option value="">Sin preferencia</option>
            <option>Selección (65€+/persona)</option>
            <option>Experiencia (75€+/persona)</option>
            <option>Celebración (95€+/persona)</option>
          </select>
        </div>
        <div class="rf-field"><label>Alergias / detalles</label><textarea id="bMsg" rows="3" placeholder="Alergias, lugar del evento, detalles importantes…"></textarea></div>
        <div class="rf-footer">
          <span class="rf-note">Respuesta en &lt; 2 horas</span>
          <button class="btn-book" id="btnBook" disabled>Solicitar fecha</button>
        </div>
      </div>
    </div>
  </div>

  <!-- Panel cómo funciona -->
  <div class="auto-panel show fi" style="margin-top:4rem">
    <p class="sl">Cómo funciona la reserva</p>
    <div class="auto-steps">
      <div class="auto-step">
        <div class="auto-num">01</div>
        <div class="auto-title">Seleccionas fecha</div>
        <div class="auto-desc">El calendario muestra en tiempo real qué fechas están libres y cuáles ya están reservadas. No puedes elegir una fecha ocupada.</div>
      </div>
      <div class="auto-step">
        <div class="auto-num">02</div>
        <div class="auto-title">Envías la solicitud</div>
        <div class="auto-desc">El formulario genera automáticamente un mensaje completo y te abre WhatsApp con todos los detalles de tu solicitud.</div>
      </div>
      <div class="auto-step">
        <div class="auto-num">03</div>
        <div class="auto-title">Confirmo en &lt; 2 h</div>
        <div class="auto-desc">Mauro revisa la solicitud, confirma disponibilidad y envía propuesta personalizada. Una vez confirmado, la fecha queda bloqueada.</div>
      </div>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="fl">Mauro Ciccarelli</div>
  <p class="fc">© 2025 · Chef privado a domicilio en Madrid</p>
  <a href="https://wa.me/34630386059" target="_blank" rel="noopener" class="fw">
    <svg width="13" height="13" viewBox="0 0 24 24" fill="currentColor"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347zM12 0C5.373 0 0 5.373 0 12c0 2.124.554 4.118 1.526 5.847L.057 23.882l6.198-1.455A11.934 11.934 0 0012 24c6.627 0 12-5.373 12-12S18.627 0 12 0zm0 21.818a9.796 9.796 0 01-5.034-1.386l-.359-.214-3.68.964.983-3.595-.234-.369A9.818 9.818 0 012.182 12C2.182 6.575 6.575 2.182 12 2.182c5.424 0 9.818 4.393 9.818 9.818 0 5.424-4.394 9.818-9.818 9.818z"/></svg>
    WhatsApp
  </a>
</footer>

<!-- MODAL CONFIRMACIÓN -->
<div class="confirm-modal" id="confirmModal">
  <div class="confirm-box">
    <button class="confirm-close" id="confClose">✕</button>
    <div class="confirm-icon">✅</div>
    <div class="confirm-title">Solicitud preparada</div>
    <p class="confirm-msg">Tu consulta está lista para enviarse por WhatsApp. Mauro la recibirá con todos los detalles y te confirmará en menos de 2 horas.</p>
    <div class="confirm-detail" id="confDetail"></div>
    <div class="confirm-actions">
      <button class="confirm-wa" id="confWA">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="currentColor"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347zM12 0C5.373 0 0 5.373 0 12c0 2.124.554 4.118 1.526 5.847L.057 23.882l6.198-1.455A11.934 11.934 0 0012 24c6.627 0 12-5.373 12-12S18.627 0 12 0zm0 21.818a9.796 9.796 0 01-5.034-1.386l-.359-.214-3.68.964.983-3.595-.234-.369A9.818 9.818 0 012.182 12C2.182 6.575 6.575 2.182 12 2.182c5.424 0 9.818 4.393 9.818 9.818 0 5.424-4.394 9.818-9.818 9.818z"/></svg>
        Enviar por WhatsApp
      </button>
      <button class="confirm-close2" id="confCancel">Cancelar</button>
    </div>
  </div>
</div>

<div class="toast" id="toast"></div>

<script>
// ══════════════════════════════════════════════
// SISTEMA DE RESERVAS CON CALENDARIO
// ══════════════════════════════════════════════

// Base de datos de fechas reservadas (localStorage — persiste en el navegador)
// Formato: "YYYY-MM-DD"
const STORAGE_KEY = 'mc_booked_dates';

function getBookedDates() {
  try {
    const raw = localStorage.getItem(STORAGE_KEY);
    return raw ? JSON.parse(raw) : [];
  } catch { return []; }
}

function addBookedDate(dateStr) {
  const dates = getBookedDates();
  if (!dates.includes(dateStr)) {
    dates.push(dateStr);
    localStorage.setItem(STORAGE_KEY, JSON.stringify(dates));
  }
}

// Para demo: pre-cargar algunas fechas como "reservadas"
(function seedDemoDates() {
  const existing = getBookedDates();
  if (existing.length === 0) {
    const today = new Date();
    const demos = [];
    // Simular 4 fechas reservadas en los próximos 60 días
    [7, 14, 21, 35].forEach(d => {
      const dt = new Date(today);
      dt.setDate(dt.getDate() + d);
      // Evitar domingos
      if (dt.getDay() !== 0) {
        demos.push(dt.toISOString().split('T')[0]);
      }
    });
    localStorage.setItem(STORAGE_KEY, JSON.stringify(demos));
  }
})();

// ── CALENDARIO ──
let calYear, calMonth, selectedDate = null;

const DAYS_ES = ['Lu','Ma','Mi','Ju','Vi','Sa','Do'];
const MONTHS_ES = ['Enero','Febrero','Marzo','Abril','Mayo','Junio','Julio','Agosto','Septiembre','Octubre','Noviembre','Diciembre'];

function initCal() {
  const now = new Date();
  calYear = now.getFullYear();
  calMonth = now.getMonth();
  renderCal();

  // Day names
  const dn = document.getElementById('calDayNames');
  DAYS_ES.forEach(d => {
    const el = document.createElement('div');
    el.className = 'cal-day-name';
    el.textContent = d;
    dn.appendChild(el);
  });
}

function renderCal() {
  document.getElementById('calTitle').textContent = MONTHS_ES[calMonth] + ' ' + calYear;
  const grid = document.getElementById('calDays');
  grid.innerHTML = '';

  const booked = getBookedDates();
  const today = new Date(); today.setHours(0,0,0,0);
  const first = new Date(calYear, calMonth, 1);
  // Monday-based: 0=Mon … 6=Sun
  let startDay = first.getDay(); // 0=Sun
  startDay = startDay === 0 ? 6 : startDay - 1;

  // Empty cells
  for (let i = 0; i < startDay; i++) {
    const el = document.createElement('div');
    el.className = 'cal-day empty';
    grid.appendChild(el);
  }

  const daysInMonth = new Date(calYear, calMonth + 1, 0).getDate();
  for (let d = 1; d <= daysInMonth; d++) {
    const date = new Date(calYear, calMonth, d);
    const dateStr = date.toISOString().split('T')[0];
    const el = document.createElement('div');
    el.textContent = d;

    const isToday = date.getTime() === today.getTime();
    const isPast = date < today;
    const isBooked = booked.includes(dateStr);
    const isSunday = date.getDay() === 0;
    const isSel = dateStr === selectedDate;

    if (isSel) el.className = 'cal-day selected';
    else if (isPast || isSunday) el.className = 'cal-day past';
    else if (isBooked) el.className = 'cal-day booked';
    else el.className = 'cal-day available';

    if (isToday) el.classList.add('today');

    if (el.classList.contains('available') || isSel) {
      el.addEventListener('click', () => selectDate(dateStr, date));
    }
    grid.appendChild(el);
  }

  updateStatus();
}

function selectDate(dateStr, dateObj) {
  selectedDate = dateStr;
  renderCal();

  const opts = { weekday:'long', day:'numeric', month:'long', year:'numeric' };
  const label = dateObj.toLocaleDateString('es-ES', opts);
  document.getElementById('selDateText').textContent = label.charAt(0).toUpperCase() + label.slice(1);
  document.getElementById('btnBook').disabled = false;
}

function updateStatus() {
  const booked = getBookedDates();
  const now = new Date();
  const upcoming = booked.filter(d => new Date(d) >= now).length;
  const msg = upcoming === 0
    ? 'Todas las fechas disponibles. ¡Buen momento para reservar!'
    : `${upcoming} fecha${upcoming > 1 ? 's' : ''} reservada${upcoming > 1 ? 's' : ''} próximamente. Consulta el calendario para ver disponibilidad.`;
  document.getElementById('sysStatus').textContent = msg;
}

document.getElementById('calPrev').addEventListener('click', () => {
  calMonth--; if (calMonth < 0) { calMonth = 11; calYear--; } renderCal();
});
document.getElementById('calNext').addEventListener('click', () => {
  calMonth++; if (calMonth > 11) { calMonth = 0; calYear++; } renderCal();
});

initCal();

// ── FORMULARIO → WHATSAPP ──
let pendingWAUrl = '';

document.getElementById('btnBook').addEventListener('click', () => {
  const nombre = document.getElementById('bNombre').value.trim();
  const tel    = document.getElementById('bTel').value.trim();
  const pax    = document.getElementById('bPax').value;
  const tipo   = document.getElementById('bTipo').value;
  const menu   = document.getElementById('bMenu').value;
  const msg    = document.getElementById('bMsg').value.trim();

  if (!nombre) { showToast('Por favor indica tu nombre'); return; }
  if (!tel)    { showToast('Por favor indica tu teléfono'); return; }
  if (!pax)    { showToast('Indica el número de personas'); return; }
  if (!tipo)   { showToast('Selecciona el tipo de evento'); return; }

  const dateDisp = document.getElementById('selDateText').textContent;

  let text = `🍽️ *Solicitud de servicio de chef privado*\n\n`;
  text += `👤 *Nombre:* ${nombre}\n`;
  text += `📞 *Teléfono:* ${tel}\n`;
  text += `📅 *Fecha:* ${dateDisp}\n`;
  text += `👥 *Personas:* ${pax}\n`;
  text += `🎉 *Tipo:* ${tipo}\n`;
  if (menu) text += `🍷 *Menú:* ${menu}\n`;
  if (msg)  text += `\n📝 *Detalles:* ${msg}`;
  text += `\n\n_Solicitud enviada desde maurociccarelli.com_`;

  pendingWAUrl = `https://wa.me/34630386059?text=${encodeURIComponent(text)}`;

  // Mostrar resumen en modal
  document.getElementById('confDetail').innerHTML = `
    <p><strong>Fecha:</strong> ${dateDisp}</p>
    <p><strong>Personas:</strong> ${pax} · <strong>Evento:</strong> ${tipo}</p>
    ${menu ? `<p><strong>Menú:</strong> ${menu}</p>` : ''}
    ${msg ? `<p><strong>Detalles:</strong> ${msg}</p>` : ''}
  `;
  document.getElementById('confirmModal').classList.add('show');
});

document.getElementById('confWA').addEventListener('click', () => {
  // Bloquear la fecha en el calendario
  if (selectedDate) addBookedDate(selectedDate);
  window.open(pendingWAUrl, '_blank');
  document.getElementById('confirmModal').classList.remove('show');
  renderCal();
  showToast('✓ Solicitud enviada — Mauro te confirmará en breve');
  // Reset form
  ['bNombre','bTel','bPax','bMsg'].forEach(id => document.getElementById(id).value = '');
  document.getElementById('bTipo').selectedIndex = 0;
  document.getElementById('bMenu').selectedIndex = 0;
  document.getElementById('btnBook').disabled = true;
  document.getElementById('selDateText').textContent = '— Elige una fecha en el calendario —';
  selectedDate = null;
  renderCal();
});

['confClose','confCancel'].forEach(id =>
  document.getElementById(id).addEventListener('click', () =>
    document.getElementById('confirmModal').classList.remove('show')
  )
);

// ── NAV ──
window.addEventListener('scroll', () =>
  document.getElementById('nav').classList.toggle('s', scrollY > 60), { passive: true }
);
document.getElementById('hbg').addEventListener('click', () => document.getElementById('mob').classList.add('o'));
document.getElementById('mbc').addEventListener('click', () => document.getElementById('mob').classList.remove('o'));
document.querySelectorAll('.ml').forEach(l => l.addEventListener('click', () => document.getElementById('mob').classList.remove('o')));

// ── FADE IN ──
const obs = new IntersectionObserver(entries =>
  entries.forEach(e => { if (e.isIntersecting) { e.target.classList.add('v'); obs.unobserve(e.target); } })
, { threshold: 0.1 });
document.querySelectorAll('.fi').forEach(el => obs.observe(el));

// ── TOAST ──
function showToast(msg) {
  const t = document.getElementById('toast');
  t.textContent = msg;
  t.classList.add('show');
  setTimeout(() => t.classList.remove('show'), 3500);
}
</script>
</body>
</html>
