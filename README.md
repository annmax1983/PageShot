# PageShot

English | [中文](languages/README_zh.md) | [Español](languages/README_es.md) | [Deutsch](languages/README_de.md) | [日本語](languages/README_ja.md) | [Français](languages/README_fr.md)

A lightweight browser extension for capturing screenshots — full page, visible area, or any selection. No forced watermark, fully local processing.

> Chrome · Edge · Firefox · Manifest V3 · No tracking · Fully In-Browser Processing

---

## Why PageShot?

Most screenshot tools charge for full-page capture, add watermarks, or upload your data to remote servers. PageShot does everything inside your browser — no screenshot data ever leaves your machine.

| Advantage | Detail |
|-----------|--------|
| 🔒 **Privacy-First** | All processing happens locally. No uploads, no tracking. The only outbound request is optional license validation. |
| 💧 **No Watermark** | Clean screenshots, no branding imposed on your captures. |
| 📄 **Full Page Capture** | One-click long screenshot — scrolls and stitches automatically. |
| 📋 **Copy & Paste** | Copy to clipboard instantly — paste directly into chats, emails, documents. |
| ✏️ **Built-in Annotation** | Draw rectangles, ellipses, arrows, text and mosaic blur before sharing. |
| ⚡ **Lightweight** | No frameworks, no bloat. |
| 🌍 **6 Languages** | Auto-detects your browser language. |

---

## Features

### 🆓 Free Features

| Feature | Description |
|---------|-------------|
| 📄 **Full Page Screenshot** | Captures the entire scrollable page in one shot — via the Chrome DevTools Protocol on Chrome / Edge, and via scroll-and-stitch inside the page on Firefox. Handles lazy-loaded images and very long pages. |
| 👁 **Visible Area Capture** | Instant capture of what's currently on screen. The fastest way to screenshot. |
| ✂️ **Selection Capture** | Drag to select any region on the page with a crosshair overlay. Precise and flexible. |
| 📋 **Copy to Clipboard** | One-click copy after capture. Paste directly into any app with Ctrl+V. |
| 💾 **Download as PNG** | Auto-names files with page title + date (e.g. `GitHub_-_Homepage_2026-07-07.png`). |
| ✏️ **Rectangle Annotation** | Draw colored rectangles to highlight areas. 5 colors available: red, blue, green, black, white. |
| ◯ **Ellipse Annotation** | Draw an ellipse around a control, an error or a region. |
| ➜ **Arrow Annotation** | Point an arrow at the exact button, field or line you mean. |
| T **Text Annotation** | Type a label directly on the screenshot. |
| 🟦 **Mosaic Blur** | Pixelate sensitive content — passwords, personal info, private messages. |
| ⌨️ **Keyboard Shortcuts** | `Ctrl+Shift+V` — Capture visible + copy · `Ctrl+Shift+F` — Full page + download · `Ctrl+Shift+S` — Selection mode. |
| 🔤 **6-Language i18n** | UI auto-matches your browser language: English, 中文, 日本語, Español, Deutsch, Français. |
| 🔒 **Fixed Element Handling** | Automatically detects and removes sticky headers/footers from long screenshots. |

### ⭐ Premium Features (License Required)

| Feature | Description |
|---------|-------------|
| 📑 **Export as PDF** | Export any captured screenshot (including long pages) as a PDF document — from the annotation editor |

### Free vs Premium

| | Free | Premium |
|---|:---:|:---:|
| Full page / visible / selection capture | ✅ | ✅ |
| Copy to clipboard & download as PNG | ✅ | ✅ |
| Rectangle, ellipse, arrow and text annotation & mosaic blur | ✅ | ✅ |
| Keyboard shortcuts | ✅ | ✅ |
| Fixed element handling | ✅ | ✅ |
| Export as PDF | — | ✅ |

---

## Preview

<p align="center">
  <img src="icons/icon128.png" alt="PageShot Icon" width="80">
</p>

---

## Supported Browsers

| Browser | Status | Notes |
|---------|--------|-------|
| Google Chrome | ✅ Fully supported | Manifest V3 |
| Microsoft Edge | ✅ Fully supported | Manifest V3 |
| Mozilla Firefox | ✅ Fully supported | Manifest V3, Firefox 140+ (desktop) |
| Brave | ✅ Supported | Chromium |
| Opera | ✅ Supported | Chromium |
| Vivaldi | ✅ Supported | Chromium |
| Any Chromium-based browser | ✅ Supported | Manifest V3 |

> **Firefox differences:**
> - Full-page capture on Firefox is produced by scrolling and stitching inside the page instead of Chrome's DevTools Protocol, so PageShot asks for **no `debugger` or `offscreen` permission** on Firefox — only `activeTab`, `contextMenus`, `downloads`, `storage`, `scripting` and `clipboardWrite`.
> - Firefox reserves `Ctrl+Shift+S` for its built-in Screenshot tool. If a PageShot shortcut does not fire, reassign it in *Add-ons Manager → PageShot → Options → Manage Extension Shortcuts* (or `about:addons`).
> - Everything else — visible-area capture, selection capture, copy, PNG download, all annotations, mosaic blur and PDF export — works the same as on Chrome and Edge.

---

## Installation

| Store | Link |
|---|---|
| Chrome Web Store | [Install for Chrome](https://chromewebstore.google.com/detail/jonikcknondlhibmemapljjodhjikcje) |
| Microsoft Edge Add-ons | [Install for Edge](https://microsoftedge.microsoft.com/addons/detail/pooedlcmpdgcfkjfojhblenegbhhahmd) |
| Firefox Add-ons (AMO) | 🔜 Under review — link will be added once the listing is live |

> Install only from the official stores above — avoid third-party download sites.

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
3. Use the **Rectangle**, **Ellipse**, **Arrow**, **Text** or **Mosaic** tools from the toolbar
4. Pick a color (for shapes and text)
5. Click **📋 Copy** or **💾 Download** when done

---

## Context Menu Structure

- Capture Visible Area
- Capture Full Page
- Capture Selection

---

## Privacy

PageShot is built with privacy as a core principle:

- ✅ **Zero data upload** — All screenshot processing happens locally
- ✅ **No analytics** — No tracking, no telemetry, no remote calls apart from optional license validation
- ✅ **No cookies** — No reading or writing of browser cookies
- ✅ **No browsing history** — No access to your browsing data
- ✅ **Local editing storage** — The five most recent captures stay in your browser for the annotation editor and older ones are pruned automatically; nothing is uploaded
- ✅ **Minimal permissions** — Only requests what's strictly necessary

---

## How It Works

1. Start a capture from the right-click menu, a keyboard shortcut, or the popup.
2. Choose what to grab: the visible area, the whole page, or a region you select.
3. The image is cropped and processed entirely inside your browser.
4. A notification offers Copy, Download, or Edit.

---

## Permissions

| Permission | Purpose | Platforms |
|-----------|---------|-----------|
| `activeTab` | Access the current tab when you trigger a capture | All |
| `contextMenus` | Add right-click menu options | All |
| `downloads` | Save screenshots to your computer | All |
| `clipboardWrite` | Copy screenshots to your clipboard | All |
| `scripting` | Inject the selection overlay on web pages | All |
| `storage` | Save your preferences locally | All |
| `offscreen` | Process images in the background | Chrome / Edge only |
| `tabs` | Get tab info for capture coordination | Chrome / Edge only |
| `debugger` | Required for full-page screenshot stitching on certain Chromium builds | Chrome / Edge only |

On Firefox the extension requests only the first six (`activeTab`, `contextMenus`, `downloads`, `clipboardWrite`, `scripting`, `storage`) plus access to `https://api.annmax1983.com/*` for optional licence checks. Firefox never sees a `debugger` warning because that permission is not declared in the Firefox build.

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

> **Note:** This repository is a project showcase. The full source code is not published here.

