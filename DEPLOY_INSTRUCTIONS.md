# 🚀 Instructions pour Déployer sur Vercel

Votre projet est maintenant prêt à être poussé sur GitHub. Suivez ces étapes :

## Étape 1 : Créer un dépôt sur GitHub

1. Allez sur [github.com](https://github.com) et connectez-vous
2. Cliquez sur le bouton **"+"** en haut à droite → **"New repository"**
3. Nommez-le : `london-city-fc` (ou un autre nom de votre choix)
4. Choisissez **"Public"** ou **"Private"**
5. **⚠️ IMPORTANT : Ne cochez PAS "Initialize with README"**
6. Cliquez sur **"Create repository"**

## Étape 2 : Connecter votre dépôt local à GitHub

Une fois le dépôt créé, GitHub vous donnera des instructions. Exécutez ces commandes dans votre terminal (remplacez `VOTRE_USERNAME` par votre nom d'utilisateur GitHub) :

```bash
cd "/Users/oceaneneury/Desktop/Cursor/Projet 5 London FC Foot"

git remote add origin https://github.com/VOTRE_USERNAME/london-city-fc.git

git push -u origin main
```

**Exemple** : Si votre nom d'utilisateur est `john`, la commande serait :
```bash
git remote add origin https://github.com/john/london-city-fc.git
```

## Étape 3 : Déployer sur Vercel

1. Allez sur [vercel.com](https://vercel.com)
2. Cliquez sur **"Sign Up"** ou **"Log In"**
3. Choisissez **"Continue with GitHub"** pour connecter votre compte
4. Autorisez Vercel à accéder à GitHub
5. Cliquez sur **"Add New..."** → **"Project"**
6. Vous verrez la liste de vos dépôts GitHub
7. Trouvez `london-city-fc` et cliquez sur **"Import"**
8. Vérifiez les paramètres :
   - **Framework Preset** : Astro (devrait être détecté automatiquement)
   - **Root Directory** : `./` (laissez vide)
   - **Build Command** : `npm run build`
   - **Output Directory** : `dist`
   - **Install Command** : `npm install`
9. Cliquez sur **"Deploy"**
10. Attendez 1-2 minutes
11. **Copiez le lien** fourni (ex: `https://london-city-fc-xxxxx.vercel.app`)

## ✅ C'est fait !

Votre site sera en ligne et accessible partout dans le monde !

---

## 🔄 Mises à jour futures

Chaque fois que vous modifiez le code et que vous faites :
```bash
git add .
git commit -m "Votre message"
git push
```

Vercel redéploiera automatiquement votre site ! ✨

---

## 🆘 Si vous avez des problèmes

### Erreur : "repository does not contain the requested branch"
- Vérifiez que vous avez bien poussé le code avec `git push -u origin main`
- Vérifiez que la branche s'appelle bien `main` (pas `master`)

### Erreur : "repository is empty"
- Vérifiez que tous les fichiers sont bien commités
- Vérifiez que vous avez bien fait `git push`

### Le build échoue
- Vérifiez que `npm run build` fonctionne localement
- Vérifiez les logs de déploiement sur Vercel
