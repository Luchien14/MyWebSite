<!DOCTYPE html>
<html lang="fr">

<head>
    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>À louer | Maison 4 chambres avec jardin</title>

    <meta name="description"
        content="À louer : maison familiale 4 chambres avec jardin, terrasse, garage et grand grenier semi-aménagé, située dans un clos résidentiel calme.">

    <style>

        :root {
            --ink: #17201d;
            --muted: #68716d;
            --cream: #f4f0e8;
            --paper: #fffdf9;
            --accent: #9b3d2f;
            --accent-dark: #743027;
            --line: #e3ddd2;
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
            font-family:
                Inter,
                ui-sans-serif,
                system-ui,
                -apple-system,
                BlinkMacSystemFont,
                "Segoe UI",
                sans-serif;

            color: var(--ink);
            background: var(--cream);
            line-height: 1.65;
        }


        a {
            color: inherit;
            text-decoration: none;
        }


        img {
            max-width: 100%;
        }


        .wrap {
            width: min(1180px, 92%);
            margin: auto;
        }


        /* =====================================================
           HERO
        ===================================================== */


        .hero {
            min-height: 88vh;

            display: grid;
            grid-template-columns: 1fr 1fr;

            background: var(--paper);
        }


        .hero-copy {
            padding:
                clamp(45px, 7vw, 100px)
                clamp(30px, 7vw, 90px);

            display: flex;
            flex-direction: column;
            justify-content: center;
        }


        /*
           GRAND À LOUER
        */


        .kicker {
            display: inline-block;

            margin-bottom: 24px;

            color: var(--accent);

            font-size:
                clamp(3.2rem, 7vw, 7rem);

            line-height: .85;

            font-weight: 950;

            letter-spacing: .04em;

            text-transform: uppercase;
        }


        h1 {
            font-family: Georgia, serif;

            font-size:
                clamp(3rem, 6vw, 6rem);

            line-height: .95;

            font-weight: 500;

            margin: 0 0 25px;

            letter-spacing: -.045em;
        }


        .hero-subtitle {
            font-size:
                clamp(1.15rem, 2vw, 1.5rem);

            color: var(--muted);

            max-width: 600px;

            margin-bottom: 15px;
        }


        .property-details {
            display: flex;

            flex-wrap: wrap;

            gap: 9px;

            margin: 10px 0 22px;
        }


        .property-details span {
            padding: 8px 15px;

            border:
                1px solid var(--line);

            border-radius: 999px;

            font-size: .9rem;

            font-weight: 750;

            background: var(--cream);
        }


        .address {
            margin-top: 8px;

            font-weight: 700;

            color: var(--ink);
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

            padding: 14px 23px;

            border-radius: 999px;

            font-weight: 800;

            border: 1px solid var(--ink);

            transition:
                transform .2s ease,
                background .2s ease;
        }


        .btn:hover {
            transform: translateY(-2px);
        }


        .btn.primary {
            background: var(--ink);

            color: white;
        }


        .btn.primary:hover {
            background: var(--accent-dark);
        }


        .btn.light {
            background: transparent;
        }


        .hero-photo {
            min-height: 88vh;

            background:

                linear-gradient(
                    90deg,
                    rgba(0,0,0,.02),
                    rgba(0,0,0,.18)
                ),

                url("images/salon-salle-a-manger.jpg")
                center / cover no-repeat;
        }



        /* =====================================================
           SECTIONS
        ===================================================== */


        section {
            padding:
                clamp(65px, 8vw, 110px)
                0;
        }


        .section-head {
            max-width: 780px;

            margin-bottom: 45px;
        }


        .eyebrow {
            color: var(--accent);

            text-transform: uppercase;

            letter-spacing: .15em;

            font-size: .75rem;

            font-weight: 850;
        }


        h2 {
            font-family: Georgia, serif;

            font-size:
                clamp(2.3rem, 4vw, 4rem);

            line-height: 1;

            margin:
                10px 0 18px;

            font-weight: 500;

            letter-spacing: -.03em;
        }


        .lead {
            font-size: 1.08rem;

            color: var(--muted);
        }



        /* =====================================================
           INTRODUCTION
        ===================================================== */


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

            font-size:
                clamp(2rem, 3vw, 2.8rem);

            line-height: 1.1;
        }


        .intro-text {
            font-size: 1.12rem;

            color: var(--muted);
        }



        /* =====================================================
           COMPOSITION
        ===================================================== */


        .composition {
            background: var(--cream);
        }


        .rooms {
            display: grid;

            grid-template-columns:
                repeat(3, 1fr);

            gap: 22px;
        }


        .room-card {
            background: var(--paper);

            padding: 30px;

            border:
                1px solid var(--line);

            box-shadow: var(--shadow);
        }


        .room-number {
            font-size: .75rem;

            color: var(--accent);

            font-weight: 850;

            text-transform: uppercase;

            letter-spacing: .13em;
        }


        .room-card h3 {
            font-family: Georgia, serif;

            font-size: 1.8rem;

            margin:
                8px 0 20px;
        }


        .room-card ul {
            padding: 0;

            margin: 0;

            list-style: none;
        }


        .room-card li {
            padding: 9px 0;

            border-bottom:
                1px solid var(--line);
        }


        .room-card li:last-child {
            border-bottom: 0;
        }



        /* =====================================================
           POINTS FORTS
        ===================================================== */


        .features {
            background: var(--paper);
        }


        .feature-grid {
            display: grid;

            grid-template-columns:
                repeat(4, 1fr);

            gap: 18px;
        }


        .feature {
            padding: 28px;

            border:
                1px solid var(--line);

            background: var(--cream);
        }


        .feature-icon {
            font-size: 1.8rem;

            margin-bottom: 12px;
        }


        .feature strong {
            display: block;

            margin-bottom: 7px;
        }


        .feature span {
            color: var(--muted);

            font-size: .95rem;
        }



        /* =====================================================
           GALERIE
        ===================================================== */


        .gallery-section {
            background: var(--cream);
        }


        .gallery {
            display: grid;

            grid-template-columns:
                1.35fr .65fr;

            gap: 14px;
        }


        .gallery-main {
            height: 560px;

            overflow: hidden;
        }


        .gallery-side {
            display: grid;

            grid-template-rows:
                1fr 1fr;

            gap: 14px;
        }


        .gallery-side div {
            overflow: hidden;
        }


        .gallery img {
            width: 100%;

            height: 100%;

            object-fit: cover;

            display: block;

            transition:
                transform .35s ease;
        }


        .gallery img:hover {
            transform: scale(1.025);
        }


        .gallery-side img {
            height: 273px;
        }



        /* =====================================================
           ENVIRONNEMENT
        ===================================================== */


        .environment {
            background: var(--paper);
        }


        .environment-grid {
            display: grid;

            grid-template-columns:
                1fr 1fr;

            gap: 70px;

            align-items: center;
        }


        .environment-list {
            display: grid;

            gap: 14px;
        }


        .environment-item {
            padding:
                18px 20px;

            border-left:
                3px solid var(--accent);

            background: var(--cream);
        }


        .environment-item strong {
            display: block;
        }



        /* =====================================================
           CONTACT
        ===================================================== */


        .contact {
            background: var(--ink);

            color: white;
        }


        .contact-grid {
            display: grid;

            grid-template-columns:
                1fr .7fr;

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

            border:
                1px solid rgba(255,255,255,.18);

            background:
                rgba(255,255,255,.05);
        }


        .contact-box strong {
            display: block;

            font-size: 1.25rem;

            margin-bottom: 8px;
        }


        .contact .btn {
            border-color: white;

            color: white;

            margin-top: 18px;
        }



        /* =====================================================
           FOOTER
        ===================================================== */


        footer {
            background: #101614;

            color: #aeb7b3;

            padding: 25px 0;

            font-size: .9rem;
        }



        /* =====================================================
           MOBILE
        ===================================================== */


        @media (max-width: 850px) {

            .hero {
                grid-template-columns: 1fr;
            }


            .hero-copy {
                padding:
                    55px 6%;
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
                grid-template-columns:
                    1fr 1fr;
            }


            .gallery {
                grid-template-columns: 1fr;
            }


            .gallery-main {
                height: 420px;
            }


            .gallery-side {
                grid-template-columns:
                    1fr 1fr;

                grid-template-rows:
                    220px;
            }


            .gallery-side img {
                height: 220px;
            }

        }



        @media (max-width: 520px) {

            .kicker {
                font-size: 3rem;
            }


            h1 {
                font-size: 3.2rem;
            }


            .feature-grid {
                grid-template-columns: 1fr;
            }


            .gallery-side {
                grid-template-columns: 1fr;

                grid-template-rows:
                    250px 250px;
            }


            .gallery-side img {
                height: 250px;
            }

        }

    </style>

</head>


<body>


<!-- =====================================================
     HERO
===================================================== -->


<header class="hero">


    <div class="hero-copy">


        <div class="kicker">
            À LOUER
        </div>


        <h1>
            Maison familiale
        </h1>


        <div class="property-details">

            <span>🛏️ 4 chambres</span>

            <span>🌿 Jardin</span>

            <span>☀️ Terrasse</span>

            <span>🚗 Garage</span>

        </div>


        <p class="hero-subtitle">

            Une maison où il fait bon vivre,
            située dans un clos résidentiel calme
            et proche de toutes les commodités.

        </p>


        <div class="address">

            📍 Un environnement paisible,
            proche des principaux axes routiers

        </div>


        <div class="cta">

            <a
                href="#contact"
                class="btn primary"
            >
                📅 Demander une visite
            </a>


            <a
                href="#photos"
                class="btn light"
            >
                Découvrir la maison
            </a>

        </div>


    </div>


    <div class="hero-photo"></div>


</header>



<!-- =====================================================
     INTRODUCTION
===================================================== -->


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

                Vous recherchez une maison confortable,
                fonctionnelle et idéalement située ?

            </p>


            <p>

                Cette agréable habitation vous offre
                un cadre de vie paisible tout en restant
                proche de tout ce dont vous avez besoin
                au quotidien.

            </p>


            <p>

                Écoles, commerces, clubs sportifs
                et principaux axes routiers sont
                facilement accessibles.

            </p>


        </div>


    </div>


</section>



<!-- =====================================================
     COMPOSITION
===================================================== -->


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
                avec de beaux volumes et de nombreux espaces
                pratiques.

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



<!-- =====================================================
     POINTS FORTS
===================================================== -->


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

                <div class="feature-icon">
                    ☀️
                </div>


                <strong>
                    Panneaux photovoltaïques
                </strong>


                <span>

                    Une installation qui contribue
                    à améliorer l'efficacité énergétique
                    de la maison.

                </span>

            </div>



            <div class="feature">

                <div class="feature-icon">
                    🔥
                </div>


                <strong>
                    Nouvelle chaudière
                </strong>


                <span>

                    Nouvelle chaudière
                    à condensation au gaz.

                </span>

            </div>



            <div class="feature">

                <div class="feature-icon">
                    🌿
                </div>


                <strong>
                    Jardin & terrasse
                </strong>


                <span>

                    Un agréable espace extérieur
                    pour profiter des beaux jours.

                </span>

            </div>



            <div class="feature">

                <div class="feature-icon">
                    🚗
                </div>


                <strong>
                    Garage
                </strong>


                <span>

                    Un garage permettant
                    de stationner une voiture à l'abri.

                </span>

            </div>


        </div>


    </div>


</section>



<!-- =====================================================
     GALERIE
===================================================== -->


<section
    class="gallery-section"
    id="photos"
>


    <div class="wrap">


        <div class="section-head">

            <div class="eyebrow">
                Galerie
            </div>


            <h2>
                Découvrez la maison.
            </h2>


            <p class="lead">

                Quelques premières vues des espaces
                de vie. D'autres photos seront ajoutées
                prochainement.

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


                <div>

                    <img
                        src="images/cuisine.jpg"
                        alt="Cuisine ouverte équipée"
                    >

                </div>


                <div>

                    <img
                        src="images/Salon et salle à manger.jpg"
                        alt="Chambre"
                    >

                </div>


            </div>


        </div>


    </div>


</section>



<!-- =====================================================
     ENVIRONNEMENT
===================================================== -->


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

                La maison profite d'un environnement
                résidentiel agréable tout en permettant
                de rejoindre facilement les commodités
                et les principaux axes.

            </p>


        </div>



        <div class="environment-list">


            <div class="environment-item">

                <strong>
                    🏫 Écoles
                </strong>

                À proximité pour faciliter
                le quotidien familial.

            </div>



            <div class="environment-item">

                <strong>
                    🛍️ Commerces
                </strong>

                Les commerces et services
                sont facilement accessibles.

            </div>



            <div class="environment-item">

                <strong>
                    ⚽ Clubs sportifs
                </strong>

                Une offre de loisirs et d'activités
                à proximité.

            </div>



            <div class="environment-item">

                <strong>
                    🛣️ Axes routiers
                </strong>

                Accès pratique aux principaux
                axes de circulation.

            </div>


        </div>


    </div>


</section>



<!-- =====================================================
     CONTACT
===================================================== -->


<section
    class="contact"
    id="contact"
>


    <div class="wrap contact-grid">


        <div>


            <div class="eyebrow">
                Location
            </div>


            <h2>
                Et si cette maison devenait la vôtre ?
            </h2>


            <p>

                Une maison familiale qui combine
                espace, confort, tranquillité
                et praticité.

            </p>


            <p>

                Vous souhaitez obtenir davantage
                d'informations ou organiser une visite ?

            </p>


        </div>



        <div class="contact-box">


            <strong>
                Intéressé(e) ?
            </strong>


            <p>

                Contactez-nous pour recevoir
                les informations complémentaires
                et convenir d'une visite.

            </p>


            <!--
                IMPORTANT :
                Remplacez l'adresse ci-dessous
                par votre véritable adresse e-mail.
            -->


            <a
                href="mailto:mf6306@hotmail.com"
                class="btn"
            >

                ✉️ Nous contacter

            </a>


        </div>


    </div>


</section>



<!-- =====================================================
     FOOTER
===================================================== -->


<footer>


    <div class="wrap">

        Maison 4 chambres à louer
        · Clos résidentiel

    </div>


</footer>


</body>

</html>
