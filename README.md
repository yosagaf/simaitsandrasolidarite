# Sima Itsandra Solidarité — Landing page

Site statique pour l'association **Sima Itsandra Solidarité** (humanitaire & caritative).
Aucun build, aucun framework : HTML + CSS + JS natif.

## Structure

```
simaitsandrasolidarite/
├── index.html              # page d'accueil
├── site.webmanifest        # manifest PWA (icônes + theme color)
├── robots.txt
├── _headers                # en-têtes sécurité + cache (Cloudflare Pages)
├── .gitignore
└── assets/
    ├── css/styles.css
    ├── js/script.js
    ├── images/
    │   └── logo.png        # logo principal
    └── icons/              # favicons
        ├── favicon.ico
        ├── favicon-16.png
        ├── favicon-32.png
        ├── favicon-192.png
        ├── favicon-512.png
        └── apple-touch-icon.png
```

## Développement local

```bash
# Option 1 — Python
python3 -m http.server 8080

# Option 2 — Node
npx serve .
```

→ http://localhost:8080

## Déploiement — Cloudflare Pages

1. Pousser ce dossier dans un dépôt GitHub (repo root = `simaitsandrasolidarite/`).
2. Sur Cloudflare → **Pages** → **Create a project** → connecter le dépôt.
3. Paramètres de build :
   - **Framework preset** : `None`
   - **Build command** : *(vide)*
   - **Build output directory** : `/`
4. Chaque `git push` redéploie automatiquement.

Si tu pousses tout le workspace `sis/` (avec `docs/` à côté), règle alors :
- **Build output directory** : `simaitsandrasolidarite`

## Branding

| Usage | Hex |
| --- | --- |
| Bleu solidarité (primaire) | `#003B7A` |
| Vert espoir (secondaire) | `#2E7D32` |
| Or humanitaire (accent) | `#E2A316` |
| Bleu nuit (texte) | `#0B2F5B` |

Typographie : **Montserrat** (Google Fonts — 400/500/600/700/800).

## Liens externes

- Dons / adhésions HelloAsso :
  <https://www.helloasso.com/associations/sima-itsandra-solidarite/formulaires/1>
