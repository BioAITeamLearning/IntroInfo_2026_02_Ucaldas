---
title: Sesión 7 · Tu página web
---
# Sesión 7 · Tu página web, publicada hoy 🌐

> *"Al final de esta clase vas a tener una URL con tu nombre que puedes mandar por WhatsApp."*

## 🧰 Herramientas del día

| Herramienta | Para qué la usamos hoy | Enlace | Costo |
|---|---|---|---|
| **Google Sites** | Página web sin código, con tu cuenta institucional | [sites.google.com](https://sites.google.com) | Gratis |
| **Lovable** / **Bolt.new** | *Vibe coding*: describes la página y la IA la programa | [lovable.dev](https://lovable.dev) · [bolt.new](https://bolt.new) | Gratis (créditos diarios) |
| **Claude Artifacts** / **Gemini Canvas** | Crear una página o juego interactivo desde el chat | [claude.ai](https://claude.ai) · [gemini.google.com](https://gemini.google.com) | Gratis |
| **GitHub Pages** / **Netlify Drop** | Publicar un archivo HTML en internet gratis | [pages.github.com](https://pages.github.com) · [app.netlify.com/drop](https://app.netlify.com/drop) | Gratis |
| **Google Stitch** | Diseñar la interfaz con IA antes de construir | [stitch.withgoogle.com](https://stitch.withgoogle.com) | Gratis |

## 🎯 Objetivos

* Entender **cómo funciona la web**: dominio, servidor, HTML/CSS/JS, hosting.
* Publicar una página en **Google Sites** (ruta segura) y una con **vibe coding** (ruta IA).
* Convertir la página en tu **portafolio del curso**.
* Saber cuándo conviene sin código, cuándo IA, cuándo un desarrollador.

## 🏗️ Actividad 1: Google Sites

1. [sites.google.com](https://sites.google.com) → *Nuevo sitio* → plantilla *Portafolio* o en blanco.
2. Secciones mínimas: **Inicio** (foto + una frase), **Sobre mí**, **Portafolio** (enlaza tu cuaderno NotebookLM, tu Gem, tu informe, tu manifiesto), **Contacto**.
3. Pide a Gemini el texto de "Sobre mí" en 3 tonos (formal, cercano, creativo) y elige uno.
4. *Publicar* → nombre `tunombre-carrera` → copia la URL.

## ✨ Actividad 2: Vibe coding

En **Lovable** (o Bolt), escribe un prompt con la anatomía de la Sesión 4:

> *"Crea una página personal para [nombre], estudiante de [carrera] en Manizales. Secciones: hero con mi nombre y una frase, sobre mí, portafolio con 4 tarjetas (título, descripción, botón), contacto. Estilo: minimalista, colores [tus colores], tipografía legible, en español, responsive (que se vea bien en celular). No uses lorem ipsum: inventa textos plausibles que luego voy a reemplazar."*

Itera 3 veces: "cambia los colores", "agrega una sección de habilidades con barras", "haz el menú fijo arriba". Observa qué hace la IA: está **escribiendo código** por ti. Lo verás en la pestaña de código.

## 🚀 Actividad 3: Publicar el HTML

Ruta fácil: descarga el HTML (o pide a Claude *"dame todo en un solo archivo `index.html`"*), arrástralo a [Netlify Drop](https://app.netlify.com/drop) → URL pública en 10 segundos.

Ruta GitHub (recomendada, sirve para todo el curso): crea un repositorio `tunombre.github.io`, sube `index.html`, *Settings → Pages* → tu página en `https://tunombre.github.io`.

```{admonition} Ruta pro 🧗
:class: tip
Abre la terminal en la carpeta del `index.html` y corre `gemini` o `claude`. Pide: *"Agrega un modo oscuro con un botón y haz que la sección de portafolio lea las tarjetas desde un archivo `proyectos.json`."* Mira los archivos cambiar. Eso es un **agente de código** trabajando en tu disco. Luego `git add . && git commit -m "modo oscuro" && git push` y tu página se actualiza sola.
```

## 🎮 Actividad 4: Un juego para tu carrera

En Claude: *"Crea un juego interactivo de [memoria / quiz / arrastrar y soltar] sobre [tema de tu carrera], con 10 preguntas, puntaje, y feedback por respuesta. En español."* Prueba, itera, publica el artefacto o descarga el HTML y súbelo a tu página.

## 📦 Lo que te llevas

Dos URLs (Sites + vibe coding/Pages) en el tablero del curso. Desde hoy, **todo lo que construyas se publica en tu página**: es la base del **Ejercicio 2**.
