# 📤 Instructions pour Pousser le Code sur GitHub

## Option 1 : Push avec authentification HTTPS (Recommandé)

Exécutez cette commande dans votre terminal :

```bash
cd "/Users/oceaneneury/Desktop/Cursor/Projet 5 London FC Foot"
git push -u origin main
```

GitHub vous demandera :
- **Username** : `neuryoceane-stack`
- **Password** : Utilisez un **Personal Access Token** (PAS votre mot de passe GitHub)

### Créer un Personal Access Token :

1. Allez sur GitHub → **Settings** → **Developer settings** → **Personal access tokens** → **Tokens (classic)**
2. Cliquez sur **"Generate new token"** → **"Generate new token (classic)"**
3. Donnez-lui un nom : `Vercel Deploy`
4. Cochez la case **`repo`** (accès complet aux dépôts)
5. Cliquez sur **"Generate token"**
6. **⚠️ IMPORTANT** : Copiez le token immédiatement (vous ne pourrez plus le voir après)
7. Utilisez ce token comme mot de passe lors du `git push`

---

## Option 2 : Utiliser GitHub Desktop (Plus Simple)

1. Téléchargez [GitHub Desktop](https://desktop.github.com/)
2. Connectez-vous avec votre compte GitHub
3. Cliquez sur **"File"** → **"Add Local Repository"**
4. Sélectionnez le dossier : `/Users/oceaneneury/Desktop/Cursor/Projet 5 London FC Foot`
5. Cliquez sur **"Publish repository"** en haut
6. Cochez **"Keep this code private"** si vous voulez (optionnel)
7. Cliquez sur **"Publish repository"**

---

## Option 3 : Utiliser SSH (Pour les utilisateurs avancés)

Si vous avez configuré SSH avec GitHub, vous pouvez utiliser :

```bash
git remote set-url origin git@github.com:neuryoceane-stack/london-city-fc.git
git push -u origin main
```

---

## ✅ Vérifier que ça a fonctionné

Une fois le push réussi, allez sur :
`https://github.com/neuryoceane-stack/london-city-fc`

Vous devriez voir tous vos fichiers !

---

## 🚀 Ensuite : Déployer sur Vercel

1. Allez sur [vercel.com](https://vercel.com)
2. Connectez-vous avec GitHub
3. Cliquez sur **"Add New..."** → **"Project"**
4. Sélectionnez `london-city-fc`
5. Cliquez sur **"Import"** puis **"Deploy"**
