# Châteaux de la Loire — Installation

## Méthode rapide (sans cap sync)

### 1. Duplique un projet existant
Dans le Finder, duplique le dossier d'une de tes apps (ex: Musées de Paris)
→ Renomme-le en `ChateauxLoire`

### 2. Remplace les fichiers web
Copie `App/public/index.html` depuis ce zip
→ dans `ChateauxLoire/App/public/index.html` (remplace l'existant)

### 3. Remplace capacitor.config.json
Copie `capacitor.config.json` depuis ce zip
→ dans `ChateauxLoire/capacitor.config.json` (remplace l'existant)

### 4. Ouvre dans Xcode
Ouvre `ChateauxLoire/App/App.xcworkspace`

### 5. Modifie le Bundle Identifier
Dans Xcode → App target → Signing & Capabilities
→ Bundle Identifier : `com.michel.garlandat.chateauxloire`

### 6. Modifie le Display Name
Dans Xcode → Info → Bundle display name
→ `Châteaux de la Loire`

### 7. Vérifie Info.plist
Assure-toi que ces clés sont présentes (ne remplace pas tout le fichier) :
- NSAppTransportSecurity → NSAllowsArbitraryLoads → YES
- UIStatusBarStyle → UIStatusBarStyleLightContent
- ITSAppUsesNonExemptEncryption → NO

### 8. Lance sur ton iPhone
Sélectionne ton iPhone → ▶ Run

---

## Bundle ID
`com.michel.garlandat.chateauxloire`

## LocalStorage keys utilisées
- `cl_lang` — langue (fr/en)
- `cl_theme` — thème (dark/light)
- `cl_favs` — favoris (JSON array d'ids)
- `cl_img_*` — cache photos Wikipedia (7 jours)

## App Store Connect
- Catégorie principale : Education
- Âge : 4+
- Données collectées : Aucune
- Prix suggéré : 1,99 €
- Privacy Policy : https://migapple.github.io
