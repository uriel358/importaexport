<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>ImportaExpor | Logística y Envíos entre EE.UU., España y Venezuela</title>
    <meta name="description" content="Soluciones integrales de paquetería, agenciamiento aduanal y procura internacional. Conectamos Estados Unidos y España con Venezuela de forma segura y eficiente.">
    <meta name="keywords" content="envíos a Venezuela, aduana Venezuela, importación desde USA, importación desde España, procura internacional, paquetería internacional, logística internacional">
    <meta name="author" content="ImportaExpor">

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&display=swap" rel="stylesheet">

    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">

    <link rel="icon" href="./images/favicon importaexport.jpg" type="image/jpeg">

    <style>
        /* --------------------------------------------------
        CSS - En un proyecto real, esto iría en un archivo separado (ej. styles.css)
        -------------------------------------------------- */
        :root {
            --primary-blue: #00008B; /* Azul Rey */
            --accent-green: #2E8B57; /* Verde Esmeralda Oscuro */
            --light-gray: #f4f7fc; /* Fondo claro para secciones */
            --dark-text: #2c3e50; /* Texto oscuro principal */
            --light-text: #ffffff; /* Texto claro */
            --gray-text: #7f8c8d; /* Texto secundario/gris */
            --font-family: 'Poppins', sans-serif;
            --box-shadow: 0 10px 30px rgba(0, 0, 139, 0.1); /* Ajustado a primary-blue */
            --border-radius: 8px;
        }

        /* --- Reseteo Básico y Estilos Globales --- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
            font-size: 16px;
        }

        body {
            font-family: var(--font-family);
            color: var(--dark-text);
            line-height: 1.7;
            background-color: var(--light-text);
        }

        h1, h2, h3, h4, h5, h6 {
            font-weight: 600;
            line-height: 1.3;
        }

        h1 { font-size: 3.2rem; color: var(--light-text); }
        h2 { font-size: 2.2rem; color: var(--primary-blue); text-align: center; margin-bottom: 1rem; }
        h3 { font-size: 1.4rem; color: var(--primary-blue); }

        p {
            color: var(--gray-text);
            margin-bottom: 1rem;
        }

        a {
            text-decoration: none;
            color: var(--accent-green);
            transition: color 0.3s ease;
        }

        img {
            max-width: 100%;
            height: auto;
            display: block;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }

        section {
            padding: 5rem 0;
        }

        .section-subtitle {
            text-align: center;
            max-width: 700px;
            margin: 0 auto 3rem auto;
            color: var(--gray-text);
        }

        .btn {
            display: inline-block;
            padding: 0.8rem 2rem;
            background-color: var(--accent-green);
            color: var(--light-text);
            font-weight: 500;
            border-radius: 50px;
            transition: transform 0.3s ease, background-color 0.3s ease;
            border: 2px solid var(--accent-green);
            text-transform: uppercase;
            letter-spacing: 0.5px;
            font-size: 0.9rem;
        }

        .btn:hover {
            transform: translateY(-3px);
            background-color: #226641; /* Tono de verde más oscuro para el hover */
            border-color: #226641; /* Coincide con el hover */
        }

        .btn-secondary {
            background-color: transparent;
            color: var(--primary-blue);
            border-color: var(--primary-blue);
        }

        .btn-secondary:hover {
            background-color: var(--primary-blue);
            color: var(--light-text);
        }

        /* --- Animación de entrada --- */
        .fade-in {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.6s ease-out, transform 0.6s ease-out;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* --- Header y Navegación --- */
        .header {
            background-color: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            left: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
        }

        .header .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-weight: 700;
            font-size: 1.8rem;
            color: var(--primary-blue);
            display: flex; /* Para alinear el logo si es una imagen */
            align-items: center;
        }
        .logo span { color: var(--accent-green); }
        .logo img {
            height: 40px; /* Ajusta el tamaño del logo */
            margin-right: 10px;
        }

        .nav-links {
            list-style: none;
            display: flex;
            align-items: center;
        }

        .nav-links li {
            margin-left: 2.5rem;
        }

        .nav-links a {
            color: var(--dark-text);
            font-weight: 500;
            font-size: 1rem;
            position: relative;
            padding-bottom: 5px;
        }

        .nav-links a:not(.btn)::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background-color: var(--accent-green);
            transition: width 0.3s ease;
        }

        .nav-links a:not(.btn):hover::after, .nav-links a:not(.btn).active::after {
            width: 100%;
        }

        .menu-toggle {
            display: none;
            font-size: 1.5rem;
            background: none;
            border: none;
            color: var(--primary-blue);
            cursor: pointer;
        }

        /* --- Sección Hero --- */
        #hero {
            /* IMAGEN DE FONDO DEL HERO */
            background: linear-gradient(rgba(0, 0, 139, 0.8), rgba(0, 0, 139, 0.7)), url('https://images.unsplash.com/photo-1578575437130-5b1273dc9798?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D') no-repeat center center/cover;
            min-height: 650px;
            display: flex;
            align-items: center;
            text-align: center;
            padding-top: 8rem;
            padding-bottom: 4rem;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }

        #hero h1 {
            margin-bottom: 1rem;
            font-weight: 700;
        }

        #hero p {
            font-size: 1.2rem;
            color: rgba(255, 255, 255, 0.9);
            margin-bottom: 2.5rem;
        }

        /* --- Sección Servicios --- */
        #services {
            background-color: var(--light-gray);
        }
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .service-card {
            background-color: var(--light-text);
            padding: 2.5rem 2rem;
            text-align: center;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0, 0, 139, 0.15); /* Ajustado a primary-blue */
        }

        /* Estilo para las imágenes dentro de las tarjetas de servicio */
        .service-card img {
            max-width: 120px; /* Tamaño un poco más ajustado para íconos */
            height: 120px; /* Mantener proporción si es cuadrada */
            object-fit: contain; /* Asegura que la imagen se vea completa */
            margin: 0 auto 1.5rem auto; /* Centrar y añadir margen inferior */
            border-radius: 8px; /* Bordes ligeramente redondeados */
            padding: 10px; /* Espacio alrededor de la imagen */
            background-color: #f0f3f8; /* Un fondo muy suave para las imágenes */
        }

        .service-card h3 {
            margin-bottom: 1rem;
        }

        /* --- Sección "Cómo Funciona" --- */
        .process-flow {
            display: flex;
            justify-content: space-between;
            position: relative;
            margin-top: 4rem;
        }

        .process-flow::before {
            content: '';
            position: absolute;
            top: 30px;
            left: 10%;
            right: 10%;
            height: 2px;
            background-color: #e0e0e0;
            z-index: -1;
        }

        .process-step {
            text-align: center;
            width: 23%;
        }

        .step-number {
            width: 60px;
            height: 60px;
            background-color: var(--light-text);
            color: var(--primary-blue);
            border: 2px solid var(--primary-blue);
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 1.5rem;
            font-weight: 700;
            margin: 0 auto 1.5rem auto;
            transition: all 0.3s ease;
        }

        .process-step:hover .step-number {
            background-color: var(--primary-blue);
            color: var(--light-text);
            transform: scale(1.1);
        }

        .process-step h4 {
            font-size: 1.1rem;
            margin-bottom: 0.5rem;
            color: var(--dark-text);
        }

        /* --- Sección Cobertura --- */
        #coverage {
            background-color: var(--light-gray);
        }

        .coverage-wrapper {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .route-card {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 2rem;
            margin-bottom: 2rem;
            background-color: white;
            padding: 2rem 3rem;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            width: 100%;
            max-width: 800px;
        }

        .country-flag {
            font-size: 4rem;
        }

        .arrows {
            font-size: 2.5rem;
            color: var(--accent-green);
        }

        /* --- Sección Por Qué Elegirnos --- */
        #why-us {
            background-color: var(--light-text); /* Asegura que tenga el mismo fondo que las cards si es necesario */
        }

        .why-us-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }
        .feature-item {
            display: flex;
            align-items: flex-start;
            gap: 1.5rem;
        }
        .feature-item .icon {
            font-size: 2.5rem;
            color: var(--primary-blue);
        }
        .feature-item h4 {
            color: var(--dark-text);
        }

        /* --- Banner CTA --- */
        #cta-banner {
            /* IMAGEN DE FONDO DEL CTA BANNER */
            background: linear-gradient(rgba(0, 0, 139, 0.85), rgba(0, 0, 139, 0.85)), url('https://images.unsplash.com/photo-1587327918459-7176465451a5?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D') no-repeat center center/cover;
            padding: 5rem 0;
            text-align: center;
        }
        #cta-banner h2 {
            color: var(--light-text);
            margin-bottom: 1rem;
        }
        #cta-banner p {
            color: rgba(255, 255, 255, 0.8);
            max-width: 600px;
            margin: 0 auto 2rem auto;
        }

        /* --- Contacto --- */
        #contact {
            background-color: var(--light-gray);
        }
        .contact-wrapper {
            display: grid;
            grid-template-columns: 1.5fr 1fr;
            gap: 3rem;
            align-items: flex-start;
        }
        .contact-form {
            background: var(--light-text);
            padding: 2.5rem;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
        }
        .contact-form h3 {
            margin-bottom: 1.5rem;
        }
        .form-group {
            margin-bottom: 1.5rem;
        }
        .form-group input, .form-group textarea {
            width: 100%;
            padding: 1rem;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-family: var(--font-family);
        }
        .form-group input:focus, .form-group textarea:focus {
            outline: none;
            border-color: var(--accent-green);
        }

        .contact-info-item {
            margin-bottom: 1.5rem;
            display: flex;
            gap: 1rem;
            align-items: center;
        }
        .contact-info-item .icon {
            font-size: 1.5rem;
            color: var(--accent-green);
        }

        /* --- Footer --- */
        .footer {
            background-color: var(--primary-blue);
            color: var(--light-text);
            padding: 4rem 0 2rem 0;
        }
        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 3rem;
        }
        .footer-col h4 {
            color: var(--light-text);
            margin-bottom: 1rem;
            font-weight: 600;
        }
        .footer-col p, .footer-col ul li a {
            color: rgba(255, 255, 255, 0.8);
        }
        .footer-col ul { list-style: none; }
        .footer-col ul li { margin-bottom: 0.5rem; }
        .footer-col ul li a:hover { color: var(--accent-green); }

        .social-links a {
            display: inline-block;
            width: 40px;
            height: 40px;
            line-height: 40px;
            text-align: center;
            background-color: rgba(255, 255, 255, 0.1);
            color: var(--light-text);
            margin-right: 0.5rem;
            border-radius: 50%;
            transition: background-color 0.3s ease, color 0.3s ease;
        }
        .social-links a:hover {
            background-color: var(--accent-green);
        }
        .footer-bottom {
            text-align: center;
            padding-top: 2rem;
            border-top: 1px solid rgba(255, 255, 255, 0.2);
            font-size: 0.9rem;
            color: rgba(255, 255, 255, 0.7);
        }

        /* --- Media Queries para Responsividad --- */
        @media (max-width: 992px) {
            .nav-links li:not(:last-child) { display: none; } /* Oculta links normales, deja el botón */
            .contact-wrapper { grid-template-columns: 1fr; }
        }

        @media (max-width: 768px) {
            h1 { font-size: 2.5rem; }
            h2 { font-size: 1.8rem; }
            section { padding: 3rem 0; }

            .nav-links {
                position: fixed;
                top: 0;
                right: -100%;
                width: 70%;
                max-width: 300px;
                height: 100vh;
                background-color: var(--light-text);
                flex-direction: column;
                align-items: flex-start;
                padding: 6rem 2rem 2rem;
                box-shadow: -5px 0 15px rgba(0,0,0,0.1);
                transition: right 0.4s ease-in-out;
            }
            .nav-links.active { right: 0; }
            .nav-links li { margin: 1rem 0; display: block; }
            .nav-links .btn { display: inline-block; margin-top: 1rem; }
            .menu-toggle { display: block; z-index: 1001; }

            #hero { min-height: auto; }
            .process-flow { flex-direction: column; gap: 2rem; }
            .process-flow::before { display: none; }
            .process-step { width: 100%; }
            .route-card { flex-direction: column; text-align: center; }
        }
    </style>
</head>
<body>

    <header class="header">
        <div class="container">
            <a href="#hero" class="logo">
                <img src="./images/Logo importaexport.png" alt="Logo ImportaExpor">
                Importa<span>Expor</span>
            </a>

            <nav>
                <ul class="nav-links">
                    <li><a href="#services">Servicios</a></li>
                    <li><a href="#process">Cómo Funciona</a></li>
                    <li><a href="#coverage">Cobertura</a></li>
                    <li><a href="https://wa.me/584241933061?text=Hola!%20Me%20gustaría%20solicitar%20una%20cotización%20para%20un%20envío." class="btn" target="_blank" rel="noopener noreferrer">Solicitar Cotización</a></li>
                </ul>
            </nav>

            <button class="menu-toggle" id="menu-toggle" aria-label="Abrir menú">
                <i class="fas fa-bars"></i>
            </button>
        </div>
    </header>

    <main>
        <section id="hero">
            <div class="container hero-content fade-in">
                <h1>Conectamos tu Mundo.<br>Logística sin Fronteras.</h1>
                <p>Tu socio confiable para envíos, aduanas y compras entre Estados Unidos, España y Venezuela. Simple, seguro y a tiempo.</p>
                <a href="https://wa.me/584241933061?text=Hola!%20Me%20gustaría%20solicitar%20una%20cotización%20para%20un%20envío%20desde%20la%20sección%20Hero." class="btn" target="_blank" rel="noopener noreferrer">Solicitar Cotización Ahora</a>
            </div>
        </section>

        <section id="services">
            <div class="container">
                <h2 class="fade-in">Nuestras Soluciones Integrales</h2>
                <p class="section-subtitle fade-in">Diseñamos soluciones a la medida de tus necesidades, ya seas una empresa o un particular.</p>
                <div class="services-grid">
                    <div class="service-card fade-in" style="transition-delay: 0.1s;">
                        <img src="https://images.pexels.com/photos/3760067/pexels-photo-3760067.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2" alt="Envío Aéreo y Marítimo">
                        <h3>Envío Aéreo y Marítimo</h3>
                        <p>Transportamos tu paquetería y carga de forma rápida y segura. Ofrecemos opciones flexibles para adaptarnos a tu presupuesto y urgencia.</p>
                    </div>
                    <div class="service-card fade-in" style="transition-delay: 0.2s;">
                        <img src="https://images.pexels.com/photos/3862638/pexels-photo-3862638.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2" alt="Agenciamiento Aduanal">
                        <h3>Agenciamiento Aduanal</h3>
                        <p>Nos encargamos de todos los trámites de importación y exportación, garantizando un proceso de desaduanamiento fluido y sin complicaciones.</p>
                    </div>
                    <div class="service-card fade-in" style="transition-delay: 0.3s;">
                        <img src="https://images.pexels.com/photos/3956488/pexels-photo-3956488.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2" alt="Servicio de Procura">
                        <h3>Servicio de Procura</h3>
                        <p>Compramos por ti en tiendas de EE.UU. y España. Consigue los productos que necesitas y nosotros nos encargamos de llevarlos hasta tu puerta.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="process">
            <div class="container">
                <h2 class="fade-in">Nuestro Proceso en 4 Simples Pasos</h2>
                <p class="section-subtitle fade-in">Hemos simplificado la logística internacional para que tu experiencia sea transparente y sin estrés.</p>
                <div class="process-flow">
                    <div class="process-step fade-in" style="transition-delay: 0.1s;">
                        <div class="step-number">1</div>
                        <h4>Cotiza y Registra</h4>
                        <p>Contáctanos con los detalles de tu envío o compra para recibir una cotización personalizada.</p>
                    </div>
                    <div class="process-step fade-in" style="transition-delay: 0.2s;">
                        <div class="step-number">2</div>
                        <h4>Envía a nuestro Almacén</h4>
                        <p>Haz llegar tu carga o tus compras a nuestras bodegas seguras en Miami o Madrid.</p>
                    </div>
                    <div class="process-step fade-in" style="transition-delay: 0.3s;">
                        <div class="step-number">3</div>
                        <h4>Proceso y Aduana</h4>
                        <p>Consolidamos, re-empacamos si es necesario, y gestionamos todo el papeleo aduanal.</p>
                    </div>
                    <div class="process-step fade-in" style="transition-delay: 0.4s;">
                        <div class="step-number">4</div>
                        <h4>Entrega en Destino</h4>
                        <p>Recibe tu mercancía en la puerta de tu casa u oficina en Venezuela. ¡Así de fácil!</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="coverage">
            <div class="container">
                <h2 class="fade-in">Rutas Estratégicas a tu Servicio</h2>
                <p class="section-subtitle fade-in">Especialistas en los corredores comerciales más importantes para Venezuela.</p>
                <div class="coverage-wrapper">
                    <div class="route-card fade-in">
                        <div class="country-flag" role="img" aria-label="Bandera de Estados Unidos">🇺🇸</div>
                        <div class="arrows"><i class="fas fa-exchange-alt"></i></div>
                        <div class="country-flag" role="img" aria-label="Bandera de Venezuela">🇻🇪</div>
                    </div>
                    <div class="route-card fade-in" style="transition-delay: 0.2s;">
                        <div class="country-flag" role="img" aria-label="Bandera de España">🇪🇸</div>
                        <div class="arrows"><i class="fas fa-exchange-alt"></i></div>
                        <div class="country-flag" role="img" aria-label="Bandera de Venezuela">🇻🇪</div>
                    </div>
                </div>
            </div>
        </section>

        <section id="why-us">
            <div class="container">
                <h2 class="fade-in">¿Por Qué Confiar en ImportaExpor?</h2>
                   <p class="section-subtitle fade-in">No solo movemos cajas, entregamos tranquilidad.</p>
                <div class="why-us-grid">
                    <div class="feature-item fade-in">
                        <div class="icon"><i class="fas fa-shield-alt"></i></div>
                        <div>
                            <h4>Seguridad Garantizada</h4>
                            <p>Tu carga está protegida en cada etapa del viaje. Ofrecemos opciones de seguro para tu total tranquilidad.</p>
                        </div>
                    </div>
                    <div class="feature-item fade-in">
                        <div class="icon"><i class="fas fa-user-tie"></i></div>
                        <div>
                            <h4>Experiencia Comprobada</h4>
                            <p>Años de experiencia en el complejo mundo de la aduana venezolana nos permiten anticipar y resolver cualquier reto.</p>
                        </div>
                    </div>
                    <div class="feature-item fade-in">
                        <div class="icon"><i class="fas fa-headset"></i></div>
                        <div>
                            <h4>Atención Personalizada</h4>
                            <p>Un asesor dedicado te acompañará durante todo el proceso, respondiendo a tus dudas de forma rápida y clara.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="cta-banner" class="fade-in">
            <div class="container">
                <h2>¿Listo para empezar a importar o exportar?</h2>
                <p>Nuestro equipo de expertos está listo para asesorarte y ofrecerte la mejor solución logística para tus necesidades.</p>
                <a href="https://wa.me/584241933061?text=Hola!%20Me%20gustaría%20hablar%20sobre%20un%20proyecto%20de%20logística%20que%20tengo." class="btn" target="_blank" rel="noopener noreferrer">Hablemos de tu Proyecto</a>
            </div>
        </section>

        <section id="contact">
            <div class="container">
                   <h2 class="fade-in">Ponte en Contacto</h2>
                   <p class="section-subtitle fade-in">Rellena el formulario para obtener una cotización o resolver tus dudas. Te responderemos en menos de 24 horas.</p>
                   <div class="contact-wrapper">
                    <div class="contact-form fade-in" style="transition-delay: 0.2s;">
                        <h3>Formulario de Cotización</h3>
                        <form action="#" method="POST">
                             <div class="form-group">
                                 <input type="text" id="name" name="name" required placeholder="Nombre Completo">
                             </div>
                             <div class="form-group">
                                 <input type="email" id="email" name="email" required placeholder="Correo Electrónico">
                             </div>
                             <div class="form-group">
                                 <input type="tel" id="phone" name="phone" required placeholder="Teléfono (Opcional)">
                             </div>
                             <div class="form-group">
                                 <textarea id="message" name="message" rows="5" required placeholder="Describe tu envío o la compra que deseas realizar..."></textarea>
                             </div>
                             <button type="submit" class="btn">Enviar Solicitud</button>
                           </form>
                    </div>
                    <div class="contact-info fade-in" style="transition-delay: 0.4s;">
                        <h3>Nuestra Oficina</h3>
                        <div class="contact-info-item">
                            <div class="icon"><i class="fas fa-map-marker-alt"></i></div>
                            <div>
                                <h4>Caracas, Venezuela</h4>
                                <p>Av. Francisco de Miranda, Torre A, Piso 10, Chacao, Caracas, 1060.</p>
                            </div>
                        </div>
                           <div class="contact-info-item">
                            <div class="icon"><i class="fas fa-warehouse"></i></div>
                            <div>
                                <h4>Almacenes</h4>
                                <p>Recibe tus paquetes en nuestras sedes de Miami (EE.UU.) y Madrid (España).</p>
                            </div>
                        </div>
                        <div class="contact-info-item">
                            <div class="icon"><i class="fas fa-phone-alt"></i></div>
                            <div>
                                <h4>Teléfono</h4>
                                <p><a href="tel:+582129555555">+58 (212) 955-5555</a></p>
                            </div>
                        </div>
                        <div class="contact-info-item">
                            <div class="icon"><i class="fas fa-envelope"></i></div>
                            <div>
                                <h4>Email</h4>
                                <p><a href="mailto:info@importaexpor.com">info@importaexpor.com</a></p>
                            </div>
                        </div>
                       </div>
                   </div>
            </div>
        </section>
    </main>

    <footer class="footer">
        <div class="container">
            <div class="footer-grid">
                <div class="footer-col">
                    <h4>Importa<span>Expor</span></h4>
                    <p>Conectando oportunidades, entregando confianza. Tu aliado en logística internacional.</p>
                </div>
                <div class="footer-col">
                    <h4>Navegación</h4>
                    <ul>
                        <li><a href="#hero">Inicio</a></li>
                        <li><a href="#services">Servicios</a></li>
                        <li><a href="#process">Cómo Funciona</a></li>
                        <li><a href="#contact">Contacto</a></li>
                        <li><a href="#coverage">Cobertura</a></li>
                    </ul>
                </div>
                   <div class="footer-col">
                    <h4>Servicios</h4>
                    <ul>
                        <li><a href="#services">Envío Aéreo y Marítimo</a></li>
                        <li><a href="#services">Agenciamiento Aduanal</a></li>
                        <li><a href="#services">Servicio de Procura</a></li>
                    </ul>
                </div>
                <div class="footer-col">
                    <h4>Síguenos</h4>
                    <p>Mantente al día con nuestras noticias y ofertas.</p>
                    <div class="social-links">
                        <a href="#" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
                        <a href="#" aria-label="Facebook"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" aria-label="LinkedIn"><i class="fab fa-linkedin-in"></i></a>
                    </div>
                </div>
            </div>
            <div class="footer-bottom">
                <p>&copy; 2025 ImportaExpor. Todos los derechos reservados. Diseñado por un experto para el éxito global.</p>
            </div>
        </div>
    </footer>

    <script>
    /* --------------------------------------------------
    JAVASCRIPT - En un proyecto real, esto iría en un archivo separado (ej. script.js)
    -------------------------------------------------- */
    document.addEventListener('DOMContentLoaded', function() {

        // --- Manejo del menú móvil ---
        const menuToggle = document.getElementById('menu-toggle');
        const navLinks = document.querySelector('.nav-links');
        const navLinkItems = document.querySelectorAll('.nav-links a');

        menuToggle.addEventListener('click', () => {
            navLinks.classList.toggle('active');
            const icon = menuToggle.querySelector('i');
            if (navLinks.classList.contains('active')) {
                icon.classList.remove('fa-bars');
                icon.classList.add('fa-times'); // Cambia a una 'X' al abrir
            } else {
                icon.classList.remove('fa-times');
                icon.classList.add('fa-bars'); // Vuelve al icono de hamburguesa al cerrar
            }
        });

        navLinkItems.forEach(item => {
            item.addEventListener('click', () => {
                navLinks.classList.remove('active');
                menuToggle.querySelector('i').classList.remove('fa-times');
                menuToggle.querySelector('i').classList.add('fa-bars');
            });
        });

        // --- Animación de elementos al hacer scroll (fade-in) ---
        const faders = document.querySelectorAll('.fade-in');

        const appearOptions = {
            threshold: 0.3, // Percentage of element visible to trigger
            rootMargin: "0px 0px -50px 0px" // Adjusts when the element appears relative to the viewport
        };

        const appearOnScroll = new IntersectionObserver(function(
            entries,
            appearOnScroll
        ) {
            entries.forEach(entry => {
                if (!entry.isIntersecting) {
                    return;
                } else {
                    entry.target.classList.add('visible');
                    appearOnScroll.unobserve(entry.target);
                }
            });
        },
        appearOptions);

        faders.forEach(fader => {
            appearOnScroll.observe(fader);
        });

    });
    </script>
</body>
</html>
