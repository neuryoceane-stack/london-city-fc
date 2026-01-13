# 🚀 Guide Rapide - Déployer sur Vercel en 5 minutes

## Étape 1 : Créer un compte GitHub (2 min)
1. Allez sur [github.com/signup](https://github.com/signup)
2. Créez un compte gratuit

## Étape 2 : Créer un dépôt GitHub (1 min)
1. Cliquez sur le "+" en haut à droite → "New repository"
2. Nom : `london-city-fc`
3. Choisissez "Public"
4. **Ne cochez PAS** "Initialize with README"
5. Cliquez "Create repository"

## Étape 3 : Pousser votre code (2 min)

Ouvrez le terminal dans ce dossier et tapez :

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/VOTRE_USERNAME/london-city-fc.git
git push -u origin main
```

⚠️ **Remplacez `VOTRE_USERNAME` par votre vrai nom d'utilisateur GitHub !**

## Étape 4 : Déployer sur Vercel (2 min)
1. Allez sur [vercel.com/signup](https://vercel.com/signup)
2. Cliquez "Continue with GitHub"
3. Autorisez Vercel à accéder à GitHub
4. Cliquez "Add New..." → "Project"
5. Sélectionnez `london-city-fc`
6. Cliquez "Deploy"
7. Attendez 1-2 minutes
8. **Copiez le lien** (ex: `https://london-city-fc-xxxxx.vercel.app`)

## 🎉 Partagez le lien avec ton copain !

Le site sera en ligne et accessible partout dans le monde !

---

## 💡 Astuce
Chaque fois que tu modifies le code et que tu fais `git push`, Vercel redéploie automatiquement le site !
