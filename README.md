<!doctype html>
<html lang="fr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Prénom Nom — CV</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=Merriweather:wght@300;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="container">
    <aside class="sidebar">
      <div class="photo" aria-hidden="true" style="background-image: url('photo.jpg');"></div>
      <h2 class="name">Prénom Nom</h2>
      <p class="role">Titre / Métier</p>
      <section class="contact">
        <h3>Contact</h3>
        <ul>
          <li>Email: <a href="mailto:prenom.nom@example.com">prenom.nom@example.com</a></li>
          <li>Tél: +33 6 12 34 56 78</li>
          <li>Ville, Pays</li>
          <li><a href="#">portfolio.link</a></li>
        </ul>
      </section>
      <section class="skills">
        <h3>Compétences</h3>
        <div class="skill">
          <span>HTML / CSS</span>
          <div class="bar"><div class="fill" style="width:90%"></div></div>
        </div>
        <div class="skill">
          <span>JavaScript</span>
          <div class="bar"><div class="fill" style="width:75%"></div></div>
        </div>
        <div class="skill">
          <span>Design UI</span>
          <div class="bar"><div class="fill" style="width:80%"></div></div>
        </div>
      </section>
      <section class="languages">
        <h3>Langues</h3>
        <ul>
          <li>Français — natif</li>
          <li>Anglais — courant</li>
        </ul>
      </section>
    </aside>
    <main class="content">
      <header class="intro">
        <p class="summary-title">Résumé</p>
        <p class="summary">Designer / développeuse web créative avec X années d'expérience en création d'interfaces, animation légère et optimisation pour impression. Passionnée par les expériences utilisateur lisibles et élégantes.</p>
      </header>
      <section class="work">
        <h3>Expériences</h3>
        <article class="timeline-item">
          <span class="period">2023 — Aujourd'hui</span>
          <div class="card">
            <h4>Poste — Entreprise</h4>
            <p class="meta">Ville — Contrat</p>
            <ul>
              <li>Responsabilité 1 : description courte.</li>
              <li>Responsabilité 2 : description courte.</li>
            </ul>
          </div>
        </article>
        <article class="timeline-item">
          <span class="period">2020 — 2023</span>
          <div class="card">
            <h4>Poste — Entreprise précédente</h4>
            <p class="meta">Ville — Contrat</p>
            <ul>
              <li>Fait marquant / réalisation.</li>
            </ul>
          </div>
        </article>
      </section>
      <section class="education">
        <h3>Formation</h3>
        <div class="card small">
          <h4>Nom du diplôme — École</h4>
          <p class="meta">Année — Ville</p>
        </div>
      </section>
      <section class="projects">
        <h3>Projets</h3>
        <div class="project-grid">
          <div class="proj">
            <h5>Projet A</h5>
            <p>Une phrase décrivant le projet et votre rôle.</p>
          </div>
          <div class="proj">
            <h5>Projet B</h5>
            <p>Une phrase décrivant le projet et votre rôle.</p>
          </div>
        </div>
      </section>
    </main>
  </div>
</body>
</html>
