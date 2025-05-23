
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Syléa - Votre trajectoire, éclairée par l'intelligence</title>
    <style>
        /* Variables globales */
        :root {
            --primary-color: #212529;         /* Noir principal */
            --secondary-color: #f8f9fa;       /* Blanc/gris très clair */
            --accent-color: #5e60ce;          /* Légère touche de violet */
            --hover-color: #4e4fc0;           /* Violet plus foncé pour hover */
            --font-main: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            --transition-speed: 0.3s;
        }

        /* Reset CSS */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Styles de base */
        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: var(--font-main);
            line-height: 1.6;
            color: var(--primary-color);
            background-color: var(--secondary-color);
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Navigation */
        header {
            padding: 24px 0;
            background-color: rgba(255, 255, 255, 0.98);
            backdrop-filter: blur(5px);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.03);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 24px;
            font-weight: 600;
            letter-spacing: -0.5px;
            color: var(--primary-color);
            text-decoration: none;
        }

        /* Hero Section */
        .hero {
            padding: 160px 0 100px;
            text-align: center;
            background: linear-gradient(to bottom right, rgba(94, 96, 206, 0.03), rgba(255, 255, 255, 0));
        }

        .hero h1 {
            font-size: 48px;
            font-weight: 700;
            letter-spacing: -1px;
            margin-bottom: 16px;
            line-height: 1.2;
        }

        .hero p.tagline {
            font-size: 24px;
            color: #495057;
            margin-bottom: 32px;
            font-weight: 400;
        }

        .hero .description {
            max-width: 650px;
            margin: 0 auto 48px;
            font-size: 18px;
            color: #495057;
        }

        .cta-button {
            display: inline-block;
            padding: 14px 32px;
            background-color: var(--accent-color);
            color: white;
            border-radius: 6px;
            font-size: 16px;
            font-weight: 500;
            text-decoration: none;
            transition: all var(--transition-speed) ease;
            border: none;
            cursor: pointer;
        }

        .cta-button:hover {
            background-color: var(--hover-color);
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(94, 96, 206, 0.2);
        }

        /* How it works section */
        .how-it-works {
            padding: 100px 0;
            background-color: white;
        }

        .section-title {
            text-align: center;
            font-size: 32px;
            font-weight: 600;
            margin-bottom: 64px;
            letter-spacing: -0.5px;
        }

        .steps {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 40px;
        }

        .step {
            flex: 1;
            min-width: 250px;
            text-align: center;
            padding: 30px;
            border-radius: 12px;
            transition: all var(--transition-speed) ease;
        }

        .step:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.04);
        }

        .step-icon {
            width: 80px;
            height: 80px;
            margin: 0 auto 24px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            background-color: rgba(94, 96, 206, 0.1);
        }

        .step-icon svg {
            width: 40px;
            height: 40px;
            color: var(--accent-color);
        }

        .step h3 {
            margin-bottom: 16px;
            font-size: 20px;
            font-weight: 600;
        }

        .step p {
            color: #6c757d;
            font-size: 16px;
        }

        /* Footer */
        footer {
            padding: 40px 0;
            text-align: center;
            background-color: var(--secondary-color);
            color: #6c757d;
            font-size: 14px;
        }

        /* Form styles */
        .prototype-form {
            max-width: 600px;
            margin: 0 auto;
            padding: 40px;
            border-radius: 12px;
            background-color: white;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.05);
        }

        .prototype-form h2 {
            margin-bottom: 32px;
            text-align: center;
            font-size: 24px;
            font-weight: 600;
        }

        .form-field {
            margin-bottom: 24px;
        }

        .form-field label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
            color: var(--primary-color);
        }

        .form-field input,
        .form-field select,
        .form-field textarea {
            width: 100%;
            padding: 12px 16px;
            border: 1px solid #dee2e6;
            border-radius: 6px;
            font-family: var(--font-main);
            font-size: 16px;
            transition: border-color var(--transition-speed) ease;
        }

        .form-field input:focus,
        .form-field select:focus,
        .form-field textarea:focus {
            outline: none;
            border-color: var(--accent-color);
        }
        
        /* Results Styles */
        .results-container {
            margin-top: 40px;
            padding-top: 30px;
            border-top: 1px solid #eee;
            text-align: center;
        }
        
        .results-container h3 {
            margin-bottom: 30px;
            font-size: 22px;
            font-weight: 600;
        }
        
        .results-grid {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 20px;
            margin-bottom: 30px;
        }
        
        .result-card {
            flex: 1;
            min-width: 200px;
            padding: 24px;
            border-radius: 10px;
            background-color: #f8f9fa;
            transition: all var(--transition-speed) ease;
        }
        
        .result-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.05);
        }
        
        .result-card h4 {
            margin-bottom: 16px;
            font-size: 18px;
            font-weight: 600;
        }
        
        .probability-circle {
            width: 120px;
            height: 120px;
            margin: 0 auto;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            background: linear-gradient(135deg, rgba(94, 96, 206, 0.15), rgba(94, 96, 206, 0.05));
            border: 2px solid var(--accent-color);
        }
        
        .probability-circle span {
            font-size: 28px;
            font-weight: 700;
            color: var(--accent-color);
        }
        
        .reset-button {
            display: inline-block;
            padding: 12px 24px;
            background-color: transparent;
            color: var(--accent-color);
            border: 1px solid var(--accent-color);
            border-radius: 6px;
            font-size: 14px;
            font-weight: 500;
            margin-top: 16px;
            cursor: pointer;
            transition: all var(--transition-speed) ease;
        }
        
        .reset-button:hover {
            background-color: rgba(94, 96, 206, 0.05);
            transform: translateY(-2px);
        }
        
        /* Message de notification */
        .notification {
            padding: 15px;
            margin-bottom: 20px;
            border-radius: 6px;
            text-align: center;
            font-weight: 500;
            display: none;
        }
        
        .notification.success {
            background-color: rgba(25, 135, 84, 0.1);
            color: #198754;
            border: 1px solid rgba(25, 135, 84, 0.2);
        }
        
        .notification.error {
            background-color: rgba(220, 53, 69, 0.1);
            color: #dc3545;
            border: 1px solid rgba(220, 53, 69, 0.2);
        }

        /* Responsive styles */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 36px;
            }

            .hero p.tagline {
                font-size: 20px;
            }

            .hero .description {
                font-size: 16px;
                padding: 0 20px;
            }

            .steps {
                flex-direction: column;
                align-items: center;
            }

            .step {
                max-width: 400px;
            }
            
            .results-grid {
                flex-direction: column;
                align-items: center;
            }
            
            .result-card {
                width: 100%;
                max-width: 300px;
            }
        }

        @media (max-width: 480px) {
            .hero h1 {
                font-size: 28px;
            }

            .hero p.tagline {
                font-size: 18px;
            }

            .cta-button {
                padding: 12px 24px;
                font-size: 14px;
            }

            .prototype-form {
                padding: 30px 20px;
            }
            
            .probability-circle {
                width: 100px;
                height: 100px;
            }
            
            .probability-circle span {
                font-size: 24px;
            }
        }
    </style>
</head>
<body>
    <!-- En-tête de la page -->
    <header>
        <div class="container">
            <nav>
                <a href="#" class="logo">Syléa</a>
                <!-- Espace pour futur menu de navigation -->
            </nav>
        </div>
    </header>

    <!-- Section Hero -->
    <section class="hero">
        <div class="container">
            <h1>Syléa</h1>
            <p class="tagline">Votre trajectoire, éclairée par l'intelligence</p>
            <p class="description">
                Syléa est une intelligence artificielle qui vous aide à prendre les bonnes décisions pour atteindre vos objectifs de vie. Entrez un but, votre âge, votre situation, et découvrez en temps réel vos probabilités de réussite en fonction de vos choix.
            </p>
            <a href="#prototype" class="cta-button">Tester le prototype</a>
        </div>
    </section>

    <!-- Section Comment ça marche -->
    <section class="how-it-works">
        <div class="container">
            <h2 class="section-title">Comment ça marche</h2>
            <div class="steps">
                <!-- Étape 1 -->
                <div class="step">
                    <div class="step-icon">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
                        </svg>
                    </div>
                    <h3>Fixez un objectif</h3>
                    <p>Définissez clairement le but que vous souhaitez atteindre dans votre vie personnelle ou professionnelle.</p>
                </div>

                <!-- Étape 2 -->
                <div class="step">
                    <div class="step-icon">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7h12m0 0l-4-4m4 4l-4 4m0 6H4m0 0l4 4m-4-4l4-4" />
                        </svg>
                    </div>
                    <h3>Choisissez entre deux options</h3>
                    <p>Explorez différentes stratégies et alternatives pour atteindre votre objectif.</p>
                </div>

                <!-- Étape 3 -->
                <div class="step">
                    <div class="step-icon">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z" />
                        </svg>
                    </div>
                    <h3>Obtenez une estimation</h3>
                    <p>Découvrez vos chances de réussite basées sur l'analyse de données et l'intelligence artificielle.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Section Prototype (formulaire simple) -->
    <section id="prototype" class="prototype-section">
        <div class="container">
            <div class="prototype-form">
                <h2>Testez le prototype</h2>
                <!-- Notification de succès/erreur -->
                <div id="notification" class="notification"></div>
                
                <form id="sylea-form">
                    <div class="form-field">
                        <label for="email">Votre adresse email</label>
                        <input type="email" id="email" name="email" placeholder="exemple@domaine.com" required>
                    </div>
                    <div class="form-field">
                        <label for="goal">Votre objectif</label>
                        <input type="text" id="goal" name="goal" placeholder="Ex: Devenir entrepreneur, Acheter un logement..." required>
                    </div>
                    <div class="form-field">
                        <label for="age">Votre âge</label>
                        <input type="number" id="age" name="age" min="18" max="100" placeholder="Ex: 25" required>
                    </div>
                    <div class="form-field">
                        <label for="situation">Votre situation actuelle</label>
                        <select id="situation" name="situation" required>
                            <option value="" disabled selected>Choisissez une option</option>
                            <option value="etudiant">Étudiant</option>
                            <option value="salarie">Salarié</option>
                            <option value="entrepreneur">Entrepreneur</option>
                            <option value="recherche">En recherche d'emploi</option>
                            <option value="autre">Autre</option>
                        </select>
                    </div>
                    <div class="form-field">
                        <label for="option1">Option 1</label>
                        <input type="text" id="option1" name="option1" placeholder="Première option à comparer" required>
                    </div>
                    <div class="form-field">
                        <label for="option2">Option 2</label>
                        <input type="text" id="option2" name="option2" placeholder="Deuxième option à comparer" required>
                    </div>
                    <button type="submit" class="cta-button">Analyser mes chances</button>
                </form>
                
                <!-- Résultats (cachés par défaut) -->
                <div id="results" class="results-container" style="display: none;">
                    <h3>Probabilités de réussite</h3>
                    <div class="results-grid">
                        <div class="result-card">
                            <h4 id="result-option1-title">Option 1</h4>
                            <div class="probability-circle">
                                <span id="result-option1-percent">0%</span>
                            </div>
                        </div>
                        <div class="result-card">
                            <h4 id="result-option2-title">Option 2</h4>
                            <div class="probability-circle">
                                <span id="result-option2-percent">0%</span>
                            </div>
                        </div>
                    </div>
                    <button id="reset-button" class="reset-button">Analyser un autre choix</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Pied de page -->
    <footer>
        <div class="container">
            <p>© 2025 Syléa — Tous droits réservés</p>
        </div>
    </footer>
    <script>
        // Script pour la gestion du formulaire et l'affichage des résultats
        document.addEventListener('DOMContentLoaded', function() {
            // Éléments DOM
            const form = document.getElementById('sylea-form');
            const resultsContainer = document.getElementById('results');
            const resetButton = document.getElementById('reset-button');
            const option1TitleElement = document.getElementById('result-option1-title');
            const option2TitleElement = document.getElementById('result-option2-title');
            const option1PercentElement = document.getElementById('result-option1-percent');
            const option2PercentElement = document.getElementById('result-option2-percent');
            const notificationElement = document.getElementById('notification');
            
            // URL de l'API pour l'envoi des données (à remplacer par votre endpoint réel)
            const API_URL = 'https://api.sylea.fr/clients';
            
            // Fonction pour afficher une notification
            function showNotification(message, type) {
                notificationElement.textContent = message;
                notificationElement.className = 'notification ' + type;
                notificationElement.style.display = 'block';
                
                // Cacher la notification après 5 secondes
                setTimeout(() => {
                    notificationElement.style.display = 'none';
                }, 5000);
            }
            
            // Fonction pour envoyer les données à l'API
            async function sendDataToAPI(userData) {
                try {
                    // Version de l'API avec fetch (peut être adaptée selon vos besoins)
                    const response = await fetch(API_URL, {
                        method: 'POST',
                        headers: {
                            'Content-Type': 'application/json',
                        },
                        body: JSON.stringify(userData)
                    });
                    
                    // En cas d'erreur HTTP
                    if (!response.ok) {
                        throw new Error('Problème lors de l\'envoi des données');
                    }
                    
                    return await response.json();
                } catch (error) {
                    console.error('Erreur:', error);
                    
                    // Alternative : enregistrer dans le localStorage en cas d'échec
                    const storedData = JSON.parse(localStorage.getItem('sylea_users') || '[]');
                    storedData.push(userData);
                    localStorage.setItem('sylea_users', JSON.stringify(storedData));
                    
                    // En environnement de production, on pourrait implémenter une logique de réessai
                    return { stored: true, error: error.message };
                }
            }
            
            // Gérer la soumission du formulaire
            form.addEventListener('submit', async function(e) {
                e.preventDefault(); // Empêcher le rechargement de la page
                
                // Récupérer les valeurs du formulaire
                const email = document.getElementById('email').value;
                const goal = document.getElementById('goal').value;
                const age = document.getElementById('age').value;
                const situation = document.getElementById('situation').value;
                const option1 = document.getElementById('option1').value;
                const option2 = document.getElementById('option2').value;
                
                // Créer l'objet utilisateur
                const user = {
                    email: email,
                    goal: goal,
                    age: parseInt(age),
                    situation: situation,
                    option1: option1,
                    option2: option2,
                    submittedAt: new Date().toISOString()
                };
                
                // Envoyer les données à l'API
                try {
                    // Pour la démo, simulons l'API avec le localStorage
                    const storedData = JSON.parse(localStorage.getItem('sylea_users') || '[]');
                    storedData.push(user);
                    localStorage.setItem('sylea_users', JSON.stringify(storedData));
                    
                    // Dans un environnement réel, vous utiliseriez :
                    // await sendDataToAPI(user);
                    
                    console.log('Données utilisateur enregistrées avec succès:', user);
                    console.log('Liste complète des utilisateurs:', storedData);
                    
                    // Générer des pourcentages aléatoires (somme = 100%)
                    const option1Percent = Math.floor(Math.random() * 101); // 0-100
                    const option2Percent = 100 - option1Percent;
                    
                    // Mettre à jour les titres des options dans les résultats
                    option1TitleElement.textContent = option1;
                    option2TitleElement.textContent = option2;
                    
                    // Mettre à jour les pourcentages
                    option1PercentElement.textContent = option1Percent + '%';
                    option2PercentElement.textContent = option2Percent + '%';
                    
                    // Mettre en évidence l'option avec le pourcentage le plus élevé
                    if (option1Percent > option2Percent) {
                        document.querySelectorAll('.result-card')[0].style.borderLeft = '4px solid var(--accent-color)';
                        document.querySelectorAll('.result-card')[1].style.borderLeft = 'none';
                    } else if (option2Percent > option1Percent) {
                        document.querySelectorAll('.result-card')[1].style.borderLeft = '4px solid var(--accent-color)';
                        document.querySelectorAll('.result-card')[0].style.borderLeft = 'none';
                    } else {
                        // Égalité
                        document.querySelectorAll('.result-card')[0].style.borderLeft = '4px solid #aaa';
                        document.querySelectorAll('.result-card')[1].style.borderLeft = '4px solid #aaa';
                    }
                    
                    // Cacher le formulaire et afficher les résultats
                    form.style.display = 'none';
                    resultsContainer.style.display = 'block';
                    
                    // Faire défiler jusqu'aux résultats si nécessaire
                    resultsContainer.scrollIntoView({ behavior: 'smooth' });
                    
                } catch (error) {
                    console.error('Erreur lors de l\'enregistrement des données:', error);
                    showNotification('Une erreur est survenue. Veuillez réessayer plus tard.', 'error');
                }
            });
            
            // Gérer le bouton de réinitialisation
            resetButton.addEventListener('click', function() {
                // Cacher les résultats et afficher le formulaire
                resultsContainer.style.display = 'none';
                form.style.display = 'block';
                
                // Faire défiler jusqu'au formulaire
                form.scrollIntoView({ behavior: 'smooth' });
            });

            // Fonction pour exporter les données (pour admin)
            function exportData() {
                const data = localStorage.getItem('sylea_users');
                if (data) {
                    const blob = new Blob([data], { type: 'application/json' });
                    const url = URL.createObjectURL(blob);
                    const a = document.createElement('a');
                    a.href = url;
                    a.download = 'sylea_users_' + new Date().toISOString().slice(0, 10) + '.json';
                    document.body.appendChild(a);
                    a.click();
                    document.body.removeChild(a);
                }
            }
            
            // Pour debugging et accès administrateur - accessible via la console du navigateur
            window.syleavlaa = {
                exportData: exportData,
                getAllUsers: () => JSON.parse(localStorage.getItem('sylea_users') || '[]'),
                clearData: () => {
                    if (confirm('Êtes-vous sûr de vouloir supprimer toutes les données ?')) {
                        localStorage.removeItem('sylea_users');
                        alert('Données supprimées');
                    }
                }
            };
        });
    </script>
</body>
</html>
