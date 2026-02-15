# London Albion City Football Club - Site Web (Astro)

Site web officiel du London Albion City Football Club, un nouveau projet de football basé à Londres avec une vision à long terme.

## 🚀 Technologies

Ce site est construit avec **[Astro](https://astro.build)**, un framework moderne pour créer des sites web rapides et performants.

## 🎨 Palette de Couleurs

Le site utilise une palette de bleus soigneusement sélectionnée :

- **Dark Navy Blue** (`#02346A`) - Bordures externes et texte principal
- **Primary Blue** (`#238AD2`) - Éléments principaux et cercles internes
- **Light Blue** (`#9ECBE8`) - Fond interne, eau et skyline
- **Steel Blue** (`#426186`) - Ombres et détails
- **Soft Blue** (`#719EC0`) - Gradients et support
- **White** (`#FFFFFF`) - Fond principal

## 📁 Structure du Projet

```
Projet 5 London FC Foot/
├── public/                 # Fichiers statiques (images, favicon, etc.)
├── src/
│   ├── components/        # Composants Astro réutilisables
│   │   ├── Navigation.astro
│   │   └── Footer.astro
│   ├── layouts/           # Layouts de base
│   │   └── BaseLayout.astro
│   └── pages/             # Pages du site (routing automatique)
│       ├── index.astro    # Page d'accueil (/)
│       └── the-club.astro  # Page The Club (/the-club)
├── astro.config.mjs       # Configuration Astro
├── package.json           # Dépendances et scripts
└── README.md             # Documentation
```

## 🛠️ Installation

1. **Installer les dépendances** :
```bash
npm install
```

2. **Lancer le serveur de développement** :
```bash
npm run dev
```

Le site sera accessible sur `http://localhost:4321` (port par défaut d'Astro).

3. **Build pour la production** :
```bash
npm run build
```

4. **Prévisualiser le build de production** :
```bash
npm run preview
```

## 📄 Pages

### Home (`/`)
Contient les sections :
- Intro
- Who we are
- Our idea

### The Club (`/the-club`)
Contient les sections :
- What we are building
- Long-term ambition

## 🎯 Fonctionnalités

### Navigation
- Menu de navigation responsive avec animation
- Menu hamburger pour mobile
- Mise en évidence de la page active
- Effet de scroll sur la navbar

### Design
- Design moderne et épuré
- Animations fluides et discrètes
- Responsive design (mobile, tablette, desktop)
- Gradients et effets visuels subtils
- Typographie optimisée pour la lisibilité

### Performance
- Astro génère du HTML statique par défaut
- JavaScript minimal (seulement pour les interactions)
- CSS optimisé et scoped
- Chargement rapide

### Accessibilité
- Support du mode réduit de mouvement (prefers-reduced-motion)
- Navigation au clavier
- Attributs ARIA appropriés
- Contraste de couleurs respecté

## 📱 Responsive Design

Le site est entièrement responsive et s'adapte à :
- **Mobile** : < 768px
- **Tablette** : 768px - 1024px
- **Desktop** : > 1024px

## 🔧 Personnalisation

### Modifier les couleurs

Les couleurs sont définies dans `src/layouts/BaseLayout.astro` dans la section `:root` :

```css
:root {
  --dark-navy: #02346A;
  --primary-blue: #238AD2;
  /* ... */
}
```

### Ajouter une nouvelle page

Créez un nouveau fichier `.astro` dans `src/pages/`. Astro générera automatiquement la route.

Exemple : `src/pages/about.astro` → `/about`

## 📝 Bonnes Pratiques Implémentées

- ✅ Code propre et maintenable
- ✅ Structure modulaire avec composants Astro
- ✅ CSS organisé avec variables
- ✅ JavaScript minimal et optimisé
- ✅ Performance optimisée (HTML statique)
- ✅ Accessibilité respectée
- ✅ Responsive design
- ✅ Animations fluides
- ✅ Pas de fallback masquant les erreurs

## 🚀 Déploiement

Le site peut être déployé sur n'importe quelle plateforme supportant les sites statiques :

- **Vercel** : `vercel deploy`
- **Netlify** : `netlify deploy`
- **GitHub Pages** : Après build, déployer le dossier `dist/`
- **Cloudflare Pages** : Connecter le repo GitHub

## 📞 Contact

Pour toute question ou suggestion concernant le site, contactez l'équipe du London Albion City FC.

---

© 2024 London Albion City Football Club. Tous droits réservés.
