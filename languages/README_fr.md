# PageShot

[English](../README.md) | [中文](README_zh.md) | [Español](README_es.md) | [Deutsch](README_de.md) | [日本語](README_ja.md) | Français

Une extension légère pour capturer des captures d'écran — page complète, zone visible, ou n'importe quelle sélection. Pas de filigrane imposé, traitement 100 % local.

> Chrome / Edge / Firefox · Manifest V3 · Aucun suivi · Traitement 100 % dans le navigateur

---

## Pourquoi PageShot ?

La plupart des outils de capture d'écran facturent la capture de page complète, ajoutent des filigranes ou envoient vos données sur des serveurs distants. PageShot fait tout dans votre navigateur — aucune capture ne quitte votre navigateur.

| Avantage | Détail |
|-----------|--------|
| 🔒 **Confidentialité avant tout** | Tout le traitement se fait en local. Pas d'envoi, pas de suivi. La seule requête sortante est la validation facultative de licence. |
| 💧 **Sans filigrane** | Captures propres, aucune marque imposée sur vos images. |
| 📄 **Capture de page complète** | Capture longue en un clic — défilement et assemblage automatiques. |
| 📋 **Copier et coller** | Copie instantanée dans le presse-papiers — collez directement dans vos conversations, e-mails, documents. |
| ✏️ **Annotations intégrées** | Dessinez des rectangles, des ellipses, des flèches et du texte, et appliquez un flou en mosaïque avant de partager. |
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
| ◯ **Annotation par ellipse** | Entourez un contrôle, une erreur ou une zone avec une ellipse. |
| ➜ **Annotation par flèche** | Pointez le bouton, le champ ou la ligne exacts avec une flèche. |
| T **Annotation texte** | Saisissez une étiquette directement sur la capture. |
| 🟦 **Flou en mosaïque** | Pixellisez les contenus sensibles — mots de passe, informations personnelles, messages privés. |
| ⌨️ **Raccourcis clavier** | `Ctrl+Shift+V` — Capturer la zone visible + copier · `Ctrl+Shift+F` — Page complète + télécharger · `Ctrl+Shift+S` — Mode sélection. |
| 🔤 **i18n en 6 langues** | L'interface s'adapte automatiquement à la langue de votre navigateur : English, 中文, 日本語, Español, Deutsch, Français. |
| 🔒 **Gestion des éléments fixes** | Détecte et supprime automatiquement les en-têtes/pieds de page fixes des captures longues. |

### ⭐ Fonctionnalités Premium (licence requise)

| Fonctionnalité | Description |
|---------|-------------|
| 📑 **Export en PDF** | Exportez n'importe quelle capture (y compris les longues pages) en document PDF — depuis l'éditeur d'annotations |

### Gratuit vs Premium

| | Gratuit | Premium |
|---|:---:|:---:|
| Capture page complète / zone visible / sélection | ✅ | ✅ |
| Copier dans le presse-papiers et télécharger en PNG | ✅ | ✅ |
| Annotation par rectangle, ellipse, flèche et texte, et flou en mosaïque | ✅ | ✅ |
| Raccourcis clavier | ✅ | ✅ |
| Gestion des éléments fixes | ✅ | ✅ |
| Export en PDF | — | ✅ |

---

## Aperçu

<p align="center">
  <img src="../icons/icon128.png" alt="Icône PageShot" width="80">
</p>

---

## Navigateurs compatibles

| Navigateur | Statut |
|---------|--------|
| Google Chrome | ✅ Entièrement pris en charge |
| Microsoft Edge | ✅ Entièrement pris en charge |
| Mozilla Firefox | ✅ Entièrement pris en charge |
| Brave | ✅ Pris en charge |
| Opera | ✅ Pris en charge |
| Vivaldi | ✅ Pris en charge |
| Tout navigateur basé sur Chromium | ✅ Pris en charge (Manifest V3) |

> **Note Firefox :** Firefox n’offre pas d’API de débogueur pour les extensions : le mode débogueur n’est donc pas proposé. Firefox ne propose pas de document offscreen, la capture pleine page passe à un assemblage par défilement dans la page ; la version Firefox ne demande donc pas la permission `offscreen`. Le reste des fonctions se comporte comme sous Chrome / Edge.

---

## Installation

| Store | Lien |
|---|---|
| Chrome Web Store | [Installer dans Chrome](https://chromewebstore.google.com/detail/jonikcknondlhibmemapljjodhjikcje) |
| Microsoft Edge Add-ons | [Installer dans Edge](https://microsoftedge.microsoft.com/addons/detail/pooedlcmpdgcfkjfojhblenegbhhahmd) |
| Modules complémentaires Firefox (AMO) | 🔜 En cours d’examen — le lien sera ajouté après publication |

> Installez uniquement depuis les boutiques officielles ci-dessus — évitez les sites de téléchargement tiers.

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
3. Utilisez les outils **Rectangle**, **Ellipse**, **Flèche**, **Texte** ou **Mosaïque** depuis la barre d'outils
4. Choisissez une couleur (pour les formes et le texte)
5. Cliquez sur **📋 Copier** ou **💾 Télécharger** quand vous avez terminé

---

## Structure du menu contextuel

- Capturer la zone visible
- Capturer la page complète
- Capturer la sélection

---

## Confidentialité

PageShot a été conçu avec la confidentialité comme principe fondamental :

- ✅ **Zéro envoi de données** — Tout le traitement des captures se fait en local
- ✅ **Pas d'analytics** — Aucun suivi, aucune télémétrie, aucun appel distant hormis la validation facultative de licence
- ✅ **Pas de cookies** — Aucune lecture ni écriture de cookies du navigateur
- ✅ **Pas d'historique de navigation** — Aucun accès à vos données de navigation
- ✅ **Stockage local d'édition** — Les cinq captures les plus récentes restent dans votre navigateur pour l'éditeur d'annotations et les plus anciennes sont supprimées automatiquement ; rien n'est téléversé
- ✅ **Permissions minimales** — Ne demande que le strict nécessaire

---

## Fonctionnement

1. Lancez la capture depuis le menu du clic droit, un raccourci clavier ou le popup.
2. Choisissez ce que vous voulez capturer : la zone visible, la page entière ou une zone que vous sélectionnez.
3. L'image est recadrée et traitée entièrement dans votre navigateur.
4. Une notification vous propose **Copier**, **Télécharger** ou **Modifier**.

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
| `debugger` | Nécessaire pour l'assemblage de captures de page complète sur certaines versions de Chromium (uniquement Chrome / Edge) |

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
