# PageShot

[English](../README.md) | [中文](README_zh.md) | Español | [Deutsch](README_de.md) | [日本語](README_ja.md) | [Français](README_fr.md)

Una extensión ligera para el navegador que captura capturas de pantalla — página completa, área visible o cualquier selección. Sin marca de agua forzada, procesamiento completamente local.

> Basada en Chromium · Manifest V3 · Sin rastreo · Procesamiento completo en el navegador

---

## ¿Por qué PageShot?

La mayoría de herramientas de captura de pantalla cobran por la captura de página completa, añaden marcas de agua o suben tus datos a servidores remotos. PageShot hace todo dentro de tu navegador — tus datos nunca salen de tu máquina.

| Ventaja | Detalle |
|---------|--------|
| 🔒 **Privacidad ante todo** | Todo el procesamiento ocurre localmente. Sin servidores, sin subidas, sin rastreo. |
| 💧 **Sin marca de agua** | Capturas limpias, sin branding impuesto en tus capturas. |
| 🆓 **Sin marcas de agua forzadas en las imágenes capturadas. |
| 📄 **Captura de página completa** | Captura larga con un clic — se desplaza y une automáticamente. |
| 📋 **Copiar y pegar** | Copia al portapapeles al instante — pega directamente en chats, correos y documentos. |
| ✏️ **Anotación integrada** | Dibuja rectángulos y desenfoque mosaico antes de compartir. |
| ⚡ **Ligera** | Sin frameworks, sin peso muerto. |
| 🌍 **6 idiomas** | Detecta automáticamente el idioma de tu navegador. |

---

## Funcionalidades

### 🆓 Funcionalidades gratuitas

| Funcionalidad | Descripción |
|---------|-------------|
| 📄 **Captura de página completa** | Captura toda la página desplazable en una sola toma mediante Chrome DevTools Protocol. Gestiona imágenes de carga diferida y páginas muy largas. |
| 👁 **Captura del área visible** | Captura instantánea de lo que hay actualmente en pantalla. La forma más rápida de hacer una captura. |
| ✂️ **Captura por selección** | Arrastra para seleccionar cualquier región de la página con una superposición de punto de mira. Precisa y flexible. |
| 📋 **Copiar al portapapeles** | Copia con un clic después de la captura. Pega directamente en cualquier aplicación con Ctrl+V. |
| 💾 **Descargar como PNG** | Nombra automáticamente los archivos con el título de la página + fecha (ej. `GitHub_-_Homepage_2026-07-07.png`). |
| ✏️ **Anotación con rectángulos** | Dibuja rectángulos de colores para resaltar áreas. 5 colores disponibles: rojo, azul, verde, negro, blanco. |
| 🟦 **Desenfoque mosaico** | Pixela contenido sensible — contraseñas, información personal, mensajes privados. |
| ⌨️ **Atajos de teclado** | `Ctrl+Shift+V` — Captura visible + copiar · `Ctrl+Shift+F` — Página completa + descargar · `Ctrl+Shift+S` — Modo selección. |
| 🔤 **i18n en 6 idiomas** | La interfaz se adapta automáticamente al idioma de tu navegador: English, 中文, 日本語, Español, Deutsch, Français. |
| 🔒 **Gestión de elementos fijos** | Detecta y elimina automáticamente encabezados/pies de página fijos de las capturas largas. |

### ⭐ Funcionalidades Premium (requieren licencia)

| Funcionalidad | Descripción |
|---------|-------------|
| 📑 **Exportar como PDF** | Exporta cualquier captura (incluidas páginas largas) como documento PDF — desde el editor de anotaciones |
| 💬 **Soporte prioritario** | Soporte prioritario por correo electrónico para usuarios Premium |

### Gratis vs Premium

| | Gratis | Premium |
|---|:---:|:---:|
| Captura de página completa / visible / selección | ✅ | ✅ |
| Copiar al portapapeles y descargar como PNG | ✅ | ✅ |
| Anotación con rectángulos y desenfoque mosaico | ✅ | ✅ |
| Atajos de teclado | ✅ | ✅ |
| Gestión de elementos fijos | ✅ | ✅ |
| Exportar como PDF | — | ✅ |
| Soporte prioritario | — | ✅ |

---

## Vista previa

<p align="center">
  <img src="icons/icon128.png" alt="Icono de PageShot" width="80">
</p>

---

## Navegadores compatibles

| Navegador | Estado |
|---------|--------|
| Google Chrome | ✅ Totalmente compatible |
| Microsoft Edge | ✅ Totalmente compatible |
| Brave | ✅ Compatible |
| Opera | ✅ Compatible |
| Vivaldi | ✅ Compatible |
| Cualquier navegador basado en Chromium | ✅ Compatible (Manifest V3) |

---

## Instalación

### Desde código fuente (modo desarrollador)

1. Abre la página de extensiones de tu navegador:
   - **Chrome**: `chrome://extensions/`
   - **Edge**: `edge://extensions/`
2. Activa el **modo de desarrollador** (interruptor arriba a la derecha)
3. Haz clic en **Cargar descomprimida** y selecciona la carpeta `page-shot`
4. El icono de PageShot aparecerá en tu barra de herramientas

---

## Uso

### Captura por clic derecho

1. Haz clic derecho en cualquier lugar de una página web
2. Selecciona **PageShot** en el menú contextual
3. Elige: **Capturar área visible**, **Capturar página completa** o **Capturar selección**
4. Aparece una notificación emergente con los botones **Copiar**, **Descargar** y **Editar**

### Atajos de teclado

| Atajo | Acción |
|----------|--------|
| `Ctrl+Shift+V` | Capturar área visible → copiar al portapapeles |
| `Ctrl+Shift+F` | Capturar página completa → descargar como PNG |
| `Ctrl+Shift+S` | Entrar en modo selección |

### Anotación

1. Después de capturar, haz clic en **✏️ Editar** en la notificación emergente
2. El editor de anotaciones se abre en una nueva pestaña
3. Usa las herramientas **Rectángulo** o **Mosaico** de la barra de herramientas
4. Elige un color (para rectángulos)
5. Haz clic en **📋 Copiar** o **💾 Descargar** cuando termines

---

## Estructura del menú contextual

```
PageShot
├── Capturar área visible
├── Capturar página completa
└── Capturar selección
```

---

## Privacidad

PageShot está construida con la privacidad como principio fundamental:

- ✅ **Cero subida de datos** — Todo el procesamiento de capturas ocurre localmente
- ✅ **Sin analíticas** — Sin rastreo, sin telemetría, sin llamadas remotas
- ✅ **Sin cookies** — Sin lectura ni escritura de cookies del navegador
- ✅ **Sin historial de navegación** — Sin acceso a tus datos de navegación
- ✅ **Solo almacenamiento temporal** — Las capturas existen brevemente durante el procesamiento y luego se borran
- ✅ **Permisos mínimos** — Solo solicita lo estrictamente necesario

---

## Cómo funciona

```
Activación (clic derecho / atajo / popup)
       ↓
El Service Worker coordina la captura
       ↓
┌─ Área visible: chrome.tabs.captureVisibleTab()
├─ Página completa: expande el viewport vía CDP → una sola captura en alta resolución
└─ Selección: captura visible → recorte al rectángulo seleccionado
       ↓
El Offscreen Document procesa la imagen (recorte / portapapeles)
       ↓
Notificación emergente con acciones Copiar / Descargar / Editar
```

> **¿Por qué Offscreen?** El Manifest V3 de Chrome ejecuta el fondo como un Service Worker sin acceso al DOM. La Canvas API requiere un DOM, así que usamos la Offscreen API de Chrome para el procesamiento de imágenes.

---

## Permisos

| Permiso | Propósito |
|-----------|---------|
| `activeTab` | Acceder a la pestaña actual cuando activas una captura |
| `contextMenus` | Añadir opciones al menú de clic derecho |
| `downloads` | Guardar capturas de pantalla en tu ordenador |
| `clipboardWrite` | Copiar capturas de pantalla a tu portapapeles |
| `scripting` | Inyectar la superposición de selección en páginas web |
| `storage` | Guardar tus preferencias localmente |
| `offscreen` | Procesar imágenes en segundo plano |
| `tabs` | Obtener información de pestañas para la coordinación de capturas |
| `debugger` | Necesario para la unión de capturas de página completa en ciertas compilaciones de Chromium |

---

## Aviso de derechos de autor

Esta herramienta de captura de pantalla es solo para el uso personal del usuario en aprendizaje, organización de documentos y grabación de contenido sin conexión. Todo el texto, las imágenes y el contenido multimedia de las páginas web pertenecen al propietario original de los derechos de autor. Los usuarios no deberían utilizar las capturas para reproducción comercial, reimpresión no autorizada, distribución pública u otros comportamientos que infrinjan los derechos de autor. Toda responsabilidad legal derivada del uso indebido recaerá exclusivamente sobre el usuario.

---

## Licencia

Copyright © 2026 PageShot. Todos los derechos reservados.

---

## ❤️ Apoyo

Si te resulta útil PageShot, ¡considera apoyar el proyecto!

**[👉 Haz clic aquí para apoyar](https://ko-fi.com/annmax?ref=pageshot)**
