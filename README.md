# PageShot

English | [中文](languages/README_zh.md) | [Español](languages/README_es.md) | [Deutsch](languages/README_de.md) | [日本語](languages/README_ja.md) | [Français](languages/README_fr.md)

A lightweight browser extension for capturing screenshots — full page, visible area, or any selection. No forced watermark, fully local processing.

> Chromium-based · Manifest V3 · Zero tracking · Fully In-Browser Processing

---

## Why PageShot?

Most screenshot tools charge for full-page capture, add watermarks, or upload your data to remote servers. PageShot does everything inside your browser — no data ever leaves your machine.

| Advantage | Detail |
|-----------|--------|
| 🔒 **100% Private** | All processing happens locally. No servers, no uploads, no tracking. |
| 💧 **No Watermark** | Clean screenshots, no branding imposed on your captures. |
| 🆓 **No forced watermarks on captured images. |
| 📄 **Full Page Capture** | One-click long screenshot — scrolls and stitches automatically. |
| 📋 **Copy & Paste** | Copy to clipboard instantly — paste directly into chats, emails, documents. |
| ✏️ **Built-in Annotation** | Draw rectangles and mosaic blur before sharing. |
| ⚡ **Lightweight** | Under 100KB. No frameworks, no bloat. |
| 🌍 **6 Languages** | Auto-detects your browser language. |

---

## Features

| Feature | Description |
|---------|-------------|
| 📄 **Full Page Screenshot** | Captures the entire scrollable page by auto-scrolling and stitching segments. Handles lazy-loaded images and very long pages (10,000px+). |
| 👁 **Visible Area Capture** | Instant capture of what's currently on screen. The fastest way to screenshot. |
| ✂️ **Selection Capture** | Drag to select any region on the page with a crosshair overlay. Precise and flexible. |
| 📋 **Copy to Clipboard** | One-click copy after capture. Paste directly into any app with Ctrl+V. |
| 💾 **Download as PNG** | Auto-names files with page title + date (e.g. `GitHub_-_Homepage_2026-07-07.png`). |
| ✏️ **Rectangle Annotation** | Draw colored rectangles to highlight areas. 5 colors available: red, blue, green, black, white. |
| 🟦 **Mosaic Blur** | Pixelate sensitive content — passwords, personal info, private messages. |
| ⌨️ **Keyboard Shortcuts** | `Ctrl+Shift+V` — Capture visible + copy · `Ctrl+Shift+F` — Full page + download · `Ctrl+Shift+S` — Selection mode. |
| 🔤 **6-Language i18n** | UI auto-matches your browser language: English, 中文, 日本語, Español, Deutsch, Français. |
| 🔒 **Fixed Element Handling** | Automatically detects and removes sticky headers/footers from long screenshots. |

---

## Preview

<p align="center">
  <img src="icons/icon128.png" alt="PageShot Icon" width="80">
</p>

---

## Supported Browsers

| Browser | Status |
|---------|--------|
| Google Chrome | ✅ Fully supported |
| Microsoft Edge | ✅ Fully supported |
| Brave | ✅ Supported |
| Opera | ✅ Supported |
| Vivaldi | ✅ Supported |
| Any Chromium-based browser | ✅ Supported (Manifest V3) |

---

## Installation

### From Source (Developer Mode)

1. Open your browser's extension page:
   - **Chrome**: `chrome://extensions/`
   - **Edge**: `edge://extensions/`
2. Enable **Developer mode** (top-right toggle)
3. Click **Load unpacked** and select the `page-shot` folder
4. The PageShot icon will appear in your toolbar

---

## Usage

### Right-Click Capture

1. Right-click anywhere on a webpage
2. Select **PageShot** from the context menu
3. Choose: **Capture Visible Area**, **Capture Full Page**, or **Capture Selection**
4. A toast appears with **Copy**, **Download**, and **Edit** buttons

### Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl+Shift+V` | Capture visible area → copy to clipboard |
| `Ctrl+Shift+F` | Capture full page → download as PNG |
| `Ctrl+Shift+S` | Enter selection mode |

### Annotation

1. After capturing, click **✏️ Edit** on the toast
2. The annotation editor opens in a new tab
3. Use **Rectangle** or **Mosaic** tools from the toolbar
4. Pick a color (for rectangles)
5. Click **📋 Copy** or **💾 Download** when done

---

## Context Menu Structure

```
PageShot
├── Capture Visible Area
├── Capture Full Page
└── Capture Selection
```

---

## Privacy

PageShot is built with privacy as a core principle:

- ✅ **Zero data upload** — All screenshot processing happens locally
- ✅ **No analytics** — No tracking, no telemetry, no remote calls
- ✅ **No cookies** — No reading or writing of browser cookies
- ✅ **No browsing history** — No access to your browsing data
- ✅ **Temporary storage only** — Screenshots exist briefly during processing, then cleared
- ✅ **Minimal permissions** — Only requests what's strictly necessary

---

## How It Works

```
Trigger (right-click / shortcut / popup)
       ↓
Service Worker coordinates the capture
       ↓
┌─ Visible Area: chrome.tabs.captureVisibleTab()
├─ Full Page: scroll → capture each viewport segment → stitch via Canvas
└─ Selection: capture visible → crop to selection rectangle
       ↓
Offscreen Document processes image (stitch / crop / clipboard)
       ↓
Toast notification with Copy / Download / Edit actions
```

> **Why Offscreen?** Chrome's Manifest V3 runs the background as a Service Worker with no DOM access. The Canvas API requires a DOM, so we use Chrome's Offscreen API for image processing.

---

## Permissions

| Permission | Purpose |
|-----------|---------|
| `activeTab` | Access the current tab when you trigger a capture |
| `contextMenus` | Add right-click menu options |
| `downloads` | Save screenshots to your computer |
| `clipboardWrite` | Copy screenshots to your clipboard |
| `scripting` | Inject the selection overlay on web pages |
| `storage` | Save your preferences locally |
| `offscreen` | Process images in the background |
| `tabs` | Get tab info for capture coordination |
| `debugger` | Required for full-page screenshot stitching on certain Chromium builds |

---

## Copyright Disclaimer

This screenshot tool is only for users' personal learning, document sorting and offline content recording. All text, pictures and multimedia content on web pages belong to the original copyright owner. Users shall not use screenshots for commercial reproduction, unauthorized reprinting, public distribution and other copyright-infringing behaviors. All legal liabilities arising from improper use shall be borne solely by the user.

---

## License

Copyright © 2026 PageShot. All rights reserved.

---

## ❤️ Support

If you find PageShot helpful, consider supporting the project!

**[👉 Click here to support](https://ko-fi.com/annmax?ref=pageshot)**

---

> **Note:** This repository is for **project showcase purposes only**. It does not contain the full source code, manifest, icons, or build scripts. Full source code will **not** be published here.

