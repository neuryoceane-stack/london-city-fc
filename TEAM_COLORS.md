# Couleurs officielles - London Albion City FC

Palette utilisée sur le site pour les textes, titres et éléments d’interface.

| Nom     | Hex       | Usage principal                    |
|---------|-----------|------------------------------------|
| Bleu marine | `#082340` | Titres, texte principal, fonds sombres |
| Rouge   | `#d01925` | Accents, liens, boutons, soulignés |
| Marron  | `#9c7647` | Détails, dégradés                  |
| Beige   | `#fef6ce` | Fonds, sections hero, hover       |

## Variables CSS (dans `BaseLayout.astro`)

- `--team-navy`  → #082340  
- `--team-red`   → #d01925  
- `--team-brown` → #9c7647  
- `--team-beige` → #fef6ce  

Tout le corps de texte (paragraphes, contenu des sections) utilise le bleu marine (`--text-primary` et `--text-secondary` = `--team-navy`). Accents et boutons en rouge, dégradés avec marron/beige.
