# portfolio

<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">                                                         
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <link rel="stylesheet" href="https://unpkg.com/aos@next/dist/aos.css" />
    <link rel="stylesheet" href="style.css">
    <title>Mouhammad Portfolio</title>
</head>
<body>
    <!-- Barre de navigation -->
    <nav>
        <div class="nav-container">
            <div class="logo" data-aos="zoom-in" data-aos-duration="1500">
                Koné <span>Mouhammad</span>
            </div>
            <ul class="nav-links">
                <li><a href="#home">Accueil</a></li>
                <li><a href="#about">À propos de Moi</a></li>
                <li><a href="#skills">Compétences</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="hamburg" onclick="toggleNav()">
                <i class="fas fa-bars"></i>
            </div>
        </div>
    </nav>

    <!-- Section Accueil -->
    <section id="home">
        <div class="main-container">
            <div class="image" data-aos="zoom-out" data-aos-duration="3000">
                <img src="main.jpg" alt="">
            </div>
            <div class="content">
                <h1 data-aos="fade-left" data-aos-duration="1500" data-aos-delay="700">
                    Salut, Moi c'est <span>Mouhammad</span>
                </h1>
                <div class="typewriter" data-aos="fade-right" data-aos-duration="1500" data-aos-delay="900">
                    <span class="typewriter-text">Je suis Étudiant, futur Bio-Informaticien</span>
                    <label for="">|</label>
                </div>
                <div class="social-links" data-aos="flip-down" data-aos-duration="1000" data-aos-delay="1200">
                    <a href="https://www.linkedin.com/in/mouhammad-abder-rachid-kon%C3%A9-323041347?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
                    <a href="https://www.facebook.com/share/19u2UrEm5G/" target="_blank"><i class="fa-brands fa-facebook"></i></a>
                    <a href="https://wa.me/+2250757587201" target="_blank"><i class="fa-brands fa-whatsapp"></i></a>
                    <a href="https://x.com/Momo2006Kone?t=JxQGyIpYnQi7bhmpjCJa0A&s=08" target="_blank"><i class="fa-brands fa-x-twitter"></i></a>
                    <a href="https://github.com/Mouhammad-Kone" target="_blank"><i class="fa-brands fa-github"></i></a>
                    <a href="https://www.instagram.com/mouhammadabderrachidkone?igsh=MjFmam54NmU4MjJi" target="_blank"><i class="fa-brands fa-instagram"></i></a>
                </div>
                <div class="btn" data-aos="zoom-out-left" data-aos-duration="1000" data-aos-delay="1300">
                    <a href="CV_Mouhammad.pdf" download="CV_Mouhammad.pdf">
                        <button>Télécharger mon CV</button>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Section À propos -->
    <section id="about">
        <div class="main-container">
            <div class="image" data-aos="zoom-out" data-aos-duration="3000">
                <img src="main2.jpg" alt="">
            </div>
            <div class="about-text">
                <h2>À propos de Moi</h2>
                <p>Née le 26 janvier 2006, j'ai fait mon parcours primaire au groupe scolaire LIBREVILLE de 2011 à 2017 dans la ville de Man, à l'ouest de la Côte d'Ivoire. De 2017 à 2021, je fait mon premier cycle au Collège Catholique Saint Martyrs de l'Ouganda couronné par l'obtention de mon BEPC. À partir de 2021, j'entame le cycle secondaire au Lycée Moderne II de Man et en 2024 j'obtiens mon Baccalauréat D. À la suite de cela, je suis admis en Classe Préparatoire au Cycle Ingénieur en BCPST(Biologie, Chimie, Physique, Science de la Terre) à l'Université Internationale de Cocody.</p>
            </div>
        </div>
    </section>

    <!-- Section Compétences -->
    <section id="skills">
        <h2 class="heading"><span>Compétences</span></h2>
        <div class="skills-container">
            <div class="skills-box">
                <i class="fa-solid fa-code"></i>
                <h3>Développement Web</h3>
                <p>Création de sites modernes et responsifs.</p>
            </div>
            <div class="skills-box">
                <i class="fa-solid fa-database"></i>
                <h3>Base de Données</h3>
                <p>Gestion et optimisation des bases de données.</p>
            </div>
            <div class="skills-box">
                <i class="fa-solid fa-laptop"></i>
                <h3>Bio-Informatique</h3>
                <p>Analyse de données biologiques avec outils informatiques.</p>
            </div>
        </div>
    </section>

    <!-- Section Contact -->
    <section id="contact">
        <div class="main-container">
            <h2>Contact</h2>
            <form id="contactForm" action="traitement.php" method="POST">
                <label for="nom">Nom :</label>
                <input type="text" id="nom" name="nom" required>

                <label for="email">Email :</label>
                <input type="email" id="email" name="email" required>

                <label for="message">Message :</label>
                <textarea id="message" name="message" required></textarea>

                <button type="submit">Envoyer</button>
            </form>
        </div>
    </section>

    <script src="https://unpkg.com/aos@next/dist/aos.js"></script>
    <script>
        AOS.init();
        function toggleNav() {
            const navLinks = document.querySelector('.nav-links');
            navLinks.classList.toggle('active');
        }
    </script>
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <script src="script.js"></script>
</body>
</html>



@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600&display=swap');

* {
    padding: 0;
    margin: 0;
    font-family: 'Poppins', sans-serif;
    box-sizing: border-box;
}

body {
    background-color: black;
    color: white;
}

/* Barre de navigation améliorée */
nav {
    width: 100%;
    height: 10vh;
    position: sticky;
    top: 0;
    background-color: black;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 20px;
}

.nav-container{
    display: flex;
}
.nav-links {
    list-style: none;
    display: flex;
    transition: max-height 0.3s ease-in-out;
}

.nav-links.active {
    display: block;
}

.nav-links li {
    margin: 0 15px;
}

.nav-links a {
    text-decoration: none;
    color: #077b32;
    font-size: 1.5rem;
    font-weight: bold;
    transition: 0.3s;
}

.nav-links a:hover {
    color: #f2fdf6;
}

.hamburg {
    cursor: pointer;
    color: white;
    font-size: 2rem;
    display: none;
}

.logo {
    color: white;
    font-size: 2rem;
    font-weight: bold;
}

.logo span {
    color: #077b32;
    text-shadow: 0 0 10px #077b32;
}

/* Responsive */
@media (max-width: 768px) {
    .nav-links {
        display: none;
        flex-direction: column;
        position: absolute;
        top: 10vh;
        left: 0;
        background: black;
        width: 100%;
    }

    .hamburg {
        display: block;
    }

    #home .main-container, #about .main-container {
        flex-direction: column;
        align-items: center;
    }
}

/* Section Accueil */
#home .main-container {
    display: flex;
    align-items: center; /* Center vertically */
    justify-content: space-between;
    padding: 50px;
}

#home .image img {
    width: 250px;
    height: auto;
    border-radius: 15px;
}

#home .content {
    display: flex;
    flex-direction: column;
    align-items: flex-start; /* Align text to the left */
    text-align: right;
    padding-left: 20px; /* Reduce padding to bring text closer to the image */
}

#home .content .typewriter {
    flex: 1;
    font-weight: 600;
}

#home .typewriter {
    font-size: clamp(1rem, 1rem + 5vw, 2.5rem);
    font-weight: bold;
}

#home .typewriter-text {
    font-size: calc(1rem + 2%); /* Increase font size by 2% */
    font-weight: bold;
}

/* Section À propos */
#about .main-container {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 50px;
}

#about .image {
    flex: 1;
}

#about .image img {
    width: 100%;
    height: auto;
    border-radius: 15px;
}

#about .about-text {
    flex: 2;
    padding-left: 30px; /* Add padding to the right */
    text-align: left;
}

/* Bouton Télécharger CV */
.btn button {
    background-color: #077b32;
    color: white;
    padding: 10px 15px;
    border: none;
    cursor: pointer;
    border-radius: 5px;
    transition: 0.3s;
}

.btn button:hover {
    background: transparent;
    border: 2px solid #077b32;
    color: #077b32;
}

/* Réseaux sociaux */
.social-links {
    margin: 20px 0;
}

.social-links i {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 3rem;
    height: 3rem;
    background-color: transparent;
    border: 0.2rem solid #077b32;
    border-radius: 50%;
    color: #077b32;
    margin: 5px 15px;
    font-size: 1.5rem;
    transition: 0.2s linear;
}

.social-links a:hover i {
    color: white;
    transform: scale(1.2);
    box-shadow: 0 0 10px #077b32;
}

/* Compétences */
.skills-container {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}

@keyframes slideInUp {
    from {
        transform: translateY(100%);
        opacity: 0;
    }
    to {
        transform: translateY(0);
        opacity: 1;
    }
}

.skills-box {
    background: #222;
    padding: 20px;
    border-radius: 10px;
    text-align: center;
    width: 300px;
    transition: 0.3s;
    animation: slideInUp 0.5s ease-out;
}

.skills-box:hover {
    transform: translateY(-5px);
    box-shadow: 0 0 15px #077b32;
}

/* Formulaire Contact */
form {
    background: #222;
    padding: 20px;
    border-radius: 10px;
    width: 100%;
    max-width: 500px;
}

form label {
    display: block;
    margin-bottom: 5px;
}

form input, form textarea {
    width: 100%;
    padding: 10px;
    margin-bottom: 15px;
    border-radius: 5px;
    border: none;
    outline: none;
}

form button {
    background-color: #077b32;
    color: white;
    padding: 10px 15px;
    border: none;
    cursor: pointer;
    border-radius: 5px;
    width: 100%;
}

form button:hover {
    background: transparent;
    border: 2px solid #077b32;
    color: #077b32;
}

button {
    transition: transform 0.3s ease;
}

button:hover {
    transform: scale(1.1);
}
