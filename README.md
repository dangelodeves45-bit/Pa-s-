<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>República de Bodvern — Site Oficial</title>
  <meta name="description" content="Site oficial fictício da República de Bodvern: história, governo, economia, defesa, saúde, cultura e mais." />
  <style>
    :root{
      --primary:#0b5bd3;
      --primary-dark:#0847a5;
      --accent:#e63946;
      --accent-2:#ff6b6b;
      --ink:#1f2937;
      --bg:#f4f7fb;
      --card:#ffffff;
    }
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, Noto Sans, "Apple Color Emoji","Segoe UI Emoji";
      color:var(--ink);
      background:var(--bg);
      line-height:1.6;
    }
    a{color:var(--primary); text-decoration:none}
    a:hover{text-decoration:underline}
    header{
      position:sticky; top:0; z-index:1000;
      background:linear-gradient(90deg,var(--primary),var(--primary-dark));
      color:#fff; box-shadow:0 6px 18px rgba(0,0,0,.15);
    }
    .nav{max-width:1100px; margin:0 auto; padding:12px 16px; display:flex; align-items:center; gap:16px}
    .brand{display:flex; align-items:center; gap:10px; font-weight:700; letter-spacing:.4px}
    .brand img{width:28px; height:28px}
    .links{margin-left:auto; display:flex; gap:16px; flex-wrap:wrap}
    .links a{color:#fff; font-weight:600; opacity:.95}
    .links a:hover{opacity:1}
    .hero{
      background: radial-gradient(60% 80% at 70% 20%, #e8efff, #f7fbff 60%, #ffffff);
      padding: 36px 16px 12px;
      border-bottom:1px solid #e6ecf5;
    }
    .hero-inner{max-width:1100px; margin:0 auto; display:grid; grid-template-columns: 1.1fr .9fr; gap:24px; align-items:center}
    .hero h1{margin:.2em 0 .2em; font-size:clamp(28px,4vw,44px)}
    .pill{display:inline-block; background:#fff; border:1px solid #e5ecf8; padding:6px 12px; border-radius:999px; font-size:14px}
    .cta{display:flex; gap:12px; margin-top:12px}
    .btn{
      border:none; padding:10px 16px; border-radius:10px; cursor:pointer; font-weight:700;
      box-shadow:0 6px 18px rgba(11,91,211,.18);
      background:linear-gradient(180deg,#ffffff,#f4f7ff);
    }
    .btn.primary{background:linear-gradient(180deg,#2a72ff,#0b5bd3); color:#fff}
    .flag-wrap{background:#fff; border:1px solid #e8eef7; border-radius:14px; padding:14px; box-shadow:0 12px 28px rgba(0,0,0,.06)}
    .section{max-width:1100px; margin:26px auto; padding:0 16px}
    .grid{display:grid; grid-template-columns:repeat(12, 1fr); gap:16px}
    .card{
      grid-column: span 6; background:var(--card); border-radius:14px; padding:18px;
      box-shadow:0 10px 24px rgba(0,0,0,.06); border:1px solid #eef2f7;
    }
    .card h2{margin:6px 0 8px; color:var(--primary-dark)}
    .facts{display:grid; grid-template-columns:repeat(2,1fr); gap:10px; margin-top:8px}
    .fact{background:#f7faff; border:1px solid #e6eefc; padding:10px; border-radius:10px; font-size:14px}
    .footer{
      margin-top:28px; padding:24px 16px; background:#0f172a; color:#cbd5e1; text-align:center
    }
    .mobile{display:none}
    @media (max-width:900px){
      .hero-inner{grid-template-columns:1fr}
      .card{grid-column: span 12}
      .facts{grid-template-columns:1fr}
      .links{display:none}
      .mobile{display:inline-flex; margin-left:auto}
    }
    .flag svg{width:100%; height:auto; border-radius:10px; border:2px solid #1b1b1b}
  </style>
</head>
<body>
  <header>
    <nav class="nav">
      <div class="brand">
        <img alt="Selo de Bodvern" src="data:image/svg+xml;utf8,..."/>
        <span>República de Bodvern</span>
      </div>
      <div class="links">
        <a href="#historia">História</a>
        <a href="#governo">Governo</a>
        <a href="#economia">Economia</a>
        <a href="#defesa">Defesa</a>
        <a href="#saude">Saúde</a>
        <a href="#cultura">Cultura</a>
        <a href="#dados">Dados</a>
        <a href="#contato">Contato</a>
      </div>
      <button class="btn mobile" onclick="document.querySelector('.links')?.classList.toggle('show')">Menu</button>
    </nav>
  </header>

  <!-- Hero e Bandeira -->
  <section class="hero">
    <div class="hero-inner">
      <div>
        <span class="pill">Portal Oficial • 2025</span>
        <h1>Bem-vindo(a) à República de Bodvern</h1>
        <p>Uma nação de união, coragem e futuro. Criada por <strong>D'angelo Giovanne Estigarribia Deves</strong>. Conheça nossa história, nossos avanços e a nova bandeira nacional — inspirada nos princípios de liberdade e progresso.</p>
        <div class="cta">
          <a class="btn primary" href="#dados">Ver dados do país</a>
          <a class="btn" href="#historia">Explorar história</a>
        </div>
      </div>
      <div class="flag-wrap">
        <div class="flag">
          <!-- Bandeira inspirada nos EUA -->
          <svg viewBox="0 0 1140 600" xmlns="http://www.w3.org/2000/svg">
            <defs>
              <linearGradient id="r" x1="0" x2="1">
                <stop offset="0%" stop-color="#e63946"/>
                <stop offset="100%" stop-color="#ff7b7b"/>
              </linearGradient>
              <linearGradient id="b" x1="0" x2="1">
                <stop offset="0%" stop-color="#0b5bd3"/>
                <stop offset="100%" stop-color="#6aa3ff"/>
              </linearGradient>
            </defs>
            <rect width="1140" height="600" fill="#ffffff"/>
            <!-- Listras -->
            <rect x="0" y="0" width="1140" height="46.15" fill="url(#r)"/>
            <rect x="0" y="46.15" width="1140" height="46.15" fill="#f2f6ff"/>
            <rect x="0" y="92.3" width="1140" height="46.15" fill="url(#r)"/>
            <rect x="0" y="138.45" width="1140" height="46.15" fill="#f2f6ff"/>
            <rect x="0" y="184.6" width="1140" height="46.15" fill="url(#r)"/>
            <rect x="0" y="230.75" width="1140" height="46.15" fill="#f2f6ff"/>
            <rect x="0" y="276.9" width="1140" height="46.15" fill="url(#r)"/>
            <rect x="0" y="323.05" width="1140" height="46.15" fill="#f2f6ff"/>
            <rect x="0" y="369.2" width="1140" height="46.15" fill="url(#r)"/>
            <rect x="0" y="415.35" width="1140" height="46.15" fill="#f2f6ff"/>
            <rect x="0" y="461.5" width="1140" height="46.15" fill="url(#r)"/>
            <rect x="0" y="507.65" width="1140" height="46.15" fill="#f2f6ff"/>
            <rect x="0" y="553.8" width="1140" height="46.15" fill="url(#r)"/>
            <rect x="0" y="0" width="456" height="336" fill="url(#b)"/>
          </svg>
        </div>
      </div>
    </div>
  </section>

  <!-- Seções -->
  <section id="historia" class="section">
    <div class="grid">
      <div class="card" style="grid-column:span 7">
        <h2>📜 História</h2>
        <p>Fundada por navegadores há mais de seis séculos, Bodvern consolidou uma identidade própria baseada em coragem, união e inovação.</p>
      </div>
      <div class="card" style="grid-column:span 5">
        <h2>📌 Marcos</h2>
        <ul>
          <li>Unificação regional e carta magna (século XV).</li>
          <li>Reformas educacionais e científicas (século XIX).</li>
          <li>Programa nacional de energia limpa (século XXI).</li>
        </ul>
      </div>
    </div>
  </section>

  <section id="governo" class="section">
    <div class="grid">
      <div class="card">
        <h2>🏛️ Governo</h2>
        <p>República constitucional com equilíbrio entre poderes, transparência e democracia participativa.</p>
      </div>
      <div class="card">
        <h2>⚖️ Direitos</h2>
        <p>Liberdades civis, inclusão social e combate à discriminação.</p>
      </div>
    </div>
  </section>

  <section id="economia" class="section">
    <div class="grid">
      <div class="card">
        <h2>💹 Economia</h2>
        <p>Focada em tecnologia limpa, biotecnologia, manufatura avançada e economia criativa.</p>
      </div>
      <div class="card">
        <h2>🔌 Energia</h2>
        <p>Matriz renovável: eólica, solar e hidrelétrica de baixo impacto.</p>
      </div>
    </div>
  </section>

  <section id="defesa" class="section">
    <div class="grid">
      <div class="card">
        <h2>🛡️ Defesa</h2>
        <p>Força militar moderna, cibersegurança, defesa aérea e marítima, priorizando paz e proteção humanitária.</p>
      </div>
      <div class="card">
        <h2>🛰️ Tecnologia</h2>
        <p>Drones, satélites e IA para vigilância, resgate e inteligência.</p>
      </div>
    </div>
  </section>

  <section id="saude" class="section">
    <div class="grid">
      <div class="card">
        <h2>⚕️ Saúde &amp; Medicina</h2>
        <p>Avanços em biotecnologia, medicina regenerativa e IA clínica para diagnósticos precisos.</p>
      </div>
      <div class="card">
        <h2>🧬 Pesquisa</h2>
        <p>Centros de excelência em genética, próteses neurais e terapias personalizadas.</p>
      </div>
    </div>
  </section>

  <section id="cultura" class="section">
    <div class="grid">
      <div class="card">
        <h2>🎭 Cultura</h2>
        <p>Festivais nacionais, música polifônica, gastronomia de fusão e patrimônio preservado.</p>
      </div>
      <div class="card">
        <h2>📚 Educação</h2>
        <p>Escolas STEAM, universidades com laboratórios abertos e incentivo ao empreendedorismo.</p>
      </div>
    </div>
  </section>

  <section id="dados" class="section">
    <div class="grid">
      <div class="card" style="grid-column:span 7">
        <h2>📊 Dados do País</h2>
        <div class="facts">
          <div class="fact"><strong>Área:</strong> ~480.000 km²</div>
          <div class="fact"><strong>População:</strong> ~28 milhões</div>
          <div class="fact"><strong>Capital:</strong> Værin</div>
          <div class="fact"><strong>Idioma:</strong> Bodverniano (cooficiais: PT, EN)</div>
          <div class="fact"><strong>Moeda:</strong> Coroa de Bodvern (BVC)</div>
          <div class="fact"><strong>PIB:</strong> BVC 1,2 tri</div>
        </div>
      </div>
      <div class="card" style="grid-column:span 5">
        <h2>🌿 Sustentabilidade</h2>
        <p>Neutralidade climática, reflorestamento costeiro, transporte limpo e economia circular.</p>
      </div>
    </div>
  </section>

  <section id="contato" class="section">
    <div class="grid">
      <div class="card" style="grid-column:span 12">
        <h2>✉️ Contato</h2>
        <p>Site criado por <strong>D'angelo Giovanne Estigarribia Deves</strong>. Fictício para demonstração.</p>
        <form onsubmit="event.preventDefault(); alert('Mensagem enviada! (fictício)');">
          <div style="display:grid; grid-template-columns:1fr 1fr; gap:10px">
            <input required placeholder="Seu nome" style="padding:10px; border:1px solid #dbe5f3; border-radius:8px"/>
            <input required type="email" placeholder="Seu e-mail" style="padding:10px; border:1px solid #dbe5f3; border-radius:8px"/>
          </div>
          <textarea required placeholder="Sua mensagem" rows="4" style="margin-top:10px; width:100%; padding:10px; border:1px solid #dbe5f3; border-radius:8px"></textarea>
          <div style="margin-top:10px">
            <button class="btn primary" type="submit">Enviar</button>
          </div>
        </form>
      </div>
    </div>
  </section>

  <footer class="footer">
    <small>© 2025 República de Bodvern — Criado por D'angelo Giovanne Estigarribia Deves</small>
  </footer>
</body>
</html>
