# PageShot

[English](../README.md) | [中文](README_zh.md) | [Español](README_es.md) | Deutsch | [日本語](README_ja.md) | [Français](README_fr.md)

Eine schlanke Browser-Erweiterung für Screenshots — ganze Seite, sichtbarer Bereich oder beliebige Auswahl. Kein erzwungenes Wasserzeichen, komplette lokale Verarbeitung.

> Chrome / Edge / Firefox · Manifest V3 · Kein Tracking · Verarbeitung vollständig im Browser

---

## Warum PageShot?

Die meisten Screenshot-Tools verlangen Geld für Ganze-Seite-Captures, fügen Wasserzeichen hinzu oder laden deine Daten auf Remote-Server hoch. PageShot erledigt alles in deinem Browser — keine Screenshot-Daten verlassen jemals deinen Rechner.

| Vorteil | Details |
|---------|---------|
| 🔒 **Datenschutz zuerst** | Alles wird lokal verarbeitet. Keine Uploads, kein Tracking. Die einzige ausgehende Anfrage ist die optionale Lizenzprüfung. |
| 💧 **Kein Wasserzeichen** | Saubere Screenshots, kein Branding auf deinen Aufnahmen. |
| 📄 **Ganze Seite** | Klick auf einen langen Screenshot — scrollt und fügt automatisch zusammen. |
| 📋 **Kopieren & Einfügen** | Sofort in die Zwischenablage kopieren — direkt in Chats, E-Mails, Dokumente einfügen. |
| ✏️ **Integrierte Annotation** | Rechtecke, Ellipsen, Pfeile, Text und Mosaik-Blur vor dem Teilen zeichnen. |
| ⚡ **Leichtgewichtig** | Keine Frameworks, kein Ballast. |
| 🌍 **6 Sprachen** | Erkennt automatisch deine Browsersprache. |

---

## Funktionen

### 🆓 Kostenlose Funktionen

| Funktion | Beschreibung |
|----------|--------------|
| 📄 **Ganze Seite** | Erfasst die gesamte scrollbare Seite in einem Shot über Chrome DevTools Protocol. Behandelt Lazy-Loaded Bilder und sehr lange Seiten. |
| 👁 **Sichtbarer Bereich** | Sofortige Erfassung dessen, was gerade auf dem Bildschirm ist. Der schnellste Weg zum Screenshot. |
| ✂️ **Auswahl** | Ziehen, um einen beliebigen Bereich auf der Seite mit Fadenkreuz-Overlay auszuwählen. Präzise und flexibel. |
| 📋 **In Zwischenablage kopieren** | Ein-Klick-Kopie nach der Aufnahme. Direkt in jede App mit Strg+V einfügen. |
| 💾 **Als PNG herunterladen** | Dateien werden automatisch benannt: Seitentitel + Datum (z.B. `GitHub_-_Homepage_2026-07-07.png`). |
| ✏️ **Rechteck-Annotation** | Farbige Rechtecke zum Markieren von Bereichen zeichnen. 5 Farben verfügbar: Rot, Blau, Grün, Schwarz, Weiß. |
| ◯ **Ellipsen-Annotation** | Eine Ellipse um ein Steuerelement, einen Fehler oder einen Bereich zeichnen. |
| ➜ **Pfeil-Annotation** | Mit einem Pfeil auf die genaue Schaltfläche, das Feld oder die Zeile zeigen. |
| T **Text-Annotation** | Eine Beschriftung direkt auf den Screenshot schreiben. |
| 🟦 **Mosaik-Blur** | Sensible Inhalte verpixeln — Passwörter, persönliche Daten, private Nachrichten. |
| ⌨️ **Tastenkürzel** | `Strg+Umschalt+V` — Sichtbaren Bereich erfassen + kopieren · `Strg+Umschalt+F` — Ganze Seite + Download · `Strg+Umschalt+S` — Auswahlmodus. |
| 🔤 **6-Sprachen-i18n** | UI passt sich automatisch an deine Browsersprache an: English, 中文, 日本語, Español, Deutsch, Français. |
| 🔒 **Fixierte Elemente** | Erkennt und entfernt automatisch Sticky-Header/Footer aus langen Screenshots. |

### ⭐ Premium-Funktionen (Lizenz erforderlich)

| Funktion | Beschreibung |
|----------|--------------|
| 📑 **Als PDF exportieren** | Jeden aufgenommenen Screenshot (inkl. langer Seiten) als PDF-Dokument exportieren — aus dem Annotation-Editor heraus |

### Kostenlos vs. Premium

| | Kostenlos | Premium |
|---|:---:|:---:|
| Ganze Seite / Sichtbar / Auswahl | ✅ | ✅ |
| In Zwischenablage kopieren & als PNG herunterladen | ✅ | ✅ |
| Rechteck-, Ellipsen-, Pfeil- und Text-Annotation & Mosaik-Blur | ✅ | ✅ |
| Tastenkürzel | ✅ | ✅ |
| Fixierte Elemente behandeln | ✅ | ✅ |
| Als PDF exportieren | — | ✅ |

---

## Vorschau

<p align="center">
  <img src="../icons/icon128.png" alt="PageShot Symbol" width="80">
</p>

---

## Unterstützte Browser

| Browser | Status |
|---------|--------|
| Google Chrome | ✅ Vollständig unterstützt |
| Microsoft Edge | ✅ Vollständig unterstützt |
| Mozilla Firefox | ✅ Vollständig unterstützt |
| Brave | ✅ Unterstützt |
| Opera | ✅ Unterstützt |
| Vivaldi | ✅ Unterstützt |
| Jeder Chromium-basierte Browser | ✅ Unterstützt (Manifest V3) |

> **Firefox-Hinweis:** Firefox bietet keine Debugger-API für Erweiterungen, daher gibt es keinen Debugger-Modus. Firefox kennt kein Offscreen-Dokument (offscreen API), daher die Ganzseiten-Aufnahme auf Scroll-Stitching innerhalb der Seite zurückgreift; die Berechtigung `offscreen` wird in der Firefox-Version nicht angefordert. Die übrigen Funktionen verhalten sich wie unter Chrome / Edge.

---

## Installation

| Store | Link |
|---|---|
| Chrome Web Store | [In Chrome installieren](https://chromewebstore.google.com/detail/jonikcknondlhibmemapljjodhjikcje) |
| Microsoft Edge Add-ons | [In Edge installieren](https://microsoftedge.microsoft.com/addons/detail/pooedlcmpdgcfkjfojhblenegbhhahmd) |
| Firefox-Add-ons (AMO) | 🔜 In Prüfung – Link folgt nach der Freigabe |

> Installieren Sie nur über die offiziellen Stores oben – meiden Sie Download-Seiten Dritter.

---

## Verwendung

### Rechtsklick-Aufnahme

1. Rechtsklick irgendwo auf einer Webseite
2. Wähle **PageShot** aus dem Kontextmenü
3. Wähle: **Sichtbaren Bereich erfassen**, **Ganze Seite erfassen** oder **Auswahl erfassen**
4. Ein Toast erscheint mit den Buttons **Kopieren**, **Herunterladen** und **Bearbeiten**

### Tastenkürzel

| Tastenkürzel | Aktion |
|---------------|--------|
| `Strg+Umschalt+V` | Sichtbaren Bereich erfassen → in Zwischenablage kopieren |
| `Strg+Umschalt+F` | Ganze Seite erfassen → als PNG herunterladen |
| `Strg+Umschalt+S` | Auswahlmodus starten |

### Annotation

1. Nach der Aufnahme klicke auf **✏️ Bearbeiten** im Toast
2. Der Annotation-Editor öffnet sich in einem neuen Tab
3. Verwende **Rechteck**, **Ellipse**, **Pfeil**, **Text** oder **Mosaik** aus der Toolbar
4. Wähle eine Farbe (für Formen und Text)
5. Klicke auf **📋 Kopieren** oder **💾 Herunterladen**, wenn fertig

---

## Kontextmenü-Struktur

- Sichtbaren Bereich erfassen
- Ganze Seite erfassen
- Auswahl erfassen

---

## Datenschutz

PageShot wurde mit Datenschutz als Grundprinzip entwickelt:

- ✅ **Kein Datenupload** — Die gesamte Screenshot-Verarbeitung passiert lokal
- ✅ **Keine Analytik** — Kein Tracking, keine Telemetrie, keine Remote-Aufrufe außer der optionalen Lizenzprüfung
- ✅ **Keine Cookies** — Kein Lesen oder Schreiben von Browser-Cookies
- ✅ **Kein Verlauf** — Kein Zugriff auf deine Browserdaten
- ✅ **Lokaler Bearbeitungsspeicher** — Die fünf letzten Aufnahmen bleiben für den Anmerkungseditor im Browser; ältere werden automatisch entfernt. Nichts wird hochgeladen
- ✅ **Minimale Berechtigungen** — Nur das absolut Notwendige

---

## So funktioniert es

1. Starte die Aufnahme über das Rechtsklick-Menü, ein Tastenkürzel oder das Popup.
2. Wähle, was du erfassen willst: den sichtbaren Bereich, die ganze Seite oder einen von dir ausgewählten Bereich.
3. Das Bild wird vollständig in deinem Browser zugeschnitten und verarbeitet.
4. Eine Meldung bietet Kopieren, Herunterladen oder Bearbeiten an.

---

## Berechtigungen

| Berechtigung | Zweck |
|---------------|-------|
| `activeTab` | Zugriff auf den aktuellen Tab bei Auslösung einer Aufnahme |
| `contextMenus` | Rechtsklick-Menüoptionen hinzufügen |
| `downloads` | Screenshots auf deinem Computer speichern |
| `clipboardWrite` | Screenshots in deine Zwischenablage kopieren |
| `scripting` | Auswahl-Overlay auf Webseiten injizieren |
| `storage` | Einstellungen lokal speichern |
| `offscreen` | Bilder im Hintergrund verarbeiten |
| `tabs` | Tab-Info für Aufnahmekoordination abrufen |
| `debugger` | Erforderlich für Ganze-Seite-Screenshot-Zusammenführung auf bestimmten Chromium-Builds (nur Chrome / Edge) |

---

## Urheberrechtshinweis

Dieses Screenshot-Tool dient ausschließlich dem persönlichen Lernen, der Dokumentenordnung und der Offline-Inhaltsaufzeichnung. Alle Texte, Bilder und multimediale Inhalte auf Webseiten gehören dem jeweiligen Urheberrechtsinhaber. Nutzer dürfen Screenshots nicht für kommerzielle Vervielfältigung, unbefugte Weiterveröffentlichung, öffentliche Verbreitung oder andere urheberrechtsverletzende Handlungen verwenden. Alle rechtlichen Folgen aus missbräuchlicher Nutzung trägt allein der Nutzer.

---

## Lizenz

Copyright © 2026 PageShot. Alle Rechte vorbehalten.

---

## ❤️ Support

Wenn dir PageShot hilft, unterstütze das Projekt gerne!

**[👉 Hier unterstützen](https://ko-fi.com/annmax?ref=pageshot)**

---

> **Hinweis:** Dieses Repository dient ausschließlich der **Projektpräsentation**. Es enthält nicht den vollständigen Quellcode, das Manifest, Icons oder Build-Skripte. Der vollständige Quellcode wird hier **nicht** veröffentlicht.
