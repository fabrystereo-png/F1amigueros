<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amigueros F1 | Torneo Amateur</title>
    <script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXX"></script>
    <script>
      window.dataLayer = window.dataLayer || [];
      function gtag(){dataLayer.push(arguments);}
      gtag('js', new Date());
      gtag('config', 'G-XXXXX');
    </script>
    
    <style>
        :root {
            --f1-red: #e10600;
            --dark-bg: #15151e;
            --card-bg: #1f1f27;
            --white: #ffffff;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--dark-bg);
            color: var(--white);
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #000;
            padding: 20px;
            text-align: center;
            border-bottom: 4px solid var(--f1-red);
        }

        .logo { max-width: 200px; }

        nav { margin-top: 15px; }
        nav a { color: white; text-decoration: none; margin: 0 15px; font-weight: bold; text-transform: uppercase; }
        nav a:hover { color: var(--f1-red); }

        .hero {
            position: relative;
            height: 60vh;
            overflow: hidden;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
        }

        #bg-video {
            position: absolute;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: -1;
            filter: brightness(0.4);
        }

        .section { padding: 50px 20px; max-width: 1000px; margin: auto; }
        h2 { border-left: 5px solid var(--f1-red); padding-left: 15px; text-transform: uppercase; }

        /* Formulario Estilo F1 */
        .form-container {
            background-color: var(--card-bg);
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 10px 20px rgba(0,0,0,0.5);
        }

        .form-group { margin-bottom: 20px; }
        label { display: block; margin-bottom: 5px; color: #ccc; }
        input, select, textarea {
            width: 100%;
            padding: 12px;
            background: #2b2b35;
            border: 1px solid #444;
            color: white;
            border-radius: 5px;
        }

        button {
            background-color: var(--f1-red);
            color: white;
            border: none;
            padding: 15px 30px;
            font-weight: bold;
            cursor: pointer;
            width: 100%;
            text-transform: uppercase;
            transition: 0.3s;
        }

        button:hover { background-color: #b00500; transform: scale(1.02); }

        .footer { text-align: center; padding: 40px; background: #000; font-size: 0.8em; }
    </style>
</head>
<body>

<header>
    <img src="logo.png" alt="Amigueros F1 Logo" class="logo">
    <nav>
        <a href="#inicio">Inicio</a>
        <a href="#novedades">Novedades</a>
        <a href="#unirse">Sumate</a>
    </nav>
</header>

<section id="inicio" class="hero">
    <video autoplay muted loop id="bg-video">
        <source src="presentacion.mp4" type="video/mp4">
    </video>
    <div>
        <h1>BIENVENIDOS AL CAMPEONATO AMIGUEROS F1</h1>
        <p>Pasión, velocidad y amistad en cada curva.</p>
    </div>
</section>

<section id="novedades" class="section">
    <h2>Últimas Novedades</h2>
    <p>Seguinos en nuestro Instagram para ver los highlights de cada carrera.</p>
    <a href="https://instagram.com/TU_USUARIO" style="color: var(--f1-red); text-decoration: none;">Ir al Instagram Oficial →</a>
</section>

<section id="unirse" class="section">
    <h2>Formulario de Inscripción</h2>
    <div class="form-container">
        <form action="https://formspree.io/f/f1amigueros@gmail.com" method="POST">
            <div class="form-group">
                <label>Nombre Completo</label>
                <input type="text" name="nombre" required>
            </div>
            
            <div class="form-group">
                <label>País / Bandera</label>
                <input type="text" name="pais" placeholder="Ej: Argentina 🇦🇷">
            </div>

            <div class="form-group">
                <label>Fecha de Nacimiento</label>
                <input type="date" name="nacimiento">
            </div>

            <div class="form-group">
                <label>Usuario de Instagram</label>
                <input type="text" name="instagram" placeholder="@tu_usuario">
            </div>

            <div class="form-group">
                <label>WhatsApp (Número de contacto)</label>
                <input type="tel" name="whatsapp" required>
            </div>

            <div class="form-group">
                <label>Experiencia en Simracing</label>
                <select name="experiencia">
                    <option value="principiante">Principiante</option>
                    <option value="intermedio">Intermedio</option>
                    <option value="avanzado">Avanzado / Pro</option>
                </select>
            </div>

            <div class="form-group">
                <label>¿Qué juego corrés?</label>
                <select name="juego">
                    <option value="F1 24">F1 24</option>
                    <option value="F1 25">F1 25</option>
                    <option value="Ambos">Ambos</option>
                </select>
            </div>

            <div class="form-group">
                <label>Escudería Preferida</label>
                <input type="text" name="equipo" placeholder="Ej: Ferrari, Red Bull...">
            </div>

            <button type="submit">Enviar Solicitud</button>
        </form>
    </div>
</section>

<div class="footer">
    <p>&copy; 2026 Amigueros F1 - Todos los derechos reservados.</p>
</div>

</body>
</html>
