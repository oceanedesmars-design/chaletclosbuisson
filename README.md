# 🏔️ Chalet Clos Buisson — Site Vitrine

Site vitrine haut de gamme pour la location du **Chalet Clos Buisson** à Chantemerle, Serre-Chevalier.

## ✨ Fonctionnalités

- **Design chaleureux & luxe alpin** — palette bois/or, typographie élégante (Cormorant Garamond)
- **Hero animé** avec zoom progressif sur la photo principale
- **Galerie photos** avec lightbox (navigation clavier + molette)
- **Présentation des deux espaces** — L'Églantier & Le Mélèze (hover interactif)
- **Fiche équipements** complète avec icônes
- **6 chambres** présentées en grille
- **Avis voyageurs** avec barres de notation animées
- **Localisation** avec carte Google Maps intégrée
- **Livret d'accueil PDF** — glisser-déposer ou sélection de fichier
- **Navigation fixe** qui change d'apparence au scroll
- **Responsive** — mobile, tablette, desktop
- **Animations** à l'entrée au scroll (Intersection Observer)

## 📁 Structure

```
/
├── index.html        ← site complet (fichier unique)
└── README.md
```

Tout le site tient dans un **seul fichier HTML** — aucune dépendance externe hormis les polices Google Fonts et les images Airbnb.

## 🚀 Déploiement sur GitHub Pages

### Option 1 — Interface web GitHub (recommandé)

1. Créez un nouveau dépôt sur [github.com](https://github.com) (ex: `chalet-clos-buisson`)
2. Uploadez `index.html` via le bouton **"Add file > Upload files"**
3. Allez dans **Settings → Pages**
4. Source : **"Deploy from a branch"** → branche `main`, dossier `/ (root)`
5. Cliquez **Save** → votre site est en ligne en 1-2 minutes

🌐 URL : `https://votre-pseudo.github.io/chalet-clos-buisson/`

### Option 2 — Git en ligne de commande

```bash
git init
git add index.html
git commit -m "Initial commit - Chalet Clos Buisson"
git branch -M main
git remote add origin https://github.com/VOTRE-PSEUDO/chalet-clos-buisson.git
git push -u origin main
```

Puis activez GitHub Pages dans Settings → Pages.

## 📄 Livret d'accueil PDF

Le livret d'accueil est **intégré côté client** : il n'est pas stocké sur le serveur.

**Pour les visiteurs du site :**
1. Rendez-vous dans la section "Livret d'accueil"
2. Glissez votre fichier PDF ou cliquez pour le sélectionner
3. Un bouton de téléchargement apparaît

**Si vous souhaitez intégrer le PDF en permanence dans le site :**
- Ajoutez votre PDF dans le dépôt (ex: `livret-accueil.pdf`)
- Modifiez la section `#welcome-book` dans `index.html` pour pointer vers ce fichier :

```html
<!-- Remplacez la zone d'upload par un lien direct -->
<a href="livret-accueil.pdf" download class="wb-download-btn">
  <span>📥</span> Télécharger le livret d'accueil
</a>
```

## 🎨 Personnalisation

### Couleurs (lignes CSS `:root`)
- `--pine` : vert sapin principal
- `--gold` : accent doré
- `--cream` : fond crème chaleureux

### Informations à mettre à jour
- `mailto:contact@closbuisson.fr` → votre vraie adresse e-mail
- Numéro de téléphone dans le footer
- Lien Airbnb (déjà correct dans le code)
- Carte Google Maps (l'iframe affiche Chantemerle)

## 🛠️ Technologies

- HTML5 / CSS3 / JavaScript vanilla
- Google Fonts (Cormorant Garamond + Jost)
- Images : hébergées sur Airbnb CDN
- Carte : Google Maps Embed API (gratuit, sans clé)

---

*Fait avec ❤️ pour le Chalet Clos Buisson — Serre-Chevalier*
