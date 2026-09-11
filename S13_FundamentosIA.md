---
title: Sesión 13 · Cómo funciona la IA
---
# Sesión 13 · Cómo funciona la IA (jugando) 🧠🎮

> *"Hoy entrenas tu propia IA en 10 minutos y ves por dentro cómo un modelo de lenguaje elige la siguiente palabra."*

## 🧰 Herramientas del día

| Herramienta | Para qué la usamos hoy | Enlace | Costo |
|---|---|---|---|
| **Teachable Machine** | Entrenar un clasificador de imágenes/sonidos/poses con tu cámara | [teachablemachine.withgoogle.com](https://teachablemachine.withgoogle.com) | Gratis |
| **Transformer Explainer** | Ver un GPT por dentro, token a token | [poloclub.github.io/transformer-explainer](https://poloclub.github.io/transformer-explainer/) | Gratis |
| **Tiktokenizer** | Ver cómo el texto se convierte en tokens | [tiktokenizer.vercel.app](https://tiktokenizer.vercel.app) | Gratis |
| **Google AI Studio** | Jugar con temperatura, instrucciones de sistema, modelos y **herramientas** (búsqueda, código) | [aistudio.google.com](https://aistudio.google.com) | Gratis |
| **Semantris** | Juego de asociación de palabras con IA (embeddings) | [research.google.com/semantris](https://research.google.com/semantris/) | Gratis |
| **Survival of the Best Fit** (repaso) | Sesgo en el entrenamiento | [survivalofthebestfit.com](https://www.survivalofthebestfit.com) | Gratis |

## 🎯 Objetivos

* Explicar con tus palabras: **datos → entrenamiento → modelo → predicción**, y qué es el sesgo.
* Distinguir IA clásica, aprendizaje automático, aprendizaje profundo e IA generativa.
* Entender **tokens, embeddings, atención, temperatura** viéndolos en simuladores.
* Entrenar tu propio modelo y usarlo desde una página web.
* Dar a un modelo **herramientas** (búsqueda, ejecución de código): el paso previo a un agente.

```{admonition} Cobertura PIIA
:class: note
Unidad 5 · a. Fundamentos de IA · b. Herramientas esenciales de IA generativa · Unidad 1 · h. Tecnologías emergentes.
```

## ⏱️ Agenda (2h30)

| Tiempo | Bloque | Qué pasa |
|---|---|---|
| 0:00 – 0:15 | 🎨 **Quick, Draw! visto por dentro** | ¿De dónde aprendió? De 50 millones de dibujos. Datos → modelo. Semantris: palabras que "están cerca" (embeddings) |
| 0:15 – 0:50 | 📷 **Actividad 1: Entrena tu IA** | Teachable Machine con tus 30 fotos |
| 0:50 – 1:15 | 🔤 **Un LLM por dentro** | Tiktokenizer (¿cuántos tokens tiene tu nombre?), Transformer Explainer (la siguiente palabra es una probabilidad), temperatura en AI Studio |
| 1:15 – 1:25 | ☕ Pausa | |
| 1:25 – 1:50 | 🗺️ **Mapa de la IA** | IA clásica vs ML vs deep learning vs generativa. Qué es un modelo, qué es un dataset, qué es un sesgo. Alucinación explicada con lo que vieron |
| 1:50 – 2:20 | 🛠️ **Actividad 2: Dale herramientas a tu modelo** | AI Studio: sistema + búsqueda + código. Primer "agente con herramientas" |
| 2:20 – 2:30 | 🏠 Cierre y reto | |

## 📷 Actividad 1: Entrena tu IA (35 min)

1. [Teachable Machine](https://teachablemachine.withgoogle.com) → *Proyecto de imagen* (o *pose* si eres de deporte, *audio* si eres de artes/música).
2. Clase 1 y Clase 2: sube tus 30 fotos o toma 30 con la cámara de cada una (dos especies, dos posturas, dos estilos, dos tipos de documento).
3. *Entrenar modelo* (1 minuto). Prueba en vivo.
4. **Rómpelo:** muéstrale algo que no es ninguna de las dos clases. ¿Qué pasa? ¿Por qué? (Solo sabe lo que le enseñaste.)
5. **Sesgo a propósito:** entrena de nuevo con todas las fotos de la clase 1 con fondo blanco y de la clase 2 con fondo oscuro. Ahora muéstrale un fondo blanco vacío. Eso es un sesgo del dataset.
6. *Exportar modelo → Subir (link compartible)*. Pídele a Claude: *"Hazme una página HTML que use este modelo de Teachable Machine [URL] con la cámara y muestre la predicción en grande."* Súbela a tu página web.

## 🔤 Un LLM por dentro (lo mínimo que hay que saber)

| Concepto | Qué es | Dónde lo ves |
|---|---|---|
| **Token** | El trozo de texto con el que trabaja el modelo (≈ ¾ de palabra) | Tiktokenizer |
| **Embedding** | El "lugar" de cada token en un espacio donde lo parecido está cerca | Semantris |
| **Atención** | Qué tokens mira el modelo para predecir el siguiente | Transformer Explainer |
| **Predicción** | El modelo no "sabe": calcula la probabilidad de la siguiente palabra | Transformer Explainer |
| **Temperatura** | Cuánto azar se permite al elegir: 0 = siempre la más probable, 1+ = creativo/caótico | AI Studio |
| **Ventana de contexto** | Cuánto texto cabe en una conversación; por eso NotebookLM "cita" y no "recuerda" | AI Studio (contador de tokens) |
| **Alucinación** | Una predicción fluida pero falsa: ahora entiendes por qué no es "mentira" | Sesión 5 |

## 🛠️ Actividad 2: Dale herramientas a tu modelo (30 min)

En [AI Studio](https://aistudio.google.com):

1. *System instructions*: pega las instrucciones de tu Gem (S4).
2. Pregunta algo de actualidad: *"¿Qué pasó esta semana en [tu área] en Colombia?"* → responde vagamente o inventa.
3. Activa la herramienta **Grounding con Google Search** y repite: ahora busca y cita.
4. Activa **Code execution** y pide: *"Calcula el IMC promedio de estos 10 atletas: [datos]"* → escribe y ejecuta código para responder.
5. Observa: instrucciones + modelo + **herramientas** + tu pregunta = **agente**. La próxima sesión lo soltamos sobre tus archivos.
6. *Get API key*: genera y guarda tu clave gratuita en Bitwarden (la usarás en la S15). **Nunca la pegues en un chat ni la subas a tu página.**

```{admonition} Ruta pro 🧗
:class: tip
En AI Studio → *Build* describe una app: *"Una app que recibe una foto de una planta/lesión/obra y devuelve una ficha con 5 campos"*. AI Studio la programa y la despliega. También puedes ver el **Stream** (voz + cámara en tiempo real) y pensar qué harías con eso en tu profesión.
```

## 📦 Entregable

Enlace a tu modelo de Teachable Machine + página que lo usa + captura de AI Studio con búsqueda activada respondiendo con fuentes.

## 🏠 Reto para la casa (~3h)

1. Instala **Node.js** y **Gemini CLI** (ver {doc}`KitDeCuentas`). Verifica que `gemini` abre en tu terminal. Si tienes problemas, trae el error en captura: lo resolvemos al inicio de la próxima clase.
2. Crea una carpeta `agente/` con **10–20 archivos reales desordenados** de tu carrera: PDFs, imágenes, documentos, hojas de cálculo, con nombres malos (`Documento1.pdf`, `IMG_2034.jpg`).
3. Escribe en 3 líneas **una tarea repetitiva** que haces con archivos y que te gustaría delegar.
