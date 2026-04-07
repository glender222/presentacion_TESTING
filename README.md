# Presentación del Proyecto DCCAPA (Slidev)

Este repositorio contiene la presentación para la automatización de mensajería (teoría de colas) construida utilizando **Slidev** (un creador de presentaciones para desarrolladores).

## 🛠️ Requisitos Previos

Antes de poder abrir o compilar la presentación, asegúrate de tener descargado e instalado lo siguiente:

1. **[Node.js](https://nodejs.org/es)** (Versión 18 o superior).  
   *Nota: Al instalar Node.js, y para comprobar que se ha instalado correctamente, puedes abrir tu terminal y ejecutar `node -v` y `npm -v`.*

---

## 🚀 ¿Cómo levantar la presentación localmente?

Si solo quieres ver la presentación en tu computadora para ensayar o enseñarla por videollamada, puedes ejecutar el servidor en vivo:

**Opción 1: Usando npx (descarga temporal al vuelo):**
```bash
npx @slidev/cli presentacion-proyecto-slidev.md --open
```

**Opción 2: Instalando Slidev globalmente en tu PC (Recomendado si lo usarás seguido):**
```bash
npm install -g @slidev/cli
slidev presentacion-proyecto-slidev.md
```

Ambos comandos abrirán una pestaña en tu navegador web automáticamente.

---

## 📦 Construir la versión estable para Web

Si deseas alojar la presentación en **GitHub Pages**, **Vercel** o cualquier hosting, debes compilar los archivos estáticos HTML/JS.

```bash
npx @slidev/cli build presentacion-proyecto-slidev.md
```
*Esto generará una carpeta llamada `dist/`. El contenido dentro de `dist/` es tu página web lista para subirse a cualquier servidor.*

---

## 📄 Descargar la presentación como PDF

Si la universidad o el profesor te pide el archivo obligatoriamente en formato `.pdf`, usa este comando:

```bash
npx @slidev/cli export presentacion-proyecto-slidev.md
```
*Tip: La primera vez que lo corras, puede que se te descargue una herramienta de Google Chrome automatizada (`playwright`), dale a aceptar (y/yes).*
# presentacion_TESTING
