<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jeu d'Énigmes - Accueil</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .container {
            background: white;
            padding: 50px;
            border-radius: 15px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.3);
            max-width: 800px;
            text-align: center;
        }

        h1 {
            font-size: 3em;
            color: #333;
            margin-bottom: 20px;
        }

        .subtitle {
            font-size: 1.2em;
            color: #666;
            margin-bottom: 40px;
        }

        .buttons {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin-bottom: 40px;
        }

        .btn {
            padding: 30px;
            border-radius: 12px;
            border: none;
            cursor: pointer;
            font-size: 1.1em;
            font-weight: 600;
            transition: all 0.3s;
            text-decoration: none;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 10px;
        }

        .btn-admin {
            background: #dc3545;
            color: white;
        }

        .btn-admin:hover {
            background: #c82333;
            transform: translateY(-5px);
            box-shadow: 0 5px 20px rgba(220, 53, 69, 0.3);
        }

        .btn-joueur {
            background: #28a745;
            color: white;
        }

        .btn-joueur:hover {
            background: #218838;
            transform: translateY(-5px);
            box-shadow: 0 5px 20px rgba(40, 167, 69, 0.3);
        }

        .icon {
            font-size: 2em;
        }

        .info {
            background: #f0f4ff;
            padding: 30px;
            border-radius: 12px;
            border-left: 4px solid #667eea;
            margin-bottom: 30px;
            text-align: left;
        }

        .info h2 {
            color: #667eea;
            margin-bottom: 15px;
        }

        .info p {
            color: #666;
            line-height: 1.8;
            margin-bottom: 10px;
        }

        .features {
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
            gap: 20px;
            margin-bottom: 30px;
        }

        .feature {
            padding: 20px;
            background: #f9f9f9;
            border-radius: 8px;
        }

        .feature-icon {
            font-size: 2.5em;
            margin-bottom: 10px;
        }

        .feature-title {
            font-weight: 600;
            color: #333;
            margin-bottom: 8px;
        }

        .feature-desc {
            font-size: 0.9em;
            color: #666;
        }

        .footer {
            color: #999;
            font-size: 0.9em;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #eee;
        }

        @media (max-width: 600px) {
            .container {
                padding: 30px;
            }

            h1 {
                font-size: 2em;
            }

            .buttons {
                grid-template-columns: 1fr;
            }

            .features {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Tu l'as voulu, tu l'as eu</h1>
        <p class="subtitle">suit le cours des énigmes</p>

        <div class="features">
            <div class="feature">
                <div class="feature-icon">✏️</div>
                <div class="feature-title">Créez</div>
                <div class="feature-desc">Créez vos propres énigmes</div>
            </div>
            <div class="feature">
                <div class="feature-icon">🔐</div>
                <div class="feature-title">Sécurisé</div>
                <div class="feature-desc">Les énigmes restent confidentielles</div>
            </div>
            <div class="feature">
                <div class="feature-icon">🎮</div>
                <div class="feature-title">Jouez</div>
                <div class="feature-desc">Partagez et jouez avec vos amis</div>
            </div>
        </div>

        <div class="info">
            <h2>Comment ça marche ?</h2>
            <p>✏️ <strong>Admin</strong> crée des énigmes</p>
            <p>📤 <strong>Admin</strong> partage le lien de jeu</p>
            <p>🎮 <strong>Joueurs</strong> résolvent les énigmes</p>
            <p>🔒 Les énigmes restent invisibles aux joueurs</p>
        </div>

        <div class="buttons">
            <a href="enigmes_admin.html" class="btn btn-admin">
                <div class="icon">🔑</div>
                <div>Espace Admin</div>
            </a>
            <a href="enigmes_joueurs.html" class="btn btn-joueur">
                <div class="icon">🎮</div>
                <div>Jouer</div>
            </a>
        </div>

        <div class="footer">
            <p>💡 Astuce : Les poissons aiment les canards, navigue avec eux</p>
            <p>📱 Fonctionne sur tous les appareils (PC, tablette, téléphone)</p>
        </div>
    </div>
</body>
</html>
