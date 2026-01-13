# 🔍 Vérifier votre Token GitHub

L'erreur 403 signifie que le token n'a pas les bonnes permissions. Vérifiez :

## 1. Vérifier les permissions du token

1. Allez sur GitHub → **Settings** → **Developer settings** → **Personal access tokens** → **Tokens (classic)**
2. Trouvez votre token `Vercel Deploy`
3. Vérifiez qu'il a bien la permission **`repo`** cochée
   - Si ce n'est pas le cas, supprimez-le et créez-en un nouveau avec **`repo`** coché

## 2. Vérifier que le dépôt existe

Allez sur : `https://github.com/neuryoceane-stack/london-city-fc`

- Si le dépôt n'existe pas, créez-le d'abord sur GitHub
- Si le dépôt existe mais est vide, c'est normal, on va le remplir

## 3. Méthode alternative : Utiliser le token manuellement

Une fois que vous avez vérifié les permissions, essayez cette commande dans le terminal :

```bash
cd "/Users/oceaneneury/Desktop/Cursor/Projet 5 London FC Foot"
git push -u origin main
```

Quand il demande :
- **Username** : `neuryoceane-stack`
- **Password** : Collez votre token (celui qui commence par `github_pat_...`)

## 4. Ou utiliser GitHub Desktop (Plus simple)

Si le token ne fonctionne pas, utilisez GitHub Desktop :
1. Ouvrez GitHub Desktop
2. File → Add Local Repository
3. Sélectionnez votre dossier
4. Publish repository
