# PageShot

[English](../README.md) | [中文](README_zh.md) | [Español](README_es.md) | [Deutsch](README_de.md) | [日本語](README_ja.md) | Français

Une extension légère pour capturer des captures d'écran — page complète, zone visible, ou n'importe quelle sélection. Pas de filigrane imposé, traitement 100 % local.

> Chromium · Manifest V3 · Aucun suivi · Traitement 100 % dans le navigateur

---

## Pourquoi PageShot ?

La plupart des outils de capture d'écran facturent la capture de page complète, ajoutent des filigranes ou envoient vos données sur des serveurs distants. PageShot fait tout dans votre navigateur — aucune donnée ne quitte votre machine.

| Avantage | Détail |
|-----------|--------|
| 🔒 **Confidentialité avant tout** | Tout le traitement se fait en local. Pas de serveurs, pas d'envoi, pas de suivi. |
| 💧 **Sans filigrane** | Captures propres, aucune marque imposée sur vos images. |
| 🆓 **Pas de filigrane forcé sur les images capturées. |
| 📄 **Capture de page complète** | Capture longue en un clic — défilement et assemblage automatiques. |
| 📋 **Copier et coller** | Copie instantanée dans le presse-papiers — collez directement dans vos conversations, e-mails, documents. |
| ✏️ **Annotations intégrées** | Dessinez des rectangles et appliquez un flou en mosaïque avant de partager. |
| ⚡ **Léger** | Aucun framework, aucun surplus. |
| 🌍 **6 langues** | Détecte automatiquement la langue de votre navigateur. |

---

## Fonctionnalités

### 🆓 Fonctionnalités gratuites

| Fonctionnalité | Description |
|---------|-------------|
| 📄 **Capture de page complète** | Capture toute la page défileable en une seule fois via le Chrome DevTools Protocol. Gère les images en chargement différé et les très longues pages. |
| 👁 **Capture de la zone visible** | Capture instantanée de ce qui est affiché à l'écran. Le moyen le plus rapide de capturer. |
| ✂️ **Capture par sélection** | Glissez pour sélectionner une zone de la page avec un réticule de précision. Flexible et précis. |
| 📋 **Copier dans le presse-papiers** | Copie en un clic après la capture. Collez directement dans n'importe quelle application avec Ctrl+V. |
| 💾 **Télécharger en PNG** | Nomme automatiquement les fichiers avec le titre de la page + la date (ex. : `GitHub_-_Homepage_2026-07-07.png`). |
| ✏️ **Annotation par rectangle** | Dessinez des rectangles colorés pour mettre en avant des zones. 5 couleurs disponibles : rouge, bleu, vert, noir, blanc. |
| 🟦 **Flou en mosaïque** | Pixellisez les contenus sensibles — mots de passe, informations personnelles, messages privés. |
| ⌨️ **Raccourcis clavier** | `Ctrl+Shift+V` — Capturer la zone visible + copier · `Ctrl+Shift+F` — Page complète + télécharger · `Ctrl+Shift+S` — Mode sélection. |
| 🔤 **i18n en 6 langues** | L'interface s'adapte automatiquement à la langue de votre navigateur : English, 中文, 日本語, Español, Deutsch, Français. |
| 🔒 **Gestion des éléments fixes** | Détecte et supprime automatiquement les en-têtes/pieds de page fixes des captures longues. |

### ⭐ Fonctionnalités Premium (licence requise)

| Fonctionnalité | Description |
|---------|-------------|
| 📑 **Export en PDF** | Exportez n'importe quelle capture (y compris les longues pages) en document PDF — depuis l'éditeur d'annotations |
| 💬 **Support prioritaire** | Support e-mail prioritaire pour les utilisateurs Premium |

### Gratuit vs Premium

| | Gratuit | Premium |
|---|:---:|:---:|
| Capture page complète / zone visible / sélection | ✅ | ✅ |
| Copier dans le presse-papiers et télécharger en PNG | ✅ | ✅ |
| Annotation par rectangle et flou en mosaïque | ✅ | ✅ |
| Raccourcis clavier | ✅ | ✅ |
| Gestion des éléments fixes | ✅ | ✅ |
| Export en PDF | — | ✅ |
| Support prioritaire | — | ✅ |

---

## Aperçu

<p align="center">
  <img src="icons/icon128.png" alt="Icône PageShot" width="80">
</p>

---

## Navigateurs compatibles

| Navigateur | Statut |
|---------|--------|
| Google Chrome | ✅ Entièrement pris en charge |
| Microsoft Edge | ✅ Entièrement pris en charge |
| Brave | ✅ Pris en charge |
| Opera | ✅ Pris en charge |
| Vivaldi | ✅ Pris en charge |
| Tout navigateur basé sur Chromium | ✅ Pris en charge (Manifest V3) |

---

## Installation

### Depuis les sources (mode développeur)

1. Ouvrez la page des extensions de votre navigateur :
   - **Chrome** : `chrome://extensions/`
   - **Edge** : `edge://extensions/`
2. Activez le **mode Développeur** (bouton en haut à droite)
3. Cliquez sur **Charger le package décompressé** et sélectionnez le dossier `page-shot`
4. L'icône PageShot apparaît dans votre barre d'outils

---

## Utilisation

### Capture par clic droit

1. Faites un clic droit n'importe où sur une page web
2. Sélectionnez **PageShot** dans le menu contextuel
3. Choisissez : **Capturer la zone visible**, **Capturer la page complète**, ou **Capturer la sélection**
4. Une notification apparaît avec les boutons **Copier**, **Télécharger** et **Modifier**

### Raccourcis clavier

| Raccourci | Action |
|----------|--------|
| `Ctrl+Shift+V` | Capturer la zone visible → copier dans le presse-papiers |
| `Ctrl+Shift+F` | Capturer la page complète → télécharger en PNG |
| `Ctrl+Shift+S` | Entrer en mode sélection |

### Annotations

1. Après la capture, cliquez sur **✏️ Modifier** dans la notification
2. L'éditeur d'annotations s'ouvre dans un nouvel onglet
3. Utilisez les outils **Rectangle** ou **Mosaïque** depuis la barre d'outils
4. Choisissez une couleur (pour les rectangles)
5. Cliquez sur **📋 Copier** ou **💾 Télécharger** quand vous avez terminé

---

## Structure du menu contextuel

```
PageShot
├── Capturer la zone visible
├── Capturer la page complète
└── Capturer la sélection
```

---

## Confidentialité

PageShot a été conçu avec la confidentialité comme principe fondamental :

- ✅ **Zéro envoi de données** — Tout le traitement des captures se fait en local
- ✅ **Pas d'analytics** — Aucun suivi, aucune télémétrie, aucun appel distant
- ✅ **Pas de cookies** — Aucune lecture ni écriture de cookies du navigateur
- ✅ **Pas d'historique de navigation** — Aucun accès à vos données de navigation
- ✅ **Stockage temporaire uniquement** — Les captures existent brièvement pendant le traitement, puis sont supprimées
- ✅ **Permissions minimales** — Ne demande que le strict nécessaire

---

## Fonctionnement

```
Déclenchement (clic droit / raccourci / popup)
       ↓
Le Service Worker coordonne la capture
       ↓
┌─ Zone visible : chrome.tabs.captureVisibleTab()
├─ Page complète : extension du viewport via CDP → capture haute résolution unique
└─ Sélection : capture de la zone visible → recadrage au rectangle de sélection
       ↓
Le document Offscreen traite l'image (recadrage / presse-papiers)
       ↓
Notification avec les actions Copier / Télécharger / Modifier
```

> **Pourquoi Offscreen ?** Le Manifest V3 de Chrome exécute le Service Worker en arrière-plan, sans accès au DOM. Le Canvas API nécessite un DOM, on utilise donc l'API Offscreen de Chrome pour le traitement des images.

---

## Permissions

| Permission | Utilisation |
|-----------|---------|
| `activeTab` | Accède à l'onglet actif quand vous déclenchez une capture |
| `contextMenus` | Ajoute des options dans le menu du clic droit |
| `downloads` | Enregistre les captures sur votre ordinateur |
| `clipboardWrite` | Copie les captures dans votre presse-papiers |
| `scripting` | Injecte le calque de sélection sur les pages web |
| `storage` | Sauvegarde vos préférences en local |
| `offscreen` | Traite les images en arrière-plan |
| `tabs` | Récupère les infos des onglets pour la coordination de capture |
| `debugger` | Nécessaire pour l'assemblage de captures de page complète sur certaines versions de Chromium |

---

## Avertissement relatif au droit d'auteur

Cet outil de capture d'écran est destiné uniquement à l'usage personnel des utilisateurs pour l'apprentissage, le tri de documents et l'enregistrement de contenus hors ligne. Tous les textes, images et contenus multimédias des pages web appartiennent à leurs propriétaires respectifs. Les utilisateurs ne doivent pas utiliser les captures à des fins de reproduction commerciale, de republication non autorisée, de distribution publique ou de toute autre activité portant atteinte au droit d'auteur. Toute responsabilité juridique découlant d'une utilisation inappropriée incombe exclusivement à l'utilisateur.

---

## Licence

Copyright © 2026 PageShot. Tous droits réservés.

---

## ❤️ Soutenir

Si PageShot vous est utile, n'hésitez pas à soutenir le projet !

**[👉 Cliquez ici pour soutenir](https://ko-fi.com/annmax?ref=pageshot)**

---

> **Note :** Ce dépôt est destiné à la **présentation du projet uniquement**. Il ne contient pas le code source complet, le manifest, les icônes ou les scripts de build. Le code source complet ne sera **pas** publié ici.
