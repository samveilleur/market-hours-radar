# 🚀 Déploiement gratuit — Market Hours Radar (sans carte bancaire)

Ce dossier (`market-radar-deploy/`) contient tous les fichiers prêts à être uploadés sur un hébergeur statique gratuit.

## Fichiers présents (10)

| Fichier | Rôle |
|---------|------|
| `index.html` | Page principale |
| `styles.css` | Thème sombre, mise en page |
| `app.js` | Rendu, interactions, dé-pin sur survol |
| `time.js` | Moteur horaire, 12 places |
| `data.json` | Volumes réels (ETF Yahoo Finance) |
| `manifest.json` | PWA (installable sur Android) |
| `sw.js` | Service Worker (hors-ligne partiel) |
| `pwa-icon-192.png` | Icône PWA |
| `pwa-icon-512.png` | Icône PWA |
| `privacy.html` | Politique de confidentialité |

---

## Option 1 — GitHub Pages (recommandé, 100 % gratuit, pas de CB)

### Étape 1 — Créer le dépôt
1. Va sur https://github.com et connecte-toi (crée un compte si besoin, gratuit).
2. Clique sur **"New repository"**.
3. Nom du dépôt : `market-hours-radar`
4. Coche **"Public"**.
5. Ne coche pas "Add a README" (on va uploader les fichiers directement).
6. Clique sur "Create repository".

### Étape 2 — Uploader les fichiers
1. Dans ton dépôt, clique sur **"uploading an existing file"**.
2. Glisse-dépose **tous les fichiers** du dossier `C:\Users\bento\Desktop\market-radar-deploy\`.
3. En bas, écris un message de commit (ex: "Déploiement initial") et clique sur "Commit changes".

### Étape 3 — Activer GitHub Pages
1. Dans ton dépôt, va dans **Settings** → **Pages** (menu de gauche).
2. Sous "Build and deployment" → **Source**, sélectionne **Deploy from a branch**.
3. Branch : `main` (ou `master`), dossier : `/ (root)`.
4. Clique sur **Save**.
5. Attends 1 à 2 minutes. GitHub donne une URL du type `https://ton-utilisateur.github.io/market-hours-radar/`.

---

## Option 2 — Vercel (gratuit pour hobby, pas de CB)

1. Va sur https://vercel.com et connecte-toi (compte GitHub, Google ou email, gratuit).
2. Clique sur **"Add New"** → **"Project"**.
3. Importe le dépôt GitHub `market-hours-radar` (ou uploade directement le dossier via le dashboard).
4. Framework : "Other" ou laisse par défaut.
5. Build command : laisser vide.
6. Output directory : `.` (la racine).
7. Clique sur "Deploy".
8. Vercel donne une URL du type `https://market-hours-radar-xxx.vercel.app`.

---

## Option 3 — Cloudflare Pages (gratuit, pas de CB)

1. Va sur https://pages.cloudflare.com et connecte-toi (compte Cloudflare gratuit).
2. Clique sur **"Create a project"** → **"Upload assets"**.
3. Glisse-dépose le dossier `market-radar-deploy/` (ou ses 10 fichiers).
4. Donne un nom au projet (ex: `market-hours-radar`).
5. Clique sur "Deploy".
6. Cloudflare donne une URL du type `https://market-hours-radar.pages.dev`.

---

## ✅ Vérification après déploiement

Ouvre l'URL donnée par l'hébergeur et vérifie :
- [ ] L'appli s'affiche (cadrans matin / après-midi)
- [ ] Le bandeau dit **"Volumes réels"** (pas "indicatifs")
- [ ] Ajoute `?selftest` à la fin de l'URL → doit afficher **PASS**
- [ ] Clic sur un nom dans la légende → épingle la place
- [ ] Survol d'un anneau du graphique → dé-pin immédiat (toutes les couleurs reviennent)

---

## 🔗 Mettre à jour tes liens

Une fois l'URL obtenue, remplace-la dans :
- `C:\Users\bento\Desktop\vente\index.html` (lien démo)
- `C:\Users\bento\mon-appli\ANNONCE-VENTE.md` (lien démo publique)
- Ton dashboard Bureau

---

## 💡 Astuce : ton site Qoder existe déjà

Tu as déjà une démo en ligne :  
**https://market-hours-radar-9986usim39q.qoder.website**

Si elle fonctionne, tu peux l'utiliser immédiatement pour vendre/diffuser. Le nouveau déploiement ci-dessus sert de sauvegarde ou de site principal si tu veux changer d'hébergeur.
