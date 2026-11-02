# Portfolio — Léa Bossuat

Portfolio personnel conçu comme un **système solaire interactif** : chaque planète en orbite ouvre une fenêtre d'informations sur un aspect
de ma vie et de mon parcours.

---

## Concept

La navigation se fait par un système solaire cliquable :

| Astre | Contenu |
|---|---|
| 🪐 Mercure | Présentation |
| 🪐 Vénus | Skills |
| 🪐 Terre & Lune | Parcours |
| 🪐 Mars | Expérience professionnel |
| 🪐 Jupiter | Projets |
| 🪐 Saturne | Centres d'intérêt |
| 🪐 Uranus | CV |
| 🪐 Neptune | Futur |
| 🪐 Pluton | Contact |

## Côtés technique 

- **HTML et CSS strictement séparés** — aucun style en ligne, aucun framework CSS.
- **Responsive** : disposition verticale sur téléphone comme sur ordinateur, s'adapte (en partie).

## Côtés technique à pousser

- **Utiliser des frameworks** — Peut permettre de simplifier l'écriture, et d'aller plus vite.
- **Changer la disposition** : Pouvoir avoir des cartes plus grande sur ordinateur, permettant de changer la disposition des objets à l'interieur.

## Structure du projet

```
.
├── home-page.html          # Structure de la page
├── home-page.css           # Stylisation de la page
├── CV_epitech.pdf          # CV à ouvrir avec le lien dans le HTML
└── .github/
    └── workflows/
        └── deploy.yml      # Déploiement automatique sur GitHub Pages
```

## Lancer le projet en local

Aucune installation, aucune dépendance : il suffit d'ouvrir `home-page.html`
dans un navigateur (double-clic, ou clic droit → Ouvrir avec).

## Déploiement

Le site est publié sur **GitHub Pages** via **GitHub Actions**.
À chaque `push` sur la branche `main`, le workflow `.github/workflows/deploy.yml` :

1. récupère le code du dépôt;
2. construit un dossier `_site` dans lequel `home-page.html` est copié sous le nom
   `index.html` (nom imposé par GitHub Pages) avec le CSS;
3. publie ce dossier sur GitHub Pages.

Le déploiement peut aussi être déclenché manuellement depuis l'onglet **Actions** du dépôt.

> ⚙️ Prérequis côté dépôt : *Settings → Pages → Source → GitHub Actions*.
