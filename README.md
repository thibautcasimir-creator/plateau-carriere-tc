"# Plateau de Carrière RH — Thibaut Casimir

CV interactif inspiré du Monopoly, déployable sur **GitHub Pages** (statique, 0 build, 0 dépendance).

## 📁 Structure

```
.
├── index.html     # Page principale (plateau interactif)
├── admin.html     # Espace admin (mot de passe : admin2026)
├── data.js        # Contenu des 24 cases + mot de passe + coordonnées contact
└── README.md
```

## 🚀 Déploiement sur GitHub Pages

1. **Créez un repository GitHub** (ex: `cv-plateau-rh`).
2. **Poussez les 4 fichiers** à la racine du repo :
   ```bash
   git init
   git add index.html admin.html data.js README.md
   git commit -m \"feat: plateau de carrière RH\"
   git branch -M main
   git remote add origin https://github.com/<votre-user>/cv-plateau-rh.git
   git push -u origin main
   ```
3. **Activez GitHub Pages** :
   - Allez dans `Settings` → `Pages`
   - Source : `Deploy from a branch`
   - Branch : `main` / dossier `/ (root)`
   - Cliquez sur `Save`
4. Au bout de 1-2 minutes, le site est en ligne sur :
   `https://<votre-user>.github.io/cv-plateau-rh/`

## 🔐 Mode admin

- URL : `https://<votre-site>/admin.html`
- Mot de passe par défaut : **`admin2026`**
- Pour le changer : éditez la constante `ADMIN_PASSWORD` dans `data.js`.

## ✏️ Modifier les contenus

Deux options :

### Option A — Via l'interface admin (recommandé)
- Ouvrez `admin.html`, connectez-vous, modifiez les cases et coordonnées, cliquez sur **Enregistrer**.
- ⚠️ Les modifications sont stockées dans le **`localStorage` du navigateur**. Elles ne sont visibles que sur **votre appareil + navigateur**. Elles ne sont pas poussées sur GitHub.

### Option B — Pour rendre les changements permanents pour tous les visiteurs
Éditez directement `data.js` (modifiez `DEFAULT_SQUARES` et `DEFAULT_CONTACT`), puis poussez le commit sur GitHub.

## 📱 QR Code

Une fois le site en ligne, générez un QR code pointant vers l'URL GitHub Pages
(par exemple via [qr-code-generator.com](https://www.qr-code-generator.com/)) et
imprimez-le sur votre CV.

## 🖼️ Image du plateau

L'image du plateau Canva est chargée depuis l'URL Emergent en CDN. Si vous
souhaitez la remplacer par votre propre URL, modifiez l'attribut `src` de
`<img id=\"board-image\">` dans `index.html`.

## ⚙️ Réinitialiser le navigateur

Pour effacer les modifications locales et revenir aux contenus par défaut :
- Bouton **Restaurer** dans l'admin, OU
- DevTools (F12) → Application → Local Storage → supprimer les clés `tc_*`.

---

© Thibaut Casimir · Plateau de Parcours RH · CV augmenté
"
