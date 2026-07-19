# LA SUNSHINES — Site (édition Candy Land)

Site statique (HTML/CSS/JS, aucune dépendance) prêt à héberger sur Vercel.

## Contenu
- `index.html` — la page
- `assets/logo-sunshines.png`, `assets/logo-themouv.png` — les logos
- `vercel.json` — config minimale (URLs propres)

## Déployer sur Vercel

**Option 1 — le plus simple (sans compte Git) :**
1. Va sur https://vercel.com/new
2. Glisse-dépose le dossier `site` (ce dossier) dans la zone d'upload
3. Vercel détecte automatiquement un projet statique → clique "Deploy"
4. Ton site est en ligne en ~30 secondes, avec une URL du type `la-sunshines.vercel.app`

**Option 2 — avec la CLI Vercel :**
```bash
npm i -g vercel
cd site
vercel --prod
```

**Option 3 — via GitHub :**
1. Crée un repo GitHub, pousse ce dossier dedans
2. Sur vercel.com → "Add New Project" → importe le repo
3. Aucune configuration à changer (framework: "Other" / statique), clique "Deploy"

## Nom de domaine personnalisé
Une fois déployé, dans le dashboard Vercel du projet : **Settings → Domains** → ajoute ton propre domaine (ex. `lasunshines.gp` ou `lasunshines.fr`) et suis les instructions DNS.

## Mettre à jour la date / l'édition
Tout est dans `index.html` :
- Le compte à rebours cible la ligne `const target = new Date("2026-07-31T16:00:00-04:00")`
- Le lien billetterie Bizouk apparaît 3 fois (nav, carte édition, CTA final)
- Le texte de l'Article 9 / CGV est dans la section `#regles`
