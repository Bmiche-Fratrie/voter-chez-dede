<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Redirection vers la modale de vote</title>
    <script>
        window.onload = function() {
            // URL de la friterie
            const targetUrl = "https://www.les-friteries.com/site/friture-chez-dede-paliseul";
            window.location.href = targetUrl;

            // Attendre que la page se charge, puis simuler un clic sur le bouton de vote
            setTimeout(function() {
                const voteButton = document.querySelector(".btn.btn-danger.btn-events[data-bs-target='#myModal']");
                if (voteButton) {
                    voteButton.click();
                }
            }, 2000); // Ajuster le délai si nécessaire
        };
    </script>
</head>
<body>
    <p>Redirection en cours...</p>
</body>
</html>
