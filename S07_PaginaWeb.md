---
title: Sesión 7 · Tu página web
---
# Sesión 7 · Tu página web, publicada hoy 🌐

> *"Al final de esta clase vas a tener una URL con tu nombre que puedes mandar por WhatsApp."*

## 🧰 Herramientas del día

| Herramienta | Para qué la usamos hoy | Enlace | Costo |
|---|---|---|---|
| **Google Sites** | Página web sin código, en 20 minutos, con tu cuenta institucional | [sites.google.com](https://sites.google.com) | Gratis |
| **Lovable** / **Bolt.new** | *Vibe coding*: describes la página y la IA la programa | [lovable.dev](https://lovable.dev) · [bolt.new](https://bolt.new) | Gratis (créditos diarios) |
| **Claude Artifacts** / **Gemini Canvas** | Crear una página o juego interactivo desde el chat | [claude.ai](https://claude.ai) · [gemini.google.com](https://gemini.google.com) | Gratis |
| **GitHub Pages** / **Netlify Drop** | Publicar un archivo HTML en internet gratis | [pages.github.com](https://pages.github.com) · [app.netlify.com/drop](https://app.netlify.com/drop) | Gratis |
| **Google Stitch** | Diseñar la interfaz con IA antes de construir | [stitch.withgoogle.com](https://stitch.withgoogle.com) | Gratis |

## 🎯 Objetivos

* Entender **cómo funciona la web**: dominio, servidor, HTML/CSS/JS, hosting (en 15 minutos y con un juego).
* Publicar una página en **Google Sites** (ruta segura) y una con **vibe coding** (ruta IA).
* Convertir la página en tu **portafolio del curso**.
* Saber cuándo conviene sin código, cuándo IA, cuándo un desarrollador.

```{admonition} Cobertura PIIA
:class: note
Unidad 3 · c.i.iii. Sitios web/blogs · b. Redes sociales y redes temáticas (tu presencia digital) · Unidad 5 · c. Aplicaciones en habilidades profesionales.
```

## ⏱️ Agenda (2h30)

| Tiempo | Bloque | Qué pasa |
|---|---|---|
| 0:00 – 0:15 | 🕸️ **¿Cómo funciona la web?** | Juego: "la carta que viaja". Dominio → DNS → servidor → HTML. Ver el código fuente de una página real (clic derecho → Inspeccionar) y cambiar el titular de un periódico en vivo |
| 0:15 – 0:45 | 🏗️ **Actividad 1: Google Sites en 30 min** | Antes, 5 min: cada uno busca 2 páginas que le gusten y una foto suya. Luego: inicio, sobre mí, portafolio (lo del Ejercicio 1) y contacto. Publicar |
| 0:45 – 1:15 | ✨ **Actividad 2: Vibe coding** | Lovable / Claude: la misma página, pero descrita en lenguaje natural |
| 1:15 – 1:25 | ☕ Pausa | |
| 1:25 – 1:55 | 🚀 **Actividad 3: Publicar el HTML** | Descargar el código generado y subirlo a Netlify Drop o GitHub Pages. Tu segunda URL |
| 1:55 – 2:15 | 🎮 **Actividad 4: Un juego para tu carrera** | Claude Artifacts: quiz, memoria, simulador simple. Enlazarlo desde tu página |
| 2:15 – 2:30 | 🗳️ **Galería y cierre** | Cada uno pega su URL en el tablero compartido. Votación: mejor diseño, mejor contenido |

## 🏗️ Actividad 1: Google Sites (30 min)

1. [sites.google.com](https://sites.google.com) → *Nuevo sitio* → plantilla *Portafolio* o en blanco.
2. Secciones mínimas: **Inicio** (foto + una frase), **Sobre mí**, **Portafolio** (enlaza tu cuaderno NotebookLM, tu Gem, tu informe, tu manifiesto), **Contacto**.
3. Pide a Gemini el texto de "Sobre mí" en 3 tonos (formal, cercano, creativo) y elige uno.
4. *Publicar* → nombre `tunombre-carrera` → copia la URL.

## ✨ Actividad 2: Vibe coding (30 min)

En **Lovable** (o Bolt), escribe un prompt con la anatomía de la Sesión 4:

> *"Crea una página personal para [nombre], estudiante de [carrera] en Manizales. Secciones: hero con mi nombre y una frase, sobre mí, portafolio con 4 tarjetas (título, descripción, botón), contacto. Estilo: minimalista, colores [tus colores], tipografía legible, en español, responsive (que se vea bien en celular). No uses lorem ipsum: inventa textos plausibles que luego voy a reemplazar."*

Itera 3 veces: "cambia los colores", "agrega una sección de habilidades con barras", "haz el menú fijo arriba". Observa qué hace la IA: está **escribiendo código** por ti. Lo verás en la pestaña de código.

## 🚀 Actividad 3: Publicar el HTML (30 min)

Ruta fácil: descarga el HTML (o pide a Claude *"dame todo en un solo archivo `index.html`"*), arrástralo a [Netlify Drop](https://app.netlify.com/drop) → URL pública en 10 segundos.

Ruta GitHub (recomendada, sirve para todo el curso): crea un repositorio `tunombre.github.io`, sube `index.html`, *Settings → Pages* → tu página en `https://tunombre.github.io`.

```{admonition} Ruta pro 🧗
:class: tip
Abre la terminal en la carpeta del `index.html` y corre `gemini` o `claude`. Pide: *"Agrega un modo oscuro con un botón y haz que la sección de portafolio lea las tarjetas desde un archivo `proyectos.json`."* Mira los archivos cambiar. Eso es un **agente de código** trabajando en tu disco. Luego `git add . && git commit -m "modo oscuro" && git push` y tu página se actualiza sola.
```

## 🎮 Actividad 4: Un juego para tu carrera (20 min)

En Claude: *"Crea un juego interactivo de [memoria / quiz / arrastrar y soltar] sobre [tema de tu carrera], con 10 preguntas, puntaje, y feedback por respuesta. En español."* Prueba, itera, publica el artefacto o descarga el HTML y súbelo a tu página.

## 📦 Lo que te llevas

Dos URLs (Sites + vibe coding/Pages) en el tablero del curso. Desde hoy, **todo lo que construyas se publica en tu página**: es la base del **Ejercicio 2**.
