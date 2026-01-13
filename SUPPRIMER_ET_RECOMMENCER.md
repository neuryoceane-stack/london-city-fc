# 🗑️ Supprimer et Recommencer le Dépôt GitHub

## Étape 1 : Supprimer le dépôt sur GitHub

1. Allez sur votre dépôt : `https://github.com/neuryoceane-stack/london-city-fc`
2. Cliquez sur **"Settings"** (en haut à droite du dépôt)
3. Faites défiler jusqu'en bas de la page
4. Dans la section **"Danger Zone"**, cliquez sur **"Delete this repository"**
5. Tapez `neuryoceane-stack/london-city-fc` pour confirmer
6. Cliquez sur **"I understand the consequences, delete this repository"**

⚠️ **Attention** : Cette action est irréversible !

## Étape 2 : Nettoyer la connexion Git locale

Une fois le dépôt supprimé sur GitHub, nettoyez votre dépôt local :

```bash
cd "/Users/oceaneneury/Desktop/Cursor/Projet 5 London FC Foot"

# Supprimer l'ancienne connexion
git remote remove origin

# Vérifier que c'est bien supprimé
git remote -v
```

## Étape 3 : Recréer un nouveau dépôt sur GitHub

1. Allez sur [github.com](https://github.com)
2. Cliquez sur **"+"** → **"New repository"**
3. Nommez-le : `london-city-fc` (ou un autre nom)
4. Choisissez **"Public"** ou **"Private"**
5. **⚠️ IMPORTANT : Ne cochez PAS "Initialize with README"**
6. Cliquez sur **"Create repository"**

## Étape 4 : Connecter votre code au nouveau dépôt

```bash
cd "/Users/oceaneneury/Desktop/Cursor/Projet 5 London FC Foot"

# Ajouter le nouveau dépôt distant
git remote add origin https://github.com/neuryoceane-stack/london-city-fc.git

# Pousser le code
git push -u origin main
```

## Étape 5 : Redéployer sur Vercel

1. Allez sur [vercel.com](https://vercel.com)
2. Si le projet existe déjà sur Vercel, supprimez-le d'abord :
   - Allez dans les paramètres du projet
   - Cliquez sur **"Delete Project"**
3. Créez un nouveau projet :
   - Cliquez sur **"Add New..."** → **"Project"**
   - Sélectionnez `london-city-fc`
   - Cliquez sur **"Import"**
   - Vérifiez les paramètres (Astro devrait être détecté)
   - Cliquez sur **"Deploy"**

---

## ✅ Alternative : Garder le même dépôt mais le vider

Si vous préférez garder le même nom de dépôt, vous pouvez :

1. Supprimer tous les fichiers du dépôt sur GitHub
2. Pousser votre nouveau code

Mais il est plus simple de supprimer et recréer !
