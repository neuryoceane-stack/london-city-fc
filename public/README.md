# Dossier Public

Ce dossier contient tous les fichiers statiques accessibles directement via l'URL.

## 📁 Structure

### `/logo/`
Déposez le logo du club ici.

**Formats recommandés :**
- **SVG** (préféré) - Vectoriel, scalable, léger
- **PNG** - Avec fond transparent pour une meilleure intégration

**Utilisation dans le code :**
```astro
<img src="/logo/logo.svg" alt="London City FC Logo" />
```

### `/images/`
Déposez toutes les autres images du site ici (photos d'équipe, stade, événements, etc.).

**Organisation suggérée :**
- `/images/hero/` - Images pour les sections hero
- `/images/team/` - Photos de l'équipe
- `/images/stadium/` - Photos du stade
- `/images/events/` - Photos d'événements

**Utilisation dans le code :**
```astro
<img src="/images/hero/stadium.jpg" alt="Stade London City" />
```

## 📝 Notes

- Tous les fichiers dans `public/` sont servis à la racine de l'URL
- Exemple : `public/logo/logo.svg` → accessible via `/logo/logo.svg`
- Les images sont optimisées automatiquement par Astro lors du build
- Utilisez des noms de fichiers descriptifs et en minuscules avec tirets (ex: `logo-club.svg`)
