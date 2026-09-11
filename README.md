<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Maison 4 chambres à louer – Clos résidentiel</title>

    <meta name="description"
          content="À louer : agréable maison familiale 4 chambres avec jardin, terrasse, garage et grenier semi-aménagé. Située dans un clos résidentiel calme à proximité des commodités et des axes principaux.">

    <style>
        :root {
            --ink: #17201d;
            --muted: #68716d;
            --cream: #f6f2ea;
            --paper: #fffdf9;
            --accent: #9b3d2f;
            --accent-dark: #743027;
            --line: #e5dfd4;
            --shadow: 0 18px 55px rgba(20, 25, 22, .10);
        }

        * {
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            margin: 0;
            font-family: Inter, ui-sans-serif, system-ui, -apple-system,
                         BlinkMacSystemFont, "Segoe UI", sans-serif;
            color: var(--ink);
            background: var(--cream);
            line-height: 1.65;
        }

        a {
            color: inherit;
            text-decoration: none;
        }

        .wrap {
            width: min(1180px, 92%);
            margin: auto;
        }

        /* =========================
           HERO
        ========================= */

        .hero {
            min-height: 78vh;
            display: grid;
            grid-template-columns: 1.08fr .92fr;
            background: var(--paper);
        }

        .hero-copy {
            padding: clamp(36px, 7vw, 100px);
            display: flex;
            flex-direction: column;
            justify-content: center;
        }

        .kicker {
            letter-spacing: .16em;
            text-transform: uppercase;
            font-size: .78rem;
            font-weight: 800;
            color: var(--accent);
            margin-bottom: 18px;
        }

        h1 {
            font-family: Georgia, serif;
            font-size: clamp(3rem, 6vw, 6rem);
            line-height: .98;
            font-weight: 500;
            margin: 0 0 26px;
            letter-spacing: -.045em;
        }

        .hero-copy p {
            font-size: 1.12rem;
            max-width: 620px;
            color: var(--muted);
        }

        .address {
            margin-top: 24px;
            font-weight: 700;
        }

        .cta {
            display: flex;
            gap: 12px;
            flex-wrap: wrap;
            margin-top: 28px;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            padding: 13px 20px;
            border-radius: 999px;
            font-weight: 800;
            border: 1px solid var(--ink);
            transition: .2s ease;
        }

        .btn.primary {
            background: var(--ink);
            color: white;
        }

        .btn.light {
            background: transparent;
        }

        .btn:hover {
            transform: translateY(-2px);
        }

        .hero-photo {
            min-height: 78vh;
            background:
                linear-gradient(
                    90deg,
                    rgba(0,0,0,.05),
                    rgba(0,0,0,.20)
                ),
                url("images/salon-salle-a-manger.jpg")
                center / cover no-repeat;
        }

        /* =========================
           SECTIONS
        ========================= */

        section {
            padding: clamp(60px, 8vw, 110px) 0;
        }

        .section-head {
            max-width: 760px;
            margin-bottom: 42px;
        }

        .eyebrow {
            color: var(--accent);
            text-transform: uppercase;
            letter-spacing: .14em;
            font-size: .75rem;
            font-weight: 800;
        }

        h2 {
            font-family: Georgia, serif;
            font-size: clamp(2.3rem, 4vw, 4rem);
            line-height: 1;
            margin: 10px 0 18px;
            font-weight: 500;
        }

        .lead {
            font-size: 1.08rem;
            color: var(--muted);
        }

        /* =========================
           INTRO
        ========================= */

        .intro {
            background: var(--paper);
        }

        .intro-grid {
            display: grid;
            grid-template-columns: .8fr 1.2fr;
            gap: 70px;
            align-items: start;
        }

        .intro-title {
            font-family: Georgia, serif;
            font-size: 2.2rem;
            line-height: 1.1;
        }

        .intro-text {
            font-size: 1.12rem;
            color: var(--muted);
        }

        /* =========================
           COMPOSITION
        ========================= */

        .composition {
            background: var(--cream);
        }

        .rooms {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 22px;
        }

        .room-card {
            background: var(--paper);
            padding: 30px;
            border: 1px solid var(--line);
            box-shadow: var(--shadow);
        }

        .room-number {
            font-size: .78rem;
            color: var(--accent);
            font-weight: 800;
            text-transform: uppercase;
            letter-spacing: .12em;
        }

        .room-card h3 {
            font-family: Georgia, serif;
            font-size: 1.8rem;
            margin: 8px 0 20px;
        }

        .room-card ul {
            padding: 0;
            margin: 0;
            list-style: none;
        }

        .room-card li {
            padding: 8px 0;
            border-bottom: 1px solid var(--line);
        }

        .room-card li:last-child {
            border-bottom: 0;
        }

        /* =========================
           POINTS FORTS
        ========================= */

        .features {
            background: var(--paper);
        }

        .feature-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 18px;
        }

        .feature {
            padding: 28px;
            border: 1px solid var(--line);
            background: var(--cream);
        }

        .feature-icon {
            font-size: 1.7rem;
            margin-bottom: 12px;
        }

        .feature strong {
            display: block;
            margin-bottom: 5px;
        }

        .feature span {
            color: var(--muted);
            font-size: .95rem;
        }

        /* =========================
           GALERIE
        ========================= */

        .gallery-section {
            background: var(--cream);
        }

        .gallery {
            display: grid;
            grid-template-columns: 1.35fr .65fr;
            gap: 14px;
        }

        .gallery-main,
        .gallery-side img {
            overflow: hidden;
        }

        .gallery img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
            transition: transform .35s ease;
        }

        .gallery-main {
            height: 560px;
        }

        .gallery-side {
            display: grid;
            grid-template-rows: 1fr 1fr;
            gap: 14px;
        }

        .gallery-side img {
            height: 273px;
        }

        .gallery img:hover {
            transform: scale(1.025);
        }

        /* =========================
           ENVIRONNEMENT
        ========================= */

        .environment {
            background: var(--paper);
        }

        .environment-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 70px;
            align-items: center;
        }

        .environment-list {
            display: grid;
            gap: 14px;
        }

        .environment-item {
            padding: 18px 20px;
            border-left: 3px solid var(--accent);
            background: var(--cream);
        }

        .environment-item strong {
            display: block;
        }

        /* =========================
           CONTACT
        ========================= */

        .contact {
            background: var(--ink);
            color: white;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: 1fr .7fr;
            gap: 60px;
            align-items: center;
        }

        .contact h2 {
            color: white;
        }

        .contact p {
            color: #d6dcda;
            max-width: 650px;
        }

        .contact-box {
            padding: 32px;
            border: 1px solid rgba(255,255,255,.18);
            background: rgba(255,255,255,.05);
        }

        .contact-box strong {
            display: block;
            font-size: 1.2rem;
            margin-bottom: 8px;
        }

        .contact .btn {
            border-color: white;
            color: white;
            margin-top: 18px;
        }

        /* =========================
           FOOTER
        ========================= */

        footer {
            background: #101614;
            color: #aeb7b3;
            padding: 25px 0;
            font-size: .9rem;
        }

        /* =========================
           MOBILE
        ========================= */

        @media (max-width: 850px) {

            .hero {
                grid-template-columns: 1fr;
            }

            .hero-copy {
                padding: 55px 6%;
            }

            .hero-photo {
                min-height: 55vh;
            }

            .intro-grid,
            .environment-grid,
            .contact-grid {
                grid-template-columns: 1fr;
                gap: 35px;
            }

            .rooms {
                grid-template-columns: 1fr;
            }

            .feature-grid {
                grid-template-columns: 1fr 1fr;
            }

            .gallery {
                grid-template-columns: 1fr;
            }

            .gallery-main {
                height: 420px;
            }

            .gallery-side {
                grid-template-columns: 1fr 1fr;
                grid-template-rows: 220px;
            }

            .gallery-side img {
                height: 220px;
            }
        }

        @media (max-width: 520px) {

            h1 {
                font-size: 3.1rem;
            }

            .feature-grid {
                grid-template-columns: 1fr;
            }

            .gallery-side {
                grid-template-columns: 1fr;
                grid-template-rows: 250px 250px;
            }

            .gallery-side img {
                height: 250px;
            }
        }
    </style>
</head>

<body>

<!-- =========================
     HERO
========================= -->

<header class="hero">

    <div class="hero-copy">

        <div class="kicker">
            À louer · Maison familiale
        </div>

        <h1>
            Une maison où il fait bon vivre.
        </h1>

        <p>
            Maison 4 chambres avec jardin, terrasse, garage et grand
            grenier semi-aménagé, située dans un clos résidentiel calme.
        </p>

        <div class="address">
            📍 Un environnement paisible, proche de toutes les commodités
        </div>

        <div class="cta">
            <a href="#contact" class="btn primary">
                Demander une visite
            </a>

            <a href="#photos" class="btn light">
                Découvrir la maison
            </a>
        </div>

    </div>

    <div class="hero-photo"></div>

</header>


<!-- =========================
     INTRODUCTION
========================= -->

<section class="intro">

    <div class="wrap intro-grid">

        <div>
            <div class="eyebrow">
                Le cadre de vie
            </div>

            <div class="intro-title">
                Le calme d'un clos résidentiel,
                le confort d'une vraie maison familiale.
            </div>
        </div>

        <div class="intro-text">

            <p>
                Vous recherchez une maison confortable, fonctionnelle
                et idéalement située ?
            </p>

            <p>
                Cette agréable habitation vous offre un cadre de vie
                paisible tout en restant proche de tout ce dont vous
                avez besoin au quotidien.
            </p>

            <p>
                Écoles, commerces, clubs sportifs et principaux axes
                routiers sont facilement accessibles.
            </p>

        </div>

    </div>

</section>


<!-- =========================
     COMPOSITION
========================= -->

<section class="composition">

    <div class="wrap">

        <div class="section-head">

            <div class="eyebrow">
                La maison
            </div>

            <h2>
                Des espaces pensés pour toute la famille.
            </h2>

            <p class="lead">
                Une organisation agréable sur trois niveaux,
                avec de beaux volumes et de nombreux espaces pratiques.
            </p>

        </div>


        <div class="rooms">

            <!-- REZ-DE-CHAUSSEE -->

            <div class="room-card">

                <div class="room-number">
                    Rez-de-chaussée
                </div>

                <h3>
                    Vie quotidienne
                </h3>

                <ul>
                    <li>Hall d'entrée</li>
                    <li>WC séparé</li>
                    <li>Séjour avec vue sur le jardin</li>
                    <li>Cuisine ouverte équipée</li>
                    <li>Buanderie</li>
                    <li>Garage 1 voiture</li>
                    <li>Terrasse & jardin</li>
                </ul>

            </div>


            <!-- PREMIER ETAGE -->

            <div class="room-card">

                <div class="room-number">
                    1er étage
                </div>

                <h3>
                    Espace nuit
                </h3>

                <ul>
                    <li>4 grandes chambres</li>
                    <li>1 salle de bain</li>
                    <li>Espaces généreux</li>
                    <li>Ambiance calme</li>
                </ul>

            </div>


            <!-- DEUXIEME ETAGE -->

            <div class="room-card">

                <div class="room-number">
                    2e étage
                </div>

                <h3>
                    Grenier
                </h3>

                <ul>
                    <li>Grand grenier semi-aménagé</li>
                    <li>Espace de rangement</li>
                    <li>Possibilité de bureau</li>
                    <li>Idéal comme salle de jeux</li>
                    <li>Espace à aménager selon vos besoins</li>
                </ul>

            </div>

        </div>

    </div>

</section>


<!-- =========================
     POINTS FORTS
========================= -->

<section class="features">

    <div class="wrap">

        <div class="section-head">

            <div class="eyebrow">
                Les + de la maison
            </div>

            <h2>
                Le confort au quotidien.
            </h2>

        </div>


        <div class="feature-grid">

            <div class="feature">

                <div class="feature-icon">☀️</div>

                <strong>
                    Panneaux photovoltaïques
                </strong>

                <span>
                    Une installation pensée pour améliorer
                    l'efficacité énergétique de la maison.
                </span>

            </div>


            <div class="feature">

                <div class="feature-icon">🔥</div>

                <strong>
                    Nouvelle chaudière
                </strong>

                <span>
                    Nouvelle chaudière à condensation au gaz.
                </span>

            </div>


            <div class="feature">

                <div class="feature-icon">🌿</div>

                <strong>
                    Jardin & terrasse
                </strong>

                <span>
                    Un agréable espace extérieur pour profiter
                    des beaux jours.
                </span>

            </div>


            <div class="feature">

                <div class="feature-icon">🚗</div>

                <strong>
                    Garage
                </strong>

                <span>
                    Un garage permettant de stationner
                    une voiture à l'abri.
                </span>

            </div>

        </div>

    </div>

</section>


<!-- =========================
     GALERIE
========================= -->

<section class="gallery-section" id="photos">

    <div class="wrap">

        <div class="section-head">

            <div class="eyebrow">
                Galerie
            </div>

            <h2>
                Quelques vues de la maison.
            </h2>

            <p class="lead">
                Découvrez les espaces de vie et l'atmosphère
                chaleureuse de cette habitation.
            </p>

        </div>


        <div class="gallery">

            <div class="gallery-main">

                <img
                    src="images/salon-salle-a-manger.jpg"
                    alt="Salon et salle à manger"
                >

            </div>


            <div class="gallery-side">

                <img
                    src="images/cuisine.jpg"
                    alt="Cuisine ouverte équipée"
                >

                <img
                    src="images/Salon et salle à manger.jpg"
                    alt="Espace salon et salle à manger"
                >

            </div>

        </div>

    </div>

</section>


<!-- =========================
     ENVIRONNEMENT
========================= -->

<section class="environment">

    <div class="wrap environment-grid">

        <div>

            <div class="eyebrow">
                Emplacement
            </div>

            <h2>
                Au calme, sans être isolé.
            </h2>

            <p class="lead">
                La maison profite d'un environnement résidentiel
                agréable tout en permettant de rejoindre facilement
                les commodités et les principaux axes.
            </p>

        </div>


        <div class="environment-list">

            <div class="environment-item">
                <strong>🏫 Écoles</strong>
                À proximité pour faciliter le quotidien familial.
            </div>

            <div class="environment-item">
                <strong>🛍️ Commerces</strong>
                Les commerces et services sont facilement accessibles.
            </div>

            <div class="environment-item">
                <strong>⚽ Clubs sportifs</strong>
                Une offre de loisirs et d'activités à proximité.
            </div>

            <div class="environment-item">
                <strong>🛣️ Axes routiers</strong>
                Accès pratique aux principaux axes de circulation.
            </div>

        </div>

    </div>

</section>


<!-- =========================
     CONTACT
========================= -->

<section class="contact" id="contact">

    <div class="wrap contact-grid">

        <div>

            <div class="eyebrow">
                Location
            </div>

            <h2>
                Et si cette maison devenait la vôtre ?
            </h2>

            <p>
                Une maison familiale qui combine espace, confort,
                tranquillité et praticité.
            </p>

            <p>
                Vous souhaitez obtenir davantage d'informations
                ou organiser une visite ?
            </p>

        </div>


        <div class="contact-box">

            <strong>
                Intéressé(e) ?
            </strong>

            <p>
                Contactez-nous pour recevoir les informations
                complémentaires et convenir d'une visite.
            </p>

            <!-- REMPLACER LE LIEN PAR VOTRE EMAIL -->
            <a
                href="mailto:mf6303@hotmail.com"
                class="btn"
            >
                ✉️ Nous contacter
            </a>

        </div>

    </div>

</section>


<!-- =========================
     FOOTER
========================= -->

<footer>

    <div class="wrap">

        Maison 4 chambres à louer · Clos résidentiel

    </div>

</footer>

</body>
</html>
