<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <>Marketing de jeux vidéo</title>
    <style>
        /* Styles CSS */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        .promotion {
            text-align: center;
            background-color: #f2f2f2;
            padding: 20px;
        }
        .partage {
            text-align: center;
            margin-top: 20px;
        }
        .partage img {
            width: 30px;
            margin: 0 10px;
        }
        .popup {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background-color: #fff;
            padding: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
            display: none;
        }
        .popup img {
            max-width: 100%;
            height: auto;
        }
        .popup .fermer {
            display: block;
            text-align: center;
            margin-top: 10px;
            color: #333;
            text-decoration: none;
        }
    </style>
</head>
<body>

<div class="promotion">
    <img src="chemin_vers_l_image.jpg" alt="Promotion en cours">
    <p>Profitez de notre promotion spéciale pour les nouveaux jeux !</p>
    <a href="lien_vers_la_page_de_promotion">En savoir plus</a>
</div>

<form action="votre_script_de_traitement.php" method="post">
    <input type="email" name="email" placeholder="Entrez votre adresse e-mail" required>
    <input type="submit" value="S'inscrire à la newsletter">
</form>

<div class="partage">
    <a href="lien_vers_facebook" target="_blank"><img src="facebook_icon.png" alt="Facebook"></a>
    <a href="lien_vers_twitter" target="_blank"><img src="twitter_icon.png" alt="Twitter"></a>
    <a href="lien_vers_instagram" target="_blank"><img src="instagram_icon.png" alt="Instagram"></a>
</div>

<iframe width="560" height="315" src="lien_vers_la_video" frameborder="0" allowfullscreen></iframe>

<div class="popup">
    <img src="promo_popup_image.jpg" alt="Promotion">
    <a href="#" class="fermer">Fermer</a>
</div>

<script>
    // JavaScript pour afficher la popup
    document.addEventListener("DOMContentLoaded", function() {
        var popup = document.querySelector('.popup');
        var fermerPopup = document.querySelector('.popup .fermer');

        // Afficher la popup après 5 secondes
        setTimeout(function() {
            popup.style.display = 'block';
        }, 5000);

        // Fermer la popup lorsqu'on clique sur le lien de fermeture
        fermerPopup.addEventListener('click', function(e) {
            e.preventDefault();
            popup.style.display = 'none';
        });
    });
</script>

</body>
</html>
