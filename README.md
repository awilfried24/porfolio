<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Portfolio - Armand-Wilfried BAMOUNI</title>
  <style>
    body {
      margin: 0;
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background-color: #f5f5f7;
      color: #222;
    }

    header {
      background: linear-gradient(135deg, #111827, #1f2933);
      color: #fff;
      padding: 32px 16px;
      text-align: center;
    }

    header h1 {
      margin: 0 0 8px;
      font-size: 2rem;
    }

    header p {
      margin: 4px 0;
      font-size: 0.95rem;
      opacity: 0.9;
    }

    .container {
      max-width: 900px;
      margin: 24px auto 40px;
      padding: 0 16px;
    }

    /* Onglets */
    .tabs {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-bottom: 16px;
    }

    .tab-btn {
      flex: 1 1 auto;
      min-width: 100px;
      padding: 10px 14px;
      border-radius: 999px;
      border: 1px solid #d1d5db;
      background-color: #e5e7eb;
      cursor: pointer;
      font-size: 0.95rem;
      text-align: center;
      transition: background-color 0.2s, color 0.2s, border-color 0.2s;
    }

    .tab-btn.active {
      background-color: #111827;
      color: #fff;
      border-color: #111827;
      font-weight: 600;
    }

    /* Contenu */
    .card {
      background-color: #fff;
      border-radius: 16px;
      padding: 20px 18px;
      box-shadow: 0 10px 25px rgba(15, 23, 42, 0.06);
    }

    .tab-content {
      display: none;
      animation: fadeIn 0.2s ease-in-out;
    }

    .tab-content.active {
      display: block;
    }

    h2 {
      margin-top: 0;
      font-size: 1.3rem;
      margin-bottom: 12px;
      color: #111827;
    }

    h3 {
      margin-bottom: 4px;
      margin-top: 14px;
      font-size: 1.05rem;
    }

    .item-meta {
      font-size: 0.85rem;
      color: #6b7280;
      margin-bottom: 4px;
    }

    p {
      margin-top: 0;
      line-height: 1.5;
      font-size: 0.95rem;
      text-align: justify;
      hyphens: auto;
    }

    ul {
      padding-left: 18px;
      margin-top: 4px;
    }

    li {
      margin-bottom: 4px;
      font-size: 0.95rem;
    }

    footer {
      text-align: center;
      font-size: 0.85rem;
      color: #6b7280;
      margin: 24px 0 16px;
    }

    footer a {
      color: #111827;
      text-decoration: none;
      font-weight: 500;
    }

    footer a:hover {
      text-decoration: underline;
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: translateY(4px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @media (max-width: 600px) {
      header h1 {
        font-size: 1.6rem;
      }
      .card {
        padding: 16px 14px;
      }
    }

    .two-columns {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 16px;
    }

    @media (max-width: 700px) {
      .two-columns {
        grid-template-columns: 1fr;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Armand-Wilfried BAMOUNI</h1>
    <p style="text-align:center;font-size:1rem;margin:6px 0;">
      Étudiant en Master 2 Mathématiques Appliquées & Statistique
    </p>

    <p style="text-align:center;font-size:1rem;margin:4px 0;">
      Statisticien, Économiste & Démographe
    </p>

    <p style="text-align:center;font-size:0.9rem;margin:6px 0;line-height:1.4;">
      📧 awilfried.bamouni@gmail.com · 📧 armand-wilfried.bamouni@etu.univ-amu.fr<br />
      📞 +33 7 53 69 75 94 ·
      <a href="https://www.linkedin.com/in/a-w-bamouni/" target="_blank" style="display:inline-flex;align-items:center;gap:6px;text-decoration:none;color:#93c5fd;">
        <img src="https://cdn-icons-png.flaticon.com/512/174/174857.png"
             alt="LinkedIn" width="18" height="18" style="vertical-align:middle;">
        <span>www.linkedin.com/in/a-w-bamouni/</span>
      </a>
    </p>
  </header>

  <main class="container">
    <!-- Onglets -->
    <div class="tabs">
      <button class="tab-btn active" data-tab="apropos">À propos de moi</button>
      <button class="tab-btn" data-tab="parcours">Parcours</button>
      <button class="tab-btn" data-tab="experiences">Expériences</button>
      <button class="tab-btn" data-tab="projets">Projets académiques</button>
    </div>

    <div class="card">
      <!-- 1 : À propos de moi -->
      <section id="apropos" class="tab-content active">
        <p class="justify">
Formé à l’interface de l’économie et de la démographie, et actuellement inscrit en Master 2 Mathématiques appliquées & statistique, j’évolue dans un univers où l’analyse quantitative éclaire des enjeux sociaux complexes. Je m’intéresse particulièrement aux questions de santé publique et de vulnérabilités sociales, tout en accordant une place essentielle au traitement et à l’exploitation de bases de données, issues aussi bien du secteur de l’assurance que d’autres domaines. Mon ambition est de mobiliser ces compétences au service de la décision, aussi bien pour les acteurs publics que pour les entreprises, afin de contribuer à des dispositifs, des services et des politiques réellement fondés sur les données.
        </p>

        <h2>Compétences</h2>

        <div class="two-columns">
          <div>
            <h3>Langues</h3>
            <ul>
              <li>Français : Langue maternelle</li>
              <li>Anglais : Niveau B2</li>
            </ul>

            <h3>Programmation & Langages</h3>
            <ul>
              <li>Python, R, Java, SQL</li>
              <li>XML / XSL, LaTeX</li>
            </ul>

            <h3>Bureautique</h3>
            <ul>
              <li>Excel (macros), Word, PowerPoint</li>
            </ul>
          </div>

          <div>
            <h3>Statistique & Démographie</h3>
            <ul>
              <li>Power BI, SAS, Stata, R, SPSS, MLwiN, NVivo</li>
              <li>Modélisation, estimation, échantillonnage</li>
            </ul>

            <h3>Simulation & SIG</h3>
            <ul>
              <li>SPECTRUM, NetLogo</li>
              <li>ArcGIS, QGIS</li>
            </ul>

            <h3>Collecte & Données</h3>
            <ul>
              <li>KoBoToolbox, CSPro, ODK</li>
              <li>Gestion de bases de données</li>
            </ul>
          </div>
        </div>
      </section>

      <!-- 2 : Parcours -->
      <section id="parcours" class="tab-content">
        <h2>Mon parcours</h2>

        <h3>Master 2 Mathématiques Appliquées, Statistique – MASS POP</h3>
        <p class="item-meta">Aix-Marseille Université · 2025–2026</p>
        <p>
          Spécialisation en analyse de données, statistiques appliquées aux sciences sociales
          et à la démographie. Approfondissement des méthodes quantitatives, de la modélisation
          et des outils de data science.
        </p>

        <h3>Master en Démographie</h3>
        <p class="item-meta">Institut Supérieur des Sciences de la Population, Unuversité Joseph KI-ZERBO/Burkina Faso · 2023–2025</p>
        <p>
          Formation axée sur l’analyse des dynamiques de population, la mortalité, la fécondité
          et l’évaluation des politiques publiques, avec une forte composante statistique.
        </p>

        <h3>Licence en Analyse et Politique Économique</h3>
        <p class="item-meta">Université Norbert ZONGO/Burkina Faso · 2018–2022</p>
        <p>
          Bases solides en microéconomie, macroéconomie et analyse des politiques publiques,
          complétées par des compétences en statistiques appliquées.
        </p>
      </section>

      <!-- 3 : Expériences -->
      <section id="experiences" class="tab-content">
        <h2>Expériences</h2>
        <h3>Assistant de recherche sur les questions d’éthique de la recherche impliquant des sujets humains au Burkina Faso.</h3>
        <p class="item-meta">Burkina Faso · Collaboration avec des équipes de recherche des USA, Népal et du Canada · Juillet - Septembre 2025 </p>
        <ul>
          <li>Participation à l’analyse de protocoles de recherche et à la revue de la littérature.</li>
          <li>Réflexion sur le consentement éclairé, la protection des données et les populations vulnérables.</li>
          <li>Contribution à la rédaction de notes et de rapports scientifiques.</li>
        </ul>

        <h3>Responsable du département statistique & gestionnaire de bases de données</h3>
        <p class="item-meta">Agence de Conseil, de Service et de Formation (ACSF)/Burkina Faso · Juillet - Novembre 2024 </p>
        <ul>
          <li>Pilotage de la collecte, du nettoyage et de l’analyse de données dans le secteur de l’éducation.</li>
          <li>Construction et mise à jour de bases de données fiables pour le suivi des projets.</li>
          <li>Production d’indicateurs et de rapports pour appuyer la prise de décision.</li>
        </ul>

        <h3>Mémoire de Master 2 : Effet de l'espacement des naissances sur la survie des enfants de moins de 5 ans au Burkina Faso - Analyse exploratoire des changements dans le temps (de 1993 à 2021)</h3>
        <p class="item-meta"> Institut Supérieur des Sciences de la Population (ISSP)· Année académique 2023–2025 </p>
        <ul>
          <li>Utilisation de l'analyse de survie.</li>
        </ul>

      </section>

      <!-- 4 : Projets académiques -->
      <section id="projets" class="tab-content">
        <h2>Projets académiques</h2>

        <h3>Atelier de modélisation sur l’intégration des immigrés d’Afrique de l’Ouest et du Nord</h3>
        <p class="item-meta">Aix-Marseille Université · Année académique 2025–2026</p>
        <p>
          Modélisation de l’intégration des immigrés par régression logistique binaire, analyse des facteurs
          socio-économiques associés à la probabilité d’intégration.
        </p>

        <h3>Modélisation et simulation multi-agents du commerce international entre quatre pays</h3>
        <p class="item-meta">Aix-Marseille Université · Année académique 2025–2026</p>
        <p>
          Mise en place d’un modèle multi-agents pour simuler les échanges commerciaux entre quatre pays aux profils
          économiques contrastés, avec exploration de scénarios de politiques commerciales.
        </p>

        <h3>Statut socioéconomique et état nutritionnel des femmes au Burkina Faso</h3>
        <p class="item-meta">Institut Supérieur de Sciences de la Population (ISSP) · Année académique 2024–2025</p>
        <p>
          Modélisation de l’association entre statut socioéconomique et état nutritionnel des femmes à partir
          d’une régression logistique multinomiale, sur données EDS.
        </p>

        <h3>Fécondité précoce des adolescentes et jeunes filles au Burkina Faso</h3>
        <p class="item-meta">Institut Supérieur de Sciences de la Population (ISSP) · Année académique 2024–2025</p>
        <p>
          Analyse des déterminants de la fécondité précoce par régression logistique binaire, identification
          des facteurs socio-démographiques associés.
        </p>

        <h3>Construction d’un score composite d’insécurité alimentaire des ménages (OPO, Burkina Faso)</h3>
        <p class="item-meta">Institut Supérieur de Sciences de la Population (ISSP) · Année académique 2024–2025</p>
        <ul>
          <li>Utilisation d’une échelle de Likert pondérée (9 items) pour construire un score global d’insécurité alimentaire.</li>
          <li>Agrégation des items en indicateur composite, classement des ménages en quartiles d’insécurité.</li>
        </ul>

        <h3>Analyse en composantes principales des indicateurs mondiaux de gouvernance (214 pays, 2016)</h3>
        <p class="item-meta">Institut Supérieur de Sciences de la Population (ISSP) · Année académique 2024–2025</p>
        <ul>
          <li>Matrice de corrélations, indicateurs de type KMO, test de sphéricité de Bartlett.</li>
          <li>Réalisation d’une ACP et projection des pays sur le plan des deux premières composantes.</li>
        </ul>

        <h3>Construction d’un indice de niveau de vie des ménages</h3>
        <p class="item-meta">Institut Supérieur de Sciences de la Population (ISSP) · Année académique 2024–2025</p>
        <ul>
          <li>Construction d’un proxy de niveau de vie par ACP.</li>
          <li>Utilisation des scores factoriels pour créer un indice continu, puis regroupement en quintiles.</li>
        </ul>

        <h3>Typologie des adolescentes et jeunes femmes burkinabè (18–24 ans)</h3>
        <p class="item-meta">Institut Supérieur de Sciences de la Population (ISSP) · Année académique 2024–2025</p>
        <ul>
          <li>Analyse Factorielle des Correspondances Multiples (AFCM/ACM).</li>
          <li>Identification de profils d’adolescentes selon milieu de résidence, niveau de vie, précocité sexuelle, union, contraception, etc.</li>
        </ul>

        <h3>Analyse de données qualitatives sur la restauration des étudiant·e·s</h3>
        <p class="item-meta">Institut Supérieur de Sciences de la Population (ISSP) · Année académique 2024–2025</p>
        <p>
          Analyse de données qualitatives sur la restauration au restaurant central à l’aide d’Excel et NVivo,
          catégorisation thématique et synthèse des perceptions étudiantes.
        </p>

        <h3>Évolution des violences physiques faites aux femmes (Burkina Faso & Côte d’Ivoire)</h3>
        <p class="item-meta">Institut Supérieur de Sciences de la Population (ISSP) · Année académique 2024–2025</p>
        <p>
          Analyse de l’évolution des violences physiques selon le niveau d’instruction entre 2010 et 2021 au Burkina Faso
          et 2011–2021 en Côte d’Ivoire, par méthodes de décomposition.
        </p>

        <h3>Modélisation du risque de naissance par analyse de survie</h3>
        <p class="item-meta">Institut Supérieur de Sciences de la Population (ISSP) · Année académique 2024–2025</p>
        <ul>
          <li>Étude du risque de naissance selon les écarts d’éducation et d’emploi entre conjoints.</li>
          <li>Utilisation de Kaplan-Meier et de modèles de Cox.</li>
        </ul>

        <h3>Analyse et répartition spatiale des infrastructures sanitaires au Burkina Faso</h3>
        <p class="item-meta">Institut Supérieur de Sciences de la Population (ISSP) · Année académique 2023–2024</p>
        <p>
          Analyse spatiale et cartographie de la distribution des infrastructures sanitaires à l’aide de SIG, identification
          des zones sous-dotées.
        </p>

        <h3>Estimation indirecte de la mortalité des enfants et des adultes</h3>
        <p class="item-meta">Institut Supérieur de Sciences de la Population (ISSP) · Année académique 2023–2024</p>
        <p>
          Utilisation de méthodes indirectes (Brass, Orphanhood) pour estimer la mortalité infanto-juvénile et adulte
          en contexte de sous-enregistrement de l’état civil.
        </p>

        <h3>Estimation directe de la mortalité des enfants</h3>
        <p class="item-meta">Institut Supérieur de Sciences de la Population (ISSP) · Année académique 2023–2024</p>
        <p>
          Estimation directe de la mortalité des enfants à partir de données d’enquête avec dates d’événements, construction
          d’indicateurs de mortalité et comparaison aux estimations indirectes.
        </p>

        <h3>Projection démographique de la région du Centre-Ouest du Burkina Faso</h3>
        <p class="item-meta">Institut Supérieur de Sciences de la Population (ISSP) · Année académique 2023–2024</p>
        <p>
          Réalisation de projections démographiques de la région du Centre-Ouest à partir de scénarios de fécondité,
          mortalité et migration.
        </p>

        <h3>Méthodes indirectes d’estimation démographique</h3>
        <p class="item-meta">Institut Supérieur de Sciences de la Population (ISSP) · Année académique 2023–2024</p>
        <p>
          Projet centré sur la mise en œuvre des principales méthodes indirectes d’estimation (Brass, enfants jamais nés,
          Orphanhood), comparaison avec les estimations directes et discussion des hypothèses.
        </p>
      </section>
    </div>
  </main>

  <footer>
    <p style="text-align:center;">
      📧
      <a href="mailto:awilfried.bamouni@gmail.com">awilfried.bamouni@gmail.com</a>
      ·
      <a href="mailto:armand-wilfried.bamouni@etu.univ-amu.fr">armand-wilfried.bamouni@etu.univ-amu.fr</a>
      · 📞 +33 7 53 69 75 94 ·
      <a href="https://www.linkedin.com/in/a-w-bamouni/" target="_blank" style="display:inline-flex;align-items:center;gap:6px;text-decoration:none;color:#111827;">
        <img src="https://cdn-icons-png.flaticon.com/512/174/174857.png"
             alt="LinkedIn" width="20" height="20">
        <span>www.linkedin.com/in/a-w-bamouni/</span>
      </a>
    </p>
  </footer>

  <script>
    // Gestion des onglets
    const buttons = document.querySelectorAll(".tab-btn");
    const contents = document.querySelectorAll(".tab-content");

    buttons.forEach((btn) => {
      btn.addEventListener("click", () => {
        const tabId = btn.getAttribute("data-tab");

        buttons.forEach((b) => b.classList.remove("active"));
        btn.classList.add("active");

        contents.forEach((section) => {
          if (section.id === tabId) {
            section.classList.add("active");
          } else {
            section.classList.remove("active");
          }
        });
      });
    });
  </script>
</body>
</html>
