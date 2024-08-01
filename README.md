<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Depósito de Gás e Água do Naldo</title>
    <link rel="stylesheet" href="styles.css">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/js/all.min.js" integrity="sha512-HbZsOXXpdI8QK/6xJzO2fl8WgH9Qw3/9D5H/R9Gg6ZNGG8h0PzGo2Pz4LxK7T4LB+gO8HSp6qF3Di5Iht5J6g==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
</head>
<body>
    <header>
        <h1>Depósito de Gás e Água do Naldo</h1>
        <nav>
            <ul>
                <li><a href="#contato">Contato</a></li>
                <li><a href="#mapa">Localização</a></li>
                <li><a href="#youtube">Canal do YouTube</a></li>
                <li><a href="#menu">Menu</a></li>
                <li><a href="#tradutor">Tradutor</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="contato">
            <h2>Contato</h2>
            <p>Telefone: (88)9 8868-1421</p>
            <p>Email: contato@depósito-naldo.com</p>
        </section>

        <section id="mapa">
            <h2>Localização</h2>
            <div id="map"></div>
        </section>

        <section id="youtube">
            <h2>Canal do YouTube</h2>
            <a href="https://www.youtube.com/channel/SEU_CANAL" target="_blank">Visite nosso canal!</a>
        </section>

        <section id="menu">
            <h2>Menu</h2>
            <p>Conteúdo do menu aqui.</p>
        </section>

        <section id="tradutor">
            <h2>Tradutor</h2>
            <div id="google_translate_element"></div>
        </section>
    </main>

    <footer>
        <div>
            <a href="https://www.facebook.com/sharer/sharer.php?u=SEU_LINK" target="_blank" class="social-icon"><i class="fab fa-facebook-f"></i></a>
            <a href="https://twitter.com/intent/tweet?url=SEU_LINK" target="_blank" class="social-icon"><i class="fab fa-twitter"></i></a>
            <a href="https://www.instagram.com/?url=SEU_LINK" target="_blank" class="social-icon"><i class="fab fa-instagram"></i></a>
        </div>
    </footer>

    <script src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&callback=initMap" async defer></script>
    <script src="https://translate.google.com/translate_a/element.js?cb=googleTranslateElementInit"></script>
    <script>
        function initMap() {
            var location = { lat: -23.550520, lng: -46.633308 }; // Alterar para a localização do depósito
            var map = new google.maps.Map(document.getElementById('map'), {
                zoom: 15,
                center: location
            });
            new google.maps.Marker({
                position: location,
                map: map
            });
        }

        function googleTranslateElementInit() {
            new google.translate.TranslateElement({pageLanguage: 'pt'}, 'google_translate_element');
        }
    </script>
</body>
</html>
