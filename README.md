[recuerdos.html](https://github.com/user-attachments/files/27561987/recuerdos.html)
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Recuerdos premium para Alejandra</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Great+Vibes&family=Playfair+Display:wght@500;600;700&display=swap" rel="stylesheet">
  <style>
    :root{--bg1:#220b16;--bg2:#12060c;--panel:rgba(67,23,45,.86);--line:rgba(255,185,208,.16);--text:#f9e8ef;--muted:#efc9d6;--rose:#d34f7c;--rose2:#ff95bf;--gold:#ebc993;--paper:#fff7ee;--ink:#62384a;--shadow:0 24px 70px rgba(0,0,0,.34);--radius:30px}
    *{box-sizing:border-box;margin:0;padding:0}
    body{min-height:100vh;font-family:'Cormorant Garamond',serif;color:var(--text);background:radial-gradient(circle at top left, rgba(255,160,204,.12), transparent 18%),radial-gradient(circle at top right, rgba(235,201,147,.1), transparent 20%),linear-gradient(180deg,var(--bg1),var(--bg2));overflow-x:hidden}
    .floating-hearts{position:fixed;inset:0;pointer-events:none;overflow:hidden;z-index:0}
    .floating-hearts span{position:absolute;bottom:-40px;width:18px;height:18px;border-radius:4px;background:linear-gradient(180deg,var(--rose2),var(--rose));transform:rotate(45deg);opacity:0;animation:heartRise linear infinite;filter:drop-shadow(0 0 8px rgba(255,105,165,.28))}
    .floating-hearts span::before,.floating-hearts span::after{content:'';position:absolute;width:18px;height:18px;background:inherit;border-radius:50%}
    .floating-hearts span::before{left:-9px}.floating-hearts span::after{top:-9px}
    .floating-hearts span:nth-child(1){left:3%;animation-duration:11s;animation-delay:-2s}.floating-hearts span:nth-child(2){left:9%;animation-duration:9.8s;animation-delay:-6s}.floating-hearts span:nth-child(3){left:16%;animation-duration:12.4s;animation-delay:-3s}.floating-hearts span:nth-child(4){left:24%;animation-duration:10.3s;animation-delay:-8s}.floating-hearts span:nth-child(5){left:31%;animation-duration:13s;animation-delay:-5s}.floating-hearts span:nth-child(6){left:39%;animation-duration:9.5s;animation-delay:-7s}.floating-hearts span:nth-child(7){left:47%;animation-duration:12.8s;animation-delay:-1s}.floating-hearts span:nth-child(8){left:55%;animation-duration:10.8s;animation-delay:-4s}.floating-hearts span:nth-child(9){left:63%;animation-duration:11.5s;animation-delay:-9s}.floating-hearts span:nth-child(10){left:71%;animation-duration:12.6s;animation-delay:-2.5s}.floating-hearts span:nth-child(11){left:80%;animation-duration:10.1s;animation-delay:-6.5s}.floating-hearts span:nth-child(12){left:88%;animation-duration:13.4s;animation-delay:-3.5s}.floating-hearts span:nth-child(13){left:95%;animation-duration:11.7s;animation-delay:-8.2s}
    @keyframes heartRise{0%{transform:translateY(0) scale(.55) rotate(45deg);opacity:0}10%{opacity:.95}70%{opacity:.65}100%{transform:translateY(-120vh) scale(1.28) rotate(45deg);opacity:0}}
    .page{width:min(100%,1180px);margin:0 auto;padding:34px 18px 60px;position:relative;z-index:1}
    .hero{text-align:center;margin-bottom:28px}.eyebrow{font:600 .82rem/1.2 'Playfair Display',serif;letter-spacing:.35em;text-transform:uppercase;color:#f5dce5;margin-bottom:12px}
    h1{font-family:'Great Vibes',cursive;font-size:clamp(3.2rem,2.3rem + 4vw,5.6rem);font-weight:400;text-shadow:0 0 22px rgba(255,180,205,.12)}
    .sub{max-width:820px;margin:10px auto 0;color:#f0dde5;font-size:1.22rem}
    .panel{background:linear-gradient(180deg, rgba(67,23,45,.82), rgba(37,13,27,.9));border:1px solid var(--line);border-radius:var(--radius);box-shadow:var(--shadow);backdrop-filter:blur(10px)}
    .music-card{padding:22px;margin-bottom:24px}.player-top{display:grid;grid-template-columns:56px 1fr auto;gap:16px;align-items:center}.icon-wrap{width:56px;height:56px;border-radius:50%;display:grid;place-items:center;background:radial-gradient(circle, rgba(255,111,167,.28), rgba(255,111,167,.08));box-shadow:0 0 22px rgba(255,111,167,.16)}
    .music-card h2{font:600 1.42rem/1.2 'Playfair Display',serif;letter-spacing:.04em;text-transform:uppercase}.tiny,.timer{color:var(--muted);font-size:1rem}.audio-box{margin-top:16px;padding:15px;border-radius:22px;background:linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.02));border:1px solid rgba(255,255,255,.08)}.audio-box p{text-align:center;color:#f0d3dc;margin-bottom:10px}.audio-box audio{width:100%}
    .intro{padding:22px;margin-bottom:24px;text-align:center}.intro h3{font-family:'Great Vibes',cursive;font-size:clamp(2.1rem,1.7rem + 1.8vw,3.4rem);font-weight:400}.intro p{color:#f0d9e2;font-size:1.12rem;margin-top:6px}
    .cards{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
    .memory-card{position:relative;height:430px;perspective:1400px}
    .memory-btn{position:absolute;inset:0;width:100%;height:100%;border:none;background:none;padding:0;cursor:pointer;border-radius:28px}
    .memory-inner{position:relative;width:100%;height:100%;transform-style:preserve-3d;transition:transform .9s cubic-bezier(.2,.8,.2,1)}
    .memory-card.flipped .memory-inner{transform:rotateY(180deg)}
    .memory-face{position:absolute;inset:0;backface-visibility:hidden;border-radius:28px;overflow:hidden;box-shadow:0 18px 35px rgba(0,0,0,.28)}
    .memory-front{background:#1e0d14}.memory-front img{width:100%;height:100%;object-fit:cover;display:block;transition:transform .45s ease, filter .45s ease}.memory-card:hover .memory-front img{transform:scale(1.03);filter:saturate(1.05)}
    .memory-front::before{content:'';position:absolute;inset:0;background:linear-gradient(180deg, rgba(255,255,255,.08), transparent 30%, transparent 70%, rgba(0,0,0,.28));pointer-events:none}
    .memory-front::after{content:'Toca para leer';position:absolute;left:16px;bottom:16px;padding:8px 14px;border-radius:999px;background:rgba(18,6,13,.62);border:1px solid rgba(255,255,255,.16);color:#fff;font:600 .85rem/1 'Playfair Display',serif;letter-spacing:.08em;text-transform:uppercase}
    .memory-back{transform:rotateY(180deg);background:linear-gradient(180deg, rgba(255,255,255,.16), rgba(255,255,255,0) 18%),radial-gradient(circle at top left, rgba(205,178,145,.12), transparent 28%),linear-gradient(180deg, var(--paper), #fbf3e8 56%, #f2e0ca 100%);color:var(--ink);padding:28px 22px;display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:center;border:1px solid rgba(130,92,61,.12)}
    .memory-back::before{content:'';position:absolute;inset:0;background-image:radial-gradient(rgba(116,86,62,.06) .6px, transparent .9px);background-size:12px 12px;opacity:.24;pointer-events:none}
    .memory-back::after{content:'';position:absolute;inset:10px;border:1px solid rgba(139,98,69,.1);border-radius:18px;pointer-events:none}
    .memory-back h4{font-family:'Great Vibes',cursive;font-size:2.45rem;color:#8f4b63;font-weight:400;margin-bottom:12px;position:relative;z-index:1}
    .memory-back p{font-size:1.28rem;line-height:1.55;position:relative;z-index:1}
    .memory-back .sign{margin-top:12px;font:600 .86rem/1.2 'Playfair Display',serif;letter-spacing:.18em;text-transform:uppercase;color:#b38459;position:relative;z-index:1}
    .footer-note{text-align:center;color:#efd9e1;font-size:1rem;margin-top:18px}
    @media (max-width:980px){.cards{grid-template-columns:1fr}.memory-card{height:470px}}
  </style>
</head>
<body>
  <div class="floating-hearts" aria-hidden="true"><span></span><span></span><span></span><span></span><span></span><span></span><span></span><span></span><span></span><span></span><span></span><span></span><span></span></div>
  <div class="page">
    <header class="hero">
      <div class="eyebrow">Recuerdos con amor</div>
      <h1>Para Alejandra Moscoso Garate</h1>
      <p class="sub">Ahora con mucho mas corazones y recuerdos giratorios, cada aventura con una dedicatoria especial escrita. No te olvides de colocar PLAY A LA CANCIÓN</p>
    </header>

    <section class="panel music-card">
      <div class="player-top">
        <div class="icon-wrap" aria-hidden="true">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round">
            <path d="M16 9a4 4 0 0 1-8 0"/><path d="M12 5c3 0 6 2 6 5v6a2 2 0 0 1-2 2H8a2 2 0 0 1-2-2v-6c0-3 3-5 6-5Z"/><path d="M9 14h.01M15 14h.01"/>
          </svg>
        </div>
        <div>
          <h2>La mamá que elegí para mis hijos</h2>
          <p class="tiny">Canción integrada en este recuerdo</p>
        </div>
        <div class="timer">Auto</div>
      </div>
      <div class="audio-box">
        <p>La canción acompaña cada imagen y cada palabra dedicada para ti.</p>
        <audio controls autoplay loop preload="auto">
          <source src="./La-mama-que-elegi-para-mis-hijos.mp3" type="audio/mpeg">
          Tu navegador no soporta audio HTML.
        </audio>
      </div>
    </section>

    <section class="panel intro">
      <h3>Postales</h3>
      <p>No olvides presionar cada imagen para girarla mi amorcito. La parte de atrás tiene una delicada leyenda para ti Alejandra Moscoso Garate.</p>
    </section>

    <section class="cards">
      <article class="memory-card"><button class="memory-btn" type="button" aria-label="Girar recuerdo de Bariloche"><div class="memory-inner"><div class="memory-face memory-front"><img src="./514263.jpg" alt="Foto familiar en Bariloche" /></div><div class="memory-face memory-back"><h4>Bariloche</h4><p>A tu lado cada viaje se vuelve inolvidable, porque en cada paisaje lo más hermoso siempre termina siendo tu presencia y tu manera de llenar todo de amor.</p><div class="sign">C.A.I.S</div></div></div></button></article>
      <article class="memory-card"><button class="memory-btn" type="button" aria-label="Girar recuerdo frente al lago"><div class="memory-inner"><div class="memory-face memory-front"><img src="./514353.jpg" alt="Foto abrazados frente al lago" /></div><div class="memory-face memory-back"><h4>Tu abrazo</h4><p>En tus brazos encuentro calma y hogar. Cada instante contigo se queda guardado en mi corazón como uno de los recuerdos más bonitos de mi vida.</p><div class="sign">C.A.I.S</div></div></div></button></article>
      <article class="memory-card"><button class="memory-btn" type="button" aria-label="Girar recuerdo en el bosque"><div class="memory-inner"><div class="memory-face memory-front"><img src="./514357.jpg" alt="Foto especial en el bosque" /></div><div class="memory-face memory-back"><h4>Mi amor</h4><p>Eres fuerza, ternura y belleza en una sola alma. Cada recuerdo contigo se vuelve un tesoro y cada día a tu lado confirma cuánto te amo, Alejandra.</p><div class="sign">C.A.I.S</div></div></div></button></article>
      <article class="memory-card"><button class="memory-btn" type="button" aria-label="Girar recuerdo en el puente"><div class="memory-inner"><div class="memory-face memory-front"><img src="./512675.jpg" alt="Foto en el puente ferroviario" /></div><div class="memory-face memory-back"><h4>Contigo</h4><p>Caminar contigo incluso sobre los caminos más largos se siente fácil, porque tu compañía convierte cualquier trayecto en algo seguro, bonito y especial.</p><div class="sign">C.A.I.S</div></div></div></button></article>
      <article class="memory-card"><button class="memory-btn" type="button" aria-label="Girar recuerdo junto al lago azul"><div class="memory-inner"><div class="memory-face memory-front"><img src="./514235.jpg" alt="Foto junto al lago azul" /></div><div class="memory-face memory-back"><h4>Tu esencia</h4><p>Hay una paz en ti que se parece a estos paisajes: serena, inmensa y hermosa. Por eso estar contigo siempre se siente como respirar amor con calma.</p><div class="sign">C.A.I.S</div></div></div></button></article>
      <article class="memory-card"><button class="memory-btn" type="button" aria-label="Girar recuerdo familiar en mirador"><div class="memory-inner"><div class="memory-face memory-front"><img src="./505578.jpg" alt="Foto familiar en mirador" /></div><div class="memory-face memory-back"><h4>Nuestra familia</h4><p>Verte junto a quienes amas me recuerda lo afortunado que soy. Eres el corazón de esta historia, el abrazo que une y la luz más bonita de nuestro hogar.</p><div class="sign">C.A.I.S</div></div></div></button></article>
    </section>

    <p class="footer-note">Si la música no inicia sola, toca el reproductor una vez. Después puedes girar cada postal para leer su mensaje.</p>
  </div>
  <script>
    document.querySelectorAll('.memory-card').forEach(card => {
      const btn = card.querySelector('.memory-btn');
      btn.addEventListener('click', () => card.classList.toggle('flipped'));
    });
  </script>
</body>
</html>
[La-mama-que-elegi-para-mis-hijos.mp3](https://github.com/user-attachments/files/27561989/La-mama-que-elegi-para-mis-hijos.mp3)
