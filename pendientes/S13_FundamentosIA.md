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

## 📷 Actividad 1: Entrena tu IA

1. [Teachable Machine](https://teachablemachine.withgoogle.com) → *Proyecto de imagen* (o *pose* si eres de deporte, *audio* si eres de artes/música).
2. Clase 1 y Clase 2: toma **30 fotos con la cámara** de cada una (dos objetos del salón, dos posturas, dos gestos, dos tipos de documento; o busca 30 imágenes de dos especies/estilos en Google Imágenes y súbelas).
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

## 🛠️ Actividad 2: Dale herramientas a tu modelo

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

## 📦 Lo que te llevas

Enlace a tu modelo de Teachable Machine + página que lo usa + captura de AI Studio con búsqueda activada respondiendo con fuentes.
