<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Terapeuta de lenguaje</title>
    <style>
        body {
            font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
            background-color: #e3f2fd;
            color: #333;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #1e88e5;
            color: white;
            padding: 1em 0;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        nav {
            background-color: #1565c0;
            color: white;
            padding: 1em;
            text-align: center;
        }
        nav a {
            color: white;
            margin: 0 1em;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s;
        }
        nav a:hover {
            color: #90caf9;
        }
        .hero {
            background: linear-gradient(to bottom right, #1e88e5, #42a5f5);
            color: white;
            padding: 5em 0;
            text-align: center;
            position: relative;
            overflow: hidden;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }
        .hero h1 {
            font-size: 4em;
            margin: 0;
            animation: fadeInDown 2s ease-in-out;
        }
        .hero p {
            font-size: 1.5em;
            margin-top: 0.5em;
            animation: fadeInUp 2s ease-in-out;
        }
        .container {
            padding: 2em;
            max-width: 1200px;
            margin: 0 auto;
        }
        .service, .contact-section, .reference, .about, .inicio {
            background-color: #bbdefb;
            border: 2px solid #90caf9;
            border-radius: 12px;
            margin: 1em 0;
            padding: 1.5em;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .service img, .contact-section img, .reference img, .about img, .inicio img {
            max-width: 100px;
            margin-bottom: 1em;
            border-radius: 8px;
        }
        .service img {
            max-width: 200px;
        }
        .service:hover, .contact-section:hover, .reference:hover, .about:hover, .inicio:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 12px rgba(0, 0, 0, 0.2);
        }
        footer {
            background-color: #1e88e5;
            color: white;
            padding: 1em 0;
            text-align: center;
        }
        .contact-info {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-top: 2em;
            background-color: #bbdefb;
            padding: 2em;
            border-radius: 12px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .contact-info div {
            margin-bottom: 1em;
            text-align: center;
        }
        .section {
            display: none;
        }
        .section.active {
            display: block;
        }
        @keyframes fadeInDown {
            from {
                opacity: 0;
                transform: translateY(-50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        @media (min-width: 600px) {
            .service, .contact-section, .reference, .about, .inicio {
                flex-direction: row;
                text-align: left;
            }
            .service img, .contact-section img, .reference img, .about img, .inicio img {
                margin-bottom: 0;
                margin-right: 1.5em;
            }
            .contact-info {
                flex-direction: row;
                justify-content: space-around;
            }
        }
        @media (max-width: 600px) {
            .hero h1 {
                font-size: 2em;
            }
            .hero p {
                font-size: 1em;
            }
            nav a {
                display: block;
                margin: 0.5em 0;
            }
            .service, .contact-section, .reference, .about, .inicio {
                text-align: center;
            }
        }
    </style>
    <script>
        function showSection(sectionId) {
            document.querySelectorAll('.section').forEach(section => {
                section.classList.remove('active');
            });
            document.getElementById(sectionId).classList.add('active');
        }
    </script>
</head>
<body>
    <header>
        <h1>Terapeuta de lenguaje</h1>
    </header>
    <nav>
        <a href="#inicio" onclick="showSection('inicio')">Inicio</a>
        <a href="#about" onclick="showSection('about')">Sobre mí</a>
        <a href="#services" onclick="showSection('services')">Servicios</a>
        <a href="#references" onclick="showSection('references')">Referencias</a>
        <a href="#contact" onclick="showSection('contact')">Contacto</a>
    </nav>
    <div class="hero">
        <h1>Bienvenido a Terapeuta de lenguaje</h1>
        <p>Mejorando la comunicación, un paso a la vez</p>
    </div>
    <div class="container section active inicio" id="inicio">
        <h2>Inicio</h2>
        <p>Bienvenido a mi página web. Soy un terapeuta de lenguaje especializado en ayudar a personas a mejorar sus habilidades de comunicación. Con años de experiencia y certificaciones en el campo, estoy aquí para ofrecerte los mejores servicios a domicilio.</p>
        <p>La terapia de lenguaje es una disciplina dedicada a la evaluación y tratamiento de problemas de comunicación y trastornos del lenguaje. Los terapeutas de lenguaje trabajan con personas de todas las edades, desde niños pequeños hasta adultos mayores, que tienen dificultades con la comunicación. Estos problemas pueden incluir trastornos del habla, del lenguaje, de la voz y de la fluidez, como la tartamudez.</p>
    </div>
    <div class="container section" id="about">
        <!-- Apartado Sobre mí vacío -->
    </div>
    <div class="container section" id="services">
        <h2>Servicios</h2>
        <div class="service">
            <img src="https://media.istockphoto.com/id/1446236920/es/foto/profesor-y-ni%C3%B1a-en-clase-de-logopedia.jpg?s=612x612&w=0&k=20&c=Qa7DK5zAowhQd91mOd3WVZ06jAklDC2jA8Mey9_hvVc=" alt="Servicios a domicilio">
            <div>
                <h3>Servicios a domicilio</h3>
                <p>Ofrecemos terapia de lenguaje directamente en la comodidad de tu hogar. Nuestro servicio a domicilio está diseñado para proporcionar una atención personalizada y cómoda para nuestros pacientes, garantizando un entorno familiar y seguro.</p>
                <p>Realizamos sesiones de evaluación y tratamiento en el hogar del paciente, adaptándonos a sus horarios y necesidades. Este enfoque facilita la colaboración con la familia y permite un seguimiento más cercano del progreso del paciente en su entorno diario.</p>
            </div>
        </div>
        <div class="service">
            <img src="https://via.placeholder.com/150" alt="Terapia de lenguaje">
            <div>
                <h3>Terapia de lenguaje</h3>
                <p>Tratamientos personalizados para mejorar las habilidades de comunicación. Trabajamos con personas de todas las edades, utilizando técnicas y herramientas avanzadas para abordar diversos problemas del lenguaje y la comunicación.</p>
                <p>Nuestros programas incluyen actividades interactivas y ejercicios específicos diseñados para mejorar el vocabulario, la gramática, la comprensión y la expresión verbal. Nos enfocamos en desarrollar estrategias que los pacientes puedan utilizar en su vida diaria para mejorar su comunicación.</p>
            </div>
        </div>
        <div class="service">
            <img src="https://via.placeholder.com/150" alt="Tratamiento para tartamudez">
            <div>
                <h3>Tratamiento para tartamudez</h3>
                <p>Ayudamos a reducir la tartamudez y mejorar la fluidez del habla. Nuestros programas están diseñados para aumentar la confianza y la capacidad de hablar con facilidad en diversas situaciones sociales y profesionales.</p>
                <p>Utilizamos técnicas de control de la respiración, ejercicios de relajación y estrategias de comunicación efectiva para ayudar a los pacientes a manejar su tartamudez. También trabajamos en el desarrollo de habilidades sociales y de afrontamiento para aumentar la autoconfianza del paciente.</p>
            </div>
        </div>
        <div class="service">
            <img src="https://via.placeholder.com/150" alt="Trastorno fonológico">
            <div>
                <h3>Trastorno fonológico</h3>
                <p>Tratamientos para corregir errores en la producción de sonidos del habla. Evaluamos y diseñamos planes de tratamiento específicos para ayudar a nuestros pacientes a superar las dificultades fonológicas y mejorar su pronunciación.</p>
                <p>Nuestros terapeutas utilizan juegos, actividades lúdicas y ejercicios repetitivos para enseñar a los niños a producir los sonidos correctamente. También trabajamos con los padres para que puedan apoyar el desarrollo del habla de sus hijos en casa.</p>
            </div>
        </div>
        <div class="service">
            <img src="https://via.placeholder.com/150" alt="Estimulación de lenguaje">
            <div>
                <h3>Estimulación de lenguaje</h3>
                <p>Ejercicios y actividades para fomentar el desarrollo del lenguaje en niños. Utilizamos métodos lúdicos y efectivos para estimular el lenguaje en niños, ayudándoles a alcanzar hitos importantes en su desarrollo comunicativo.</p>
                <p>Proporcionamos un entorno rico en lenguaje, utilizando juegos, canciones y lecturas interactivas para estimular el desarrollo del lenguaje en niños pequeños. Nuestro objetivo es hacer que el aprendizaje del lenguaje sea una experiencia divertida y atractiva para los niños.</p>
            </div>
        </div>
    </div>
    <div class="container section" id="references">
        <h2>Referencias</h2>
        <div class="reference">
            <img src="https://via.placeholder.com/100" alt="Referencia 1">
            <div>
                <h3>María Gómez</h3>
                <p>"La terapia de lenguaje con este profesional ha sido una experiencia maravillosa para mi hijo. Hemos visto un progreso significativo en su habla y confianza."</p>
            </div>
        </div>
        <div class="reference">
            <img src="https://via.placeholder.com/100" alt="Referencia 2">
            <div>
                <h3>Carlos Rodríguez</h3>
                <p>"Recomiendo altamente estos servicios. El terapeuta es muy paciente y conocedor, y ha ayudado mucho a mi padre con su tartamudez."</p>
            </div>
        </div>
        <div class="reference">
            <img src="https://via.placeholder.com/100" alt="Referencia 3">
            <div>
                <h3>Ana Martínez</h3>
                <p>"El enfoque personalizado y la atención a detalle han hecho una gran diferencia en el desarrollo del lenguaje de mi hija. Estamos muy agradecidos."</p>
            </div>
        </div>
    </div>
    <div class="container section" id="contact">
        <h2>Contacto</h2>
        <p>Si tienes alguna pregunta o deseas agendar una cita, por favor no dudes en contactarme.</p>
        <div class="contact-section">
            <img src="https://via.placeholder.com/150" alt="Contacto">
            <div>
                <h3>Email</h3>
                <p>info@terapeutadelenguaje.com</p>
            </div>
        </div>
        <div class="contact-section">
            <img src="https://via.placeholder.com/150" alt="Contacto">
            <div>
                <h3>Teléfono</h3>
                <p>+1 234 567 890</p>
            </div>
        </div>
    </div>
    <footer>
        <p>&copy; 2024 Terapeuta de lenguaje. Todos los derechos reservados.</p>
    </footer>
</body>
</html>
