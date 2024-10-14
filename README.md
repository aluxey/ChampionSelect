# League of Legends Champion Selector

**League of Legends Champion Selector** est un outil conçu pour aider les joueurs à sélectionner le bon champion lors de la phase de sélection, en prenant en compte plusieurs facteurs clés tels que le rôle joué, la composition de l'équipe, les synergies et les contres des champions ennemis.

## Fonctionnalités

* Système de recommandation de champions : Recommande les champions en fonction du rôle choisi (Top, Jungle, Mid, ADC, Support), de la synergie avec les autres membres de l'équipe et des contre-picks pour affronter les champions ennemis.

* Filtres de champions : Permet de filtrer les champions en fonction de leurs attributs tels que leur type (tank, mage, assassin, etc.), leur difficulté ou leur style de jeu.

* Mises à jour de la méta : Intègre des mises à jour régulières en fonction des patchs actuels du jeu, prenant en compte les buffs, nerfs, et autres changements.

* Analyse des données : Utilise des données sur les taux de victoire, de sélection et de bannissement pour recommander les meilleurs choix en partie classée.

* Préférences utilisateurs : Les utilisateurs peuvent sauvegarder leurs champions préférés ou fréquemment utilisés pour des suggestions personnalisées.

## Plan de Développement
1. Collecte de données

    Données des champions : Toutes les informations sur les champions (rôles, capacités, forces et faiblesses) seront récupérées grâce à l'API officielle de Riot Games.
    Méta actuelle : Les statistiques de performance (taux de victoire, sélection, etc.) seront extraites via des sites tels que OP.GG ou U.GG, ou directement via l'API Riot.

2. Stack Technique

    Frontend : React pour une interface utilisateur réactive et moderne.
    Backend : Node.js avec Express.js ou Flask en Python pour gérer les interactions avec l'API Riot et le traitement des données.
    Base de données : MongoDB ou Firebase pour stocker les données utilisateurs et champion.
    API : Intégration avec l'API Riot Games pour récupérer les données en temps réel.

3. Fonctions principales

    Filtrage des champions : Filtrer les champions selon leur rôle, type, et niveau de difficulté.
    Algorithme de recommandation :
        Synergie : Recommandation de champions qui se combinent bien avec ceux de l'équipe.
        Contre-picks : Suggestions de champions qui contrent ceux de l'équipe ennemie.
        Pertinence dans la méta : Recommandation des champions les plus performants du patch actuel en fonction de leur taux de victoire.

4. Interface Utilisateur

    Sélection simple avec des menus déroulants pour choisir un rôle (Top, Jungle, Mid, ADC, Support) et des listes de champions avec des images pour faciliter le choix.
    Vue détaillée des champions : Statistiques clés et conseils de contre.
    Composition d'équipe : Affiche la synergie et les contre-picks dans un panneau de suggestions.

5. Fonctionnalités avancées (optionnelles)

    Liste de tiers : Mise à jour dynamique d'une liste de tiers selon les statistiques de la méta.
    Analyse des matchups : Détails et conseils sur les matchups pour chaque rôle.
    Statistiques personnelles : Suivi de la performance utilisateur avec différents champions et suggestions d'améliorations.

6. Déploiement

    Frontend : Hébergé sur Vercel.
    Backend : Hébergé sur Heroku ou AWS.

## Installation

Clonez ce repository :

```bash
git clone https://github.com/ton-utilisateur/lol-champ-selector.git
```

Installez les dépendances du frontend et backend :

```bash
cd frontend && npm install
cd ../backend && npm install
```

Configurez votre clé API Riot Games dans un fichier .env :

```makefile
RIOT_API_KEY=your_api_key_here
```

Démarrez l'application :

```bash
npm run start
```

## Utilisation

Une fois l'application lancée, sélectionnez votre rôle, filtrez les champions selon vos préférences, et laissez l'algorithme vous recommander les champions les plus adaptés en fonction de la composition de votre équipe et des adversaires.