<!doctype html>
<html lang="fr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Test CV — Alignement</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=Merriweather:wght@300;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --accent:#7c3aed;
      --accent2:#e11d48;
      --muted:#6b7280;
      --bg:#f8f5fb;
      --paper:#ffffff;
      --text:#111827;
      --radius:12px;
      --gap:24px;
      --max-width:1000px;
      --shadow: 0 6px 18px rgba(17,24,39,0.06);
      --accent-gradient: linear-gradient(90deg,var(--accent),var(--accent2));
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:'Poppins',system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;color:var(--text);background:linear-gradient(180deg,var(--bg),#ffffff);-webkit-font-smoothing:antialiased}
    a{color:var(--accent);text-decoration:none}
    /* CONTENEUR PRINCIPAL : grid + alignement en haut */
    .container{
      max-width:var(--max-width);
      margin:28px auto;
      display:grid;
      grid-template-columns:320px 1fr;
      gap:var(--gap);
      padding:28px;
      align-items: start;    /* aligne les colonnes en haut */
      align-content: start;
    }
    /* forcer chaque colonne à démarrer en haut (robuste) */
    .sidebar, .content { align-self: start; }
    /* Sidebar : enfants alignés vers le haut, photo centrée horizontalement */
    .sidebar{
      background: linear-gradient(180deg, rgba(124,58,237,0.06), rgba(225,29,72,0.02));
      padding:24px;
      border-radius:var(--radius);
      box-shadow:var(--shadow);
      display:flex;
      flex-direction:column;
      align-items:flex-start; /* <-- IMPORTANT : évite le centrage vertical des éléments */
      gap:14px;
    }
    .photo{
      width:120px;height:120px;border-radius:50%;background-size:cover;background-position:center;border:4px solid rgba(255,255,255,0.6);box-shadow:0 6px 18px rgba(17,24,39,0.08);
      margin: 0 auto; /* centre horizontalement la photo tout en gardant les autres éléments alignés en haut */
    }
    .name{margin:0;font-weight:700;font-size:1.25rem}
    .role{margin:0;color:var(--muted);font-weight:600;font-size:0.95rem}
    .sidebar h3{width:100%;margin-top:12px;margin-bottom:8px;font-size:0.95rem;color:var(--accent)}
    .contact ul, .languages ul{list-style:none;padding:0;margin:0;font-size:0.9rem;color:var(--muted)}
    .contact li{margin:6px 0}
    .skills .skill{width:100%;margin-bottom:10px}
    .skill span{display:block;font-size:0.9rem;margin-bottom:6px}
    .bar{background:linear-gradient(90deg,#fff,#fff);height:8px;border-radius:999px;padding:2px;background-clip:padding-box;border:1px solid rgba(0,0,0,0.04)}
    .fill{height:100%;border-radius:999px;background:var(--accent-gradient);box-shadow:0 4px 10px rgba(124,58,237,0.12)}
    /* Content */
    .content{
      background:var(--paper);
      padding:28px;
      border-radius:var(--radius);
      box-shadow:var(--shadow);
      display:flex;
      flex-direction:column;
      gap:18px;
    }
    /* styles restants (abrégés pour le test) */
    .intro .summary-title{font-family:'Merriweather',serif;color:var(--accent);margin:0;font-weight:700}
    .summary{margin:6px 0 0;color:var(--muted);line-height:1.5}
    h3{margin:0 0 12px 0;color:#0f172a}
    .card{background:linear-gradient(180deg,#fff,#fbfbff);padding:12px;border-radius:10px;border:1px solid rgba(15,23,42,0.03)}
    .project-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(180px,1fr));gap:12px}
    .proj{background:linear-gradient(180deg,#fff,#fcfdff);padding:10px;border-radius:10px;border:1px solid rgba(15,23,42,0.03)}
    /* responsive */
    @media (max-width:880px){
      .container{grid-template-columns:1fr;padding:18px}
      .sidebar{flex-direction:row;gap:12px;align-items:flex-start;padding:18px}
      .sidebar .photo{width:80px;height:80px}
      .name{font-size:1rem}
    }
  </style>
</head>
<body>
  <div class="container">
    <aside class="sidebar">
      <div class="photo" aria-hidden="true" style="background-image: url('https://via.placeholder.com/300');"></div>
      <h2 class="name">Emeline Da Silva</h2>
      <p class="role">Lycéenne / Terminal</p>
      <section class="contact">
        <h3>Contact</h3>
        <ul>
          <li>Email: <a href="mailto:emelineds85@gmail.com">emelineds85@gmail.com</a></li>
          <li>Vendée, France</li>
          <li><a href="#">portfolio.link</a></li>
        </ul>
      </section>
    </aside>
    <main class="content">
      <header class="intro">
        <p class="summary-title">Résumé</p>
        <p class="summary">Etudiante en Informatique et en maths, passionnée par la programmation.</p>
      </header>
      <section class="work">
        <h3>Formation</h3>
        <div class="card small">
          <h4>Baccalauréat Général — Lycée</h4>
          <p class="meta">2026/2027 — Montaigu</p>
        </div>
      </section>
      <section class="projects">
        <h3>Projets</h3>
        <div class="project-grid">
          <div class="proj"><h5>Projet Python</h5><p>Mon jeu pendu (NSI).</p></div>
          <div class="proj"><h5>Projet HTML</h5><p>Page web.</p></div>
        </div>
      </section>
    </main>
  </div>
</body>
</html>
