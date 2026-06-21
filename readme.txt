<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Invitación de Boda - Wendy & José</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <link
        href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700&family=Great+Vibes&family=Montserrat:wght@300;400;600&display=swap"
        rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
</head>

<body>

    <main class="invite-container container-fluid p-0">
        
        <section class="screen-section d-flex flex-colum align-items-center justify-content-between p-4 text-center setup-bg-1">
            <div class="vintage-double-border"></div>

            <header class="my-3 animate-fade-in">
                <div class="monogram">W & J</div>
                <div class="vintage-divider"></div>
            </header>

            <div class="main-content animate-fade-in-delayed">
                <h2 class="subtitle-vintage">NUESTRA BODA</h2>
                <h1 class="names-cursive">Wendy & José</h1>
                <p class="date-text mt-3">24 DE JULIO DEL 2027</p>

                <div class="countdown d-flex justify-content-center gap-2 my-4">
                    <div class="countdown-item">
                        <samp id="days">00</samp>
                        <small>Días</small>
                    </div>
                    <div class="countdown-item">
                        <samp id="hours">00</samp>
                        <small>Horas</small>
                    </div>
                    <div class="countdown-item">
                        <samp id="minutes">00</samp>
                        <small>Min</small>
                    </div>
                </div>
            </div>

            <div class="scroll-indicator mb-3">
                <small class="text-uppercase tracking-wider">Desliza para ver mas info</small>
                <div class="arrow-down"></div>
            </div>
        </section> 

        <section class="screen-section d-flex flex-column align-items-center justify-content-center p-4 text-center protocol-section">
            <div class="vintage-double-border"></div>

            <div class="p-3 reveal-on-scroll">
                <p class="vintage-phrase mb-5">
                    "En compañia de nuestros padres, tenemos el honor de invitarte a la boda de..."
                </p>

                <div class="row g-4 my-2">
                    <div class="col-6">
                        <h5 class="parent-title">Padres de la Novia</h5>
                        <p class="parent-name">Eleazar Dominguez.<br>Rosario Valencia.</p>
                    </div>
                    <div class="col-6">
                        <h5 class="parent-title">Padres del Novio</h5>
                        <p class="parent-name">Mateo Porquillo.<br>Maricela Hernandez.</p>
                    </div>
                </div>

                <div class="vintage-divider my-4"></div>

                <div>
                    <h4 class="subtitle-vintage mb-3">Nuestros Padrinos</h4>
                    <p class="parent-name"><strong>De Invitación</strong> Paul Dominguez</p>
                </div>
            </div>
        </section>

        <section class="screen-section d-flex flex-column align-items-center justify-content-center p-4 text-center location-section">
            <div class="vintage-overlay"></div>
            <div class="vintage-double-border"></div>

            <div class="position-relative z-index-2 reveal-on-scroll">
                <h2 class="subtitle-vintage text-white mb-4">¿Donde y Cuándo?</h2>
                <p class="location-details text-white">La ceremonia y recepción se llevara a cabo en la casa roma.</p>
                <p class="location-time text-white-50">Recepción: 6:00 hrs</p>

                <a href="https://maps.google.com" target="_blank" class="btn btn-vintage-gold mt-3">Ver ubicación en el mapa</a>
            </div>
        </section>

        <section class="screen-section d-flex flex-column align-items-center justify-content-center p-4 text-center dresscode-section">
            <div class="vintage-double-border"></div>

            <div class="reveal-on-scroll">
                <h2 class="subtitle-vintage mb-3">Codigo de vestimenta</h2>
                <h4 class="dress-type mb-4">Formal</h4>

                <div class="dress-code-img-wrapper mx-auto mb-4">
                    <div class="placeholder-img d-flex align-items-center justify-content-center text-muted">
                        <span>[Foto de ejemplo]</span>
                    </div>
                </div>

                <p class="parent-name px-3">Agradecemos evitar el uso del color blanco y derivados.</p>
            </div>
        </section>

        <section class="screen-section d-flex flex-column align-items-center justify-content-center p-4 text-center end-section">
            <div class="vintage-double-border"></div>

            <div class="w-100 px-3 reveal-on-scroll">
                <h2 class="names-cursive mb-5" style="font-size: 3.5rem;">!Te esperamos!</h2>

                <div class="d-grind gap-3 max-button-width mx-auto">
                    <a href="#" class="btn btn-vintage">Confirmar Asistencia</a>
                    <a href="#" class="btn bnt-vintage-outline">Mesa de regalos</a>
                </div>
            </div>
        </section>

    </main>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>

    <script>
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('active');
                }
            });
        }, { threshold: 0.15});

        document.querySelectorAll('.reveal-on-scroll').forEach((el) => observer.observe(el));
    </script>
</body>

</html>