# 🚀 Guide de Déploiement sur Vercel

Ce guide vous explique comment déployer votre site London City FC sur Vercel pour le partager avec votre copain.

## 📋 Prérequis

- Un compte GitHub (gratuit) - [Créer un compte](https://github.com/signup)
- Un compte Vercel (gratuit) - [Créer un compte](https://vercel.com/signup)

---

## 🎯 Méthode 1 : Déploiement via l'Interface Web (RECOMMANDÉ - Plus Simple)

### Étape 1 : Créer un dépôt GitHub

1. **Créer un nouveau dépôt sur GitHub** :
   - Allez sur [github.com](https://github.com)
   - Cliquez sur le bouton "+" en haut à droite → "New repository"
   - Nommez-le : `london-city-fc` (ou un autre nom)
   - Choisissez "Public" ou "Private"
   - **Ne cochez PAS** "Initialize with README"
   - Cliquez sur "Create repository"

2. **Pousser votre code sur GitHub** :
   
   Ouvrez votre terminal dans le dossier du projet et exécutez :

   ```bash
   # Initialiser Git (si pas déjà fait)
   git init
   
   # Ajouter tous les fichiers
   git add .
   
   # Créer le premier commit
   git commit -m "Initial commit - London City FC website"
   
   # Ajouter le dépôt distant (remplacez VOTRE_USERNAME par votre nom d'utilisateur GitHub)
   git remote add origin https://github.com/VOTRE_USERNAME/london-city-fc.git
   
   # Pousser le code
   git branch -M main
   git push -u origin main
   ```

### Étape 2 : Déployer sur Vercel

1. **Se connecter à Vercel** :
   - Allez sur [vercel.com](https://vercel.com)
   - Cliquez sur "Sign Up" ou "Log In"
   - Choisissez "Continue with GitHub" pour connecter votre compte GitHub

2. **Importer le projet** :
   - Une fois connecté, cliquez sur "Add New..." → "Project"
   - Vous verrez la liste de vos dépôts GitHub
   - Trouvez `london-city-fc` et cliquez sur "Import"

3. **Configurer le projet** :
   - **Framework Preset** : Vercel devrait détecter automatiquement "Astro"
   - **Root Directory** : Laissez vide (ou `./` si demandé)
   - **Build Command** : `npm run build` (devrait être pré-rempli)
   - **Output Directory** : `dist` (devrait être pré-rempli)
   - **Install Command** : `npm install` (devrait être pré-rempli)

4. **Déployer** :
   - Cliquez sur "Deploy"
   - Attendez 1-2 minutes pendant le déploiement
   - Une fois terminé, vous obtiendrez un lien comme : `https://london-city-fc-xxxxx.vercel.app`

5. **Partager le lien** :
   - Copiez le lien fourni par Vercel
   - Partagez-le avec votre copain ! 🎉

---

## 🛠️ Méthode 2 : Déploiement via CLI (Pour les plus techniques)

### Étape 1 : Installer Vercel CLI

```bash
npm install -g vercel
```

### Étape 2 : Se connecter

```bash
vercel login
```

### Étape 3 : Déployer

Dans le dossier de votre projet :

```bash
vercel
```

Suivez les instructions à l'écran. Vercel détectera automatiquement Astro.

### Étape 4 : Déployer en production

```bash
vercel --prod
```

---

## 🔄 Mises à jour automatiques

Une fois connecté à GitHub, **chaque fois que vous poussez du code sur GitHub**, Vercel redéploiera automatiquement votre site ! C'est magique ✨

---

## 🌐 Personnaliser le nom de domaine

Vercel vous donne un nom de domaine gratuit comme `london-city-fc-xxxxx.vercel.app`.

Vous pouvez aussi :
- **Changer le nom** : Dans les paramètres du projet sur Vercel, vous pouvez modifier le nom
- **Ajouter un domaine personnalisé** : Si vous avez un domaine, vous pouvez l'ajouter dans les paramètres

---

## 📝 Notes importantes

- ✅ Vercel est **100% gratuit** pour les projets personnels
- ✅ Le site sera **rapide** et **sécurisé** (HTTPS automatique)
- ✅ Les **images et fichiers** dans `public/` seront automatiquement servis
- ✅ Chaque déploiement crée une **nouvelle version** (vous pouvez revenir en arrière si besoin)

---

## 🆘 En cas de problème

Si le déploiement échoue :

1. Vérifiez que `npm run build` fonctionne localement :
   ```bash
   npm run build
   ```

2. Vérifiez les logs de déploiement sur Vercel (onglet "Deployments")

3. Assurez-vous que tous les fichiers sont bien dans le dépôt GitHub

---

## 🎉 C'est tout !

Une fois déployé, vous aurez un lien permanent que vous pourrez partager avec n'importe qui, n'importe où dans le monde !
