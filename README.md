<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¡Feliz Día del Amor y la Amistad! ❤️</title>
    <!-- Importar fuentes de Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;700&family=Open+Sans:wght@300;400;700&display=swap" rel="stylesheet">
    
    <style>
        /* Variables CSS para facilitar el cambio de colores */
        :root {
            --primary-color: #ff6b6b; /* Un rojo vibrante para el amor */
            --secondary-color: #4ecdc4; /* Un turquesa refrescante para la amistad */
            --text-dark: #333;
            --text-light: #f4f4f4;
            --background-light: #ffffff;
            --background-dark: #f0f2f5;
            --card-background: #ffffff;
            --shadow-light: rgba(0, 0, 0, 0.08);
        }

        /* Reset y estilos generales del cuerpo */
        body {
            font-family: 'Open Sans', sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: var(--background-dark);
            color: var(--text-dark);
            line-height: 1.6;
            overflow-x: hidden; /* Evita scroll horizontal */
        }

        /* Estilos de encabezados */
        h1, h2, h3 {
            font-family: 'Dancing Script', cursive;
            color: var(--primary-color);
            text-align: center;
            margin-bottom: 20px;
        }

        h1 {
            font-size: 3.5em; /* Más grande para el título principal */
            color: var(--text-light);
            text-shadow: 2px 2px 5px rgba(0,0,0,0.3);
            letter-spacing: 2px;
        }

        h2 {
            font-size: 2.5em;
            margin-top: 40px;
            position: relative;
        }
        h2::after {
            content: '';
            position: absolute;
            left: 50%;
            bottom: -10px;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background-color: var(--secondary-color);
            border-radius: 5px;
        }

        h3 {
            font-size: 1.8em;
            color: var(--secondary-color);
        }

        /* Estilos del encabezado principal (header) */
        header {
            background: linear-gradient(135deg, var(--primary-color) 0%, #ff9a8d 100%);
            color: var(--text-light);
            padding: 60px 20px;
            text-align: center;
            box-shadow: 0 4px 8px var(--shadow-light);
            position: relative;
            overflow: hidden;
        }
        header::before { /* Elemento decorativo */
            content: '❤️';
            position: absolute;
            top: 10px;
            left: 10%;
            font-size: 3em;
            opacity: 0.2;
            animation: floatHeart 4s infinite ease-in-out;
        }
        header::after { /* Elemento decorativo */
            content: '✨';
            position: absolute;
            bottom: 15px;
            right: 15%;
            font-size: 2.5em;
            opacity: 0.2;
            animation: floatSparkle 5s infinite ease-in-out reverse;
        }

        .subtitle {
            font-family: 'Open Sans', sans-serif;
            font-size: 1.3em;
            margin-top: 10px;
            color: var(--text-light);
        }

        /* Sección Hero (Bienvenida) */
        .hero {
            background-color: var(--background-light);
            padding: 80px 20px;
            text-align: center;
            position: relative;
            overflow: hidden;
            border-bottom: 5px solid var(--secondary-color);
        }
        .hero-content {
            max-width: 800px;
            margin: 0 auto;
            position: relative;
            z-index: 2;
        }
        .hero h2 {
            font-size: 3em;
            color: var(--primary-color);
            margin-bottom: 20px;
        }
        .hero p {
            font-size: 1.2em;
            color: var(--text-dark);
            margin-bottom: 30px;
        }
        
        /* Botón general */
        button, .cta-button {
            background-color: var(--secondary-color);
            color: var(--text-light);
            border: none;
            padding: 15px 30px;
            font-size: 1.1em;
            border-radius: 50px;
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.2s ease;
            text-decoration: none; /* Para el .cta-button */
            display: inline-block; /* Para el .cta-button */
            margin-top: 20px;
            font-family: 'Open Sans', sans-serif;
            font-weight: 700;
            box-shadow: 0 4px 10px rgba(0,0,0,0.2);
        }

        button:hover, .cta-button:hover {
            background-color: #3aa69e; /* Un tono más oscuro */
            transform: translateY(-3px);
            box-shadow: 0 6px 15px rgba(0,0,0,0.25);
        }

        /* Contenedor de mensajes */
        .messages-container {
            padding: 60px 20px;
            background-color: var(--background-dark);
        }

        .message-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            max-width: 1200px;
            margin: 40px auto;
        }

        .message-card {
            background-color: var(--card-background);
            border-radius: 15px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 6px 15px var(--shadow-light);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            position: relative;
            overflow: hidden;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .message-card::before { /* Icono decorativo en la esquina */
            content: '❤️';
            position: absolute;
            top: 15px;
            right: 15px;
            font-size: 1.8em;
            color: var(--primary-color);
            opacity: 0.7;
            transform: rotate(15deg);
        }

        .message-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }

        .message-card h3 {
            margin-top: 0;
            margin-bottom: 15px;
            color: var(--primary-color);
        }

        .message-card p {
            font-size: 1em;
            color: var(--text-dark);
        }

        /* Sección de llamada a la acción */
        .call-to-action {
            background: linear-gradient(45deg, var(--secondary-color) 0%, #76ddda 100%);
            color: var(--text-light);
            padding: 80px 20px;
            text-align: center;
            margin-top: 50px;
            box-shadow: 0 -4px 8px var(--shadow-light);
            position: relative;
            overflow: hidden;
        }
        .call-to-action h2 {
            color: var(--text-light);
            font-size: 3em;
            margin-bottom: 25px;
        }
        .call-to-action h2::after {
            background-color: var(--text-light); /* Línea blanca debajo del h2 */
        }
        .call-to-action p {
            font-size: 1.3em;
            margin-bottom: 40px;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }
        /* Corazones flotantes en CTA */
        .call-to-action::before, .call-to-action::after {
            content: '💖';
            position: absolute;
            font-size: 4em;
            opacity: 0.15;
        }
        .call-to-action::before {
            top: 20%;
            left: 10%;
            animation: floatHeart 6s infinite ease-in-out;
        }
        .call-to-action::after {
            bottom: 15%;
            right: 12%;
            animation: floatHeart 7s infinite ease-in-out reverse;
        }


        /* Pie de página */
        footer {
            background-color: var(--text-dark);
            color: var(--text-light);
            text-align: center;
            padding: 30px 20px;
            font-size: 0.9em;
            border-top: 5px solid var(--primary-color);
        }

        /* Animaciones */
        @keyframes floatHeart {
            0% { transform: translateY(0); }
            50% { transform: translateY(-20px) rotate(5deg); }
            100% { transform: translateY(0); }
        }

        @keyframes floatSparkle {
            0% { transform: translateY(0); }
            50% { transform: translateY(-15px) rotate(-5deg); }
            100% { transform: translateY(0); }
        }

        /* Utilidad para ocultar/mostrar elementos */
        .hidden {
            display: none;
        }

        /* Media Queries para diseño responsivo */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5em;
            }
            h2 {
                font-size: 2em;
            }
            .hero, .call-to-action {
                padding: 60px 15px;
            }
            .subtitle {
                font-size: 1.1em;
            }
            .message-grid {
                grid-template-columns: 1fr; /* Una columna en pantallas pequeñas */
            }
        }

        @media (max-width: 480px) {
            h1 {
                font-size: 2em;
            }
            h2 {
                font-size: 1.8em;
            }
            button, .cta-button {
                padding: 12px 25px;
                font-size: 1em;
            }
            .hero p, .call-to-action p {
                font-size: 1em;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>De Luis, con mucho cariño para mis amistades</h1>
        <p class="subtitle">¡Celebrando el Día del Amor y la Amistad!</p>
    </header>

    <main>
        <section class="hero">
            <div class="hero-content">
                <h2>Un mensaje especial para ustedes</h2>
                <p>En este día tan significativo, quiero tomar un momento para agradecerles por ser parte de mi vida. Su amistad es un tesoro invaluable que aprecio con todo mi corazón. ¡Gracias por cada risa, cada apoyo y cada aventura compartida!</p>
                <button id="discoverBtn">Descubre los mensajes</button>
            </div>
             
        </section>

        <section class="messages-container hidden" id="messagesContainer">
            <h2>Nuestra Amistad, Un Regalo Invaluable</h2>
            <div class="message-grid">
                <div class="message-card">
                    <h3>Presencia que Conforta</h3>
                    <p>Gracias por estar siempre, en los buenos y malos momentos. Su apoyo incondicional es mi mayor fortaleza y un bálsamo para el alma.</p>
                </div>
                <div class="message-card">
                    <h3>Risas que Unen</h3>
                    <p>Cada risa compartida es un recuerdo que atesoro con cariño. Con ustedes, la vida es más ligera, más alegre y llena de momentos inolvidables.</p>
                </div>
                <div class="message-card">
                    <h3>Confianza Eterna</h3>
                    <p>Poder contarles todo, saber que me escuchan sin juzgar y que siempre entenderán, es una bendición que no cambiaría por nada.</p>
                </div>
                <div class="message-card">
                    <h3>Aventuras Inolvidables</h3>
                    <p>Las experiencias y las aventuras vividas a su lado son la sal de mi vida. ¡Que vengan muchas más historias que contar y caminos que recorrer juntos!</p>
                </div>
                <div class="message-card">
                    <h3>Corazones Abiertos</h3>
                    <p>Gracias por la autenticidad, la honestidad y el cariño sincero que me brindan. Valoro profundamente la persona única que es cada uno de ustedes.</p>
                </div>
                <div class="message-card">
                    <h3>Sueños Compartidos</h3>
                    <p>Me inspiran a ser mejor persona cada día, a perseguir mis sueños con pasión y a creer en mí mismo. ¡Sus sueños también son parte de mi alegría!</p>
                </div>
            </div>
             
        </section>

        <section class="call-to-action">
            <h2>¡Gracias por todo!</h2>
            <p>Espero que este pequeño detalle les alegre el día y les recuerde lo mucho que significan para mí. ¡Les envío un abrazo enorme, lleno de gratitud y cariño sincero!</p>
            <a href="#" class="cta-button">¡Celebremos la Amistad Hoy y Siempre!</a>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Luis. Con Amor para mis Amistades. ❤️</p>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const discoverBtn = document.getElementById('discoverBtn');
            const messagesContainer = document.getElementById('messagesContainer');

            // Función para hacer scroll suave
            const smoothScroll = (targetId) => {
                const targetElement = document.getElementById(targetId);
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 20, // Ajusta el offset si tienes un encabezado fijo
                        behavior: 'smooth'
                    });
                }
            };

            discoverBtn.addEventListener('click', () => {
                // Muestra el contenedor de mensajes
                messagesContainer.classList.remove('hidden');

                // Opcional: Desplázate suavemente hacia el contenedor de mensajes
                setTimeout(() => { // Pequeño retraso para asegurar que el elemento esté visible antes de hacer scroll
                    smoothScroll('messagesContainer');
                }, 100);
            });

            // Animación al cargar la página (opcional, para un efecto "wow")
            const cards = document.querySelectorAll('.message-card');
            cards.forEach((card, index) => {
                card.style.opacity = 0;
                card.style.transform = 'translateY(20px)';
                // Usa Intersection Observer para animar cuando la tarjeta entra en la vista
                const observer = new IntersectionObserver((entries) => {
                    entries.forEach(entry => {
                        if (entry.isIntersecting) {
                            setTimeout(() => {
                                entry.target.style.transition = 'opacity 0.6s ease-out, transform 0.6s ease-out';
                                entry.target.style.opacity = 1;
                                entry.target.style.transform = 'translateY(0)';
                            }, index * 150); // Retraso escalonado
                            observer.unobserve(entry.target);
                        }
                    });
                }, { threshold: 0.2 }); // Cuando el 20% de la tarjeta es visible
                observer.observe(card);
            });
        });
    </script>
</body>
</html>
