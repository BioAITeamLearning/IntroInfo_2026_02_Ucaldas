---
title: Sesión 2 · Tu kit de superpoderes
---
# Sesión 2 · Tu nuevo kit de superpoderes 🦸

> *"La clase pasada vimos de qué está hecho un computador. Hoy vemos de qué eres capaz tú con uno."*

## 🧰 Herramientas del día

| Herramienta | Para qué la usamos hoy | Enlace | Costo |
|---|---|---|---|
| **Gemini** | Asistente general: texto, imágenes, voz, cámara en vivo | [gemini.google.com](https://gemini.google.com) | Gratis (cuenta institucional) |
| **NotebookLM** | Convertir tus documentos en podcast, mapa mental, quiz | [notebooklm.google.com](https://notebooklm.google.com) | Gratis |
| **Quick, Draw!** | Juego: la IA adivina lo que dibujas | [quickdraw.withgoogle.com](https://quickdraw.withgoogle.com) | Gratis |
| **Claude** (demo) | Crear un juego o app describiéndola | [claude.ai](https://claude.ai) | Gratis |

## 🎯 Objetivos

* Entender en 15 minutos **qué es la IA**, cómo aprende de ejemplos, por qué a veces inventa y quién es quién en 2026.
* Ver en vivo **10 cosas que la IA puede hacer hoy** por un biólogo, un abogado, un artista o un deportólogo.
* Comparar distintos asistentes de IA con el mismo problema y entender que **no todos sirven para lo mismo**.
* Convertir un documento real de tu carrera en un **podcast, un mapa mental y un quiz** en menos de 10 minutos.
* Conocer el mapa del curso: todo lo que vas a construir en 16 semanas.

```{admonition} Cobertura PIIA
:class: note
Unidad 1 · h. Tecnologías emergentes (IA generativa, sistemas interactivos) · b. Estructura y aplicaciones · g. Software para texto y presentaciones (con Gemini en Docs/Slides) · Unidad 5 · a. Fundamentos de IA (introducción; se profundiza en la Sesión 13).
```

## ⏱️ Agenda (2h30)

| Tiempo | Bloque | Qué pasa |
|---|---|---|
| 0:00 – 0:10 | 🎮 **Calentamiento: Quick, Draw!** | En parejas, uno dibuja y la IA adivina. Pregunta detonante: *¿cómo sabe la IA lo que dibujaste?* |
| 0:10 – 0:25 | 🧠 **¿Qué es la IA?** (micro-intro) | De Quick Draw a ChatGPT en 15 minutos: qué es, cómo aprende, por qué inventa, quién es quién. Ver sección abajo |
| 0:25 – 0:45 | 🎩 **Tour de 10 superpoderes** (demo en vivo) | Ver tabla abajo. Dos minutos por demo, sin teoría, solo *wow* |
| 0:45 – 0:55 | 🗺️ **El mapa del curso y las reglas** | Recorremos {doc}`MapaDelCurso`: "todo esto lo van a hacer ustedes". Tres ejercicios, tres notas |
| 0:55 – 1:05 | 🎒 **Kit check** | Todos entran a Gemini y NotebookLM con el correo institucional y crean cuenta en Claude y Perplexity ({doc}`KitDeCuentas`) |
| 1:05 – 1:25 | 🤝 **Actividad 1: Speed dating con IAs** | Equipos base por carrera, mismo reto en 4 asistentes distintos |
| 1:25 – 1:35 | ☕ Pausa | |
| 1:35 – 2:10 | 🎧 **Actividad 2: Tu carrera en un podcast** | Buscar un documento real de tu carrera y convertirlo en NotebookLM |
| 2:10 – 2:25 | 🗣️ **Puesta en común** | Cada equipo pone 30 segundos de su podcast. Votamos el mejor |
| 2:25 – 2:30 | 🏁 Cierre | Qué construimos hoy y cómo se conecta con el Ejercicio 1 |

```{admonition} Material del docente 📽️
:class: tip
* <a href="_static/sesion02/slides.html" target="_blank">Diapositivas de la sesión</a> (flechas para avanzar, `F` pantalla completa, `N` notas del docente, `T` cronómetro).
* <a href="_static/sesion02/tarjetas.html" target="_blank">Tarjetas para imprimir</a>: una por equipo con el reto de su carrera y la tabla de speed dating, más la guía del podcast por estudiante.
* El guion con los prompts exactos de cada demo está al final de esta página.
```

## 🧠 ¿Qué es la IA? (lo mínimo, en 15 minutos)

Arrancamos desde lo que acaban de vivir: Quick Draw adivinó sus dibujos porque **le mostraron 50 millones de dibujos de otras personas**. Nadie le explicó qué es un gato. Esa es la idea central de la IA moderna: **aprender de ejemplos, no de reglas**.

### Una historia en 8 fechas

| Año | Qué pasó | Por qué importa |
|---|---|---|
| 1950 | Alan Turing pregunta: *¿pueden pensar las máquinas?* | Nace la pregunta (y el "test de Turing") |
| 1956 | Se inventa el término *inteligencia artificial* (Dartmouth) | Décadas de IA basada en **reglas** escritas a mano |
| 1997 | Deep Blue le gana a Kasparov en ajedrez | Fuerza bruta + reglas: impresionante, pero solo sabe ajedrez |
| 2012 | Una red neuronal profunda "ve" imágenes mejor que todo lo anterior (ImageNet) | Arranca el **deep learning**: aprender de millones de ejemplos |
| 2016 | AlphaGo vence al campeón mundial de Go | Aprende jugando contra sí misma |
| 2017 | Google publica los **Transformers** ("Attention is all you need") | La arquitectura de todos los chats de hoy |
| Nov 2022 | Sale ChatGPT: 100 millones de usuarios en 2 meses | La IA generativa llega a todo el mundo |
| 2024–26 | Modelos multimodales (ven, oyen, hablan) y **agentes** que actúan | Lo que vamos a usar en este curso |

### Las muñecas rusas

```{raw} html
<div style="display:flex;justify-content:center;margin:1rem 0">
<div style="background:#212529;color:#f4f5f7;border-radius:14px;padding:14px 18px;max-width:640px;width:100%">
 <b>Inteligencia artificial</b> · software que hace cosas que creíamos que necesitaban inteligencia humana
 <div style="background:#2f3640;border-radius:12px;padding:12px 16px;margin-top:8px">
  <b>Aprendizaje automático (ML)</b> · aprende de ejemplos en vez de reglas
  <div style="background:#3d4654;border-radius:10px;padding:10px 14px;margin-top:8px">
   <b>Aprendizaje profundo</b> · redes neuronales con muchas capas; ve, oye, lee
   <div style="background:#4c5768;border-radius:8px;padding:8px 12px;margin-top:8px">
    <b>IA generativa</b> · produce texto, imagen, audio, video, código
    <div style="background:#ffc857;color:#212529;border-radius:6px;padding:6px 10px;margin-top:8px">
     <b>LLMs y agentes</b> · Gemini, ChatGPT, Claude… y las herramientas de este curso
    </div>
   </div>
  </div>
 </div>
</div>
</div>
```

### ¿Qué hace un chat de IA por dentro?

Una sola cosa: **predice la siguiente palabra**. Se entrenó leyendo una parte enorme de internet y aprendió qué palabra suele venir después de cuál. Prueba en vivo: *"El Nevado del ___"*, *"Para interponer una tutela se necesita ___"*. De ahí salen sus dos caras:

| Por eso es genial en… | Y por eso… |
|---|---|
| Redactar, resumir, traducir, explicar a distintos niveles, programar, ver imágenes, encontrar patrones | Puede decir algo **falso con total seguridad** ("alucinar"): no sabe, calcula probabilidades |
| Conversar en tu idioma sobre casi cualquier tema | No tiene información de hoy si no **busca**; no conoce tu contexto si no se lo **das** |
| Trabajar 24/7 sin cansarse | No reemplaza tu **criterio profesional**: tú firmas, tú respondes |

### Quién es quién (2026)

| Empresa | Modelo / producto | Lo distintivo |
|---|---|---|
| Google | **Gemini** (+ NotebookLM, AI Studio) | Integrado en Workspace: tu correo institucional ya lo tiene |
| OpenAI | **ChatGPT** | El más conocido; el que arrancó la ola en 2022 |
| Anthropic | **Claude** | Muy bueno para documentos largos y para crear apps desde el chat (Artifacts) |
| Meta, Mistral, DeepSeek | Llama, Mistral, DeepSeek | Modelos **abiertos**: se pueden descargar y correr en tu computador |
| Perplexity | Perplexity | Búsqueda con fuentes citadas |

Todos son primos: misma tecnología (Transformers), distintos datos, reglas y precios. Por eso hoy los vamos a comparar.

### Vocabulario que van a oír todo el semestre

| Palabra | En cristiano |
|---|---|
| **Modelo** | El "cerebro" entrenado (Gemini 2.5, GPT-5, Claude…) |
| **Prompt** | Lo que le escribes. Sesión 4 entera sobre esto |
| **Token** | El pedacito de texto con el que trabaja el modelo (≈ ¾ de palabra) |
| **Alucinación** | Respuesta fluida pero falsa |
| **Multimodal** | Entiende texto, imagen, audio y video a la vez |
| **Agente** | Una IA que además de responder **hace cosas**: busca, ejecuta, escribe archivos |

```{note}
Esto es solo la puerta de entrada. En la **Sesión 13** abrimos un modelo por dentro (tokens, atención, temperatura) y entrenamos uno propio.
```

## 🎩 Tour de 10 superpoderes (demos del docente)

Cada demo dura ~2 minutos. La idea es que vean el resultado, no el proceso. Adaptar los ejemplos a las carreras del grupo.

| # | Superpoder | Herramienta | Ejemplo para el grupo |
|---|---|---|---|
| 1 | **Ver con la cámara** | Gemini Live (celular) | Apuntar la cámara a una planta / un documento legal / una obra y preguntar |
| 2 | **Chatear con un PDF de 200 páginas** | NotebookLM | Subir el Código Civil / una guía clínica / un reglamento deportivo y preguntar |
| 3 | **Convertir un PDF en podcast** | NotebookLM · Audio Overview | El mismo PDF, ahora en una conversación de dos voces en español |
| 4 | **Crear un juego sin programar** | Claude Artifacts | "Hazme un juego de memoria con términos de anatomía" → jugarlo en vivo |
| 5 | **Generar un video** | Gemini (Veo) / Flow | "Un colibrí en cámara lenta sobre un páramo colombiano" |
| 6 | **Analizar una carpeta entera** | Gemini CLI en la terminal | "Lee estos 30 PDFs y dime cuáles hablan de X" (avance de la S14) |
| 7 | **Hacer una app desde una hoja de cálculo** | AppSheet | Inventario del laboratorio → app en el celular en 3 min (avance de la S9) |
| 8 | **Investigar con fuentes** | Gemini Deep Research | Un informe de 10 páginas con citas sobre un tema de la carrera |
| 9 | **Hablar en otro idioma** | Gemini Live / Google Translate cámara | Conversación en inglés con corrección en tiempo real |
| 10 | **Hacer una presentación en 1 minuto** | Gamma / NotebookLM | Del PDF a 8 diapositivas con diseño |

```{tip}
Cierra el tour con la pregunta: **"¿Cuál de estos les gustaría saber hacer?"** y anótalo. Sirve para ajustar los ejemplos de las próximas sesiones.
```

## 🤝 Actividad 1: Speed dating con IAs (20 min)

Hoy se forman los **equipos base** de 3–4 personas **de la misma carrera** (duran todo el semestre). Cada equipo recibe una tarjeta con un reto de su carrera, o escribe uno propio, por ejemplo:

* *Biología:* "Explícame cómo funciona la PCR como si tuviera 12 años y luego dame 3 preguntas de examen."
* *Derecho:* "Resume la Ley 1581 de 2012 (protección de datos) en 5 puntos y dame un ejemplo de incumplimiento."
* *Artes:* "Propón 5 conceptos para una exposición sobre memoria y territorio, con referentes reales."
* *Deporte:* "Diseña un plan de entrenamiento de 4 semanas para un corredor principiante de 10K."

El **mismo prompt** se envía a **Gemini, ChatGPT, Claude y Perplexity**. El grupo llena la tarjeta:

| Criterio (1–5) | Gemini | ChatGPT | Claude | Perplexity |
|---|---|---|---|---|
| ¿Respondió lo que pedí? | | | | |
| ¿Cita fuentes reales? (¡verifiquen una!) | | | | |
| ¿Se entiende / está bien escrito? | | | | |
| ¿Dijo algo falso o inventado? | | | | |
| ¿Cuál usaría para este reto? | | | | |

**Conclusión guiada:** no hay "la mejor IA"; hay la mejor para cada tarea. Y **todas** pueden inventar: por eso la Sesión 5 es sobre verificar.

## 🎧 Actividad 2: Tu carrera en un podcast (35 min)

1. Consigue **un documento real de tu carrera** (5 min): busca en Google `filetype:pdf` + un tema tuyo (una guía clínica, una ley, un catálogo de exposición, un plan de entrenamiento), o descarga el PIIA de una materia tuya, o usa un PDF que ya tengas en el correo o en Drive.
2. Entra a [NotebookLM](https://notebooklm.google.com) y crea un cuaderno con el nombre de tu carrera. Agrega **3 fuentes**: ese PDF, una URL de Wikipedia o de un artículo, y un video de YouTube del tema.
3. Haz 3 preguntas al cuaderno en el chat. Fíjate en que **cada respuesta cita el fragmento exacto** de tus fuentes.
4. En el panel *Studio* genera:
   * un **Audio Overview** (podcast) — pídelo en español y con enfoque "para alguien que llega nuevo al tema";
   * un **Mapa mental**;
   * un **Quiz** de 5 preguntas.
5. Escucha el primer minuto del podcast. ¿Dijo algo que no está en tus fuentes? Eso es lo que discutiremos.

```{admonition} Ruta pro 🧗
:class: tip
Pídele a NotebookLM un **Video Overview** o una **Infografía** del mismo cuaderno. Y en Gemini pide: "Crea un plan de estudio de 4 semanas para este tema en una tabla" y pégalo en un Google Doc con **Gemini en Docs**.
```

## 📦 Lo que te llevas

Tu cuaderno de NotebookLM con tu carrera (es la primera pieza del **Ejercicio 1**). En el tablero compartido del curso pega el enlace y **3 líneas**: qué te sorprendió, qué te dio desconfianza, qué quieres construir en el curso.

## 🎬 Guion del docente (prompts exactos de cada demo)

```{admonition} Preparar antes de clase (30 min)
:class: dropdown
* Sesión iniciada en: Gemini (con Deep Research disponible), NotebookLM, Claude, AppSheet, Gamma, terminal con `gemini` instalado.
* Un cuaderno de NotebookLM **ya creado** con un PDF largo (≈200 páginas) de alguna de las carreras del grupo y con el podcast **ya generado** (tarda 3–5 min; no esperar en vivo).
* Una carpeta `demo/` con 20–30 PDFs e imágenes variados de distintas carreras.
* Una hoja de Google con 10 filas de "inventario de laboratorio" (nombre, cantidad, ubicación, foto, responsable).
* Un informe de Deep Research **ya terminado** sobre un tema del grupo.
* Celular con Gemini instalado y proyectado (o con el cable/AirPlay listo).
* Plan B sin internet: capturas de pantalla / video de cada demo en las diapositivas de respaldo.
```

| # | Demo | Qué escribir / hacer | Qué señalar |
|---|---|---|---|
| 1 | **Gemini Live con cámara** | Abrir Gemini en el celular → Live → cámara. Apuntar a una planta del salón / un artículo del Código / una obra en pantalla. Decir: *"¿Qué es esto y qué me deberías preguntar antes de opinar?"* | Ve, oye, habla. Es multimodal. |
| 2 | **Chatear con un PDF de 200 páginas** | Cuaderno preparado. Preguntar: *"¿En qué página se define X y qué excepciones menciona?"* | Cada respuesta trae la **cita**; clic en la cita lleva al párrafo exacto. |
| 3 | **PDF → podcast** | Mismo cuaderno, reproducir el Audio Overview ya generado (45 s). | Dos voces, en español, discutiendo *tu* documento. Es lo que van a hacer hoy. |
| 4 | **Juego sin programar** | Claude: *"Crea un juego de memoria con 8 parejas de términos y definiciones de anatomía del hombro. Con puntaje, cronómetro y colores alegres. En español."* Jugarlo en vivo. | La IA escribió ~200 líneas de código que nadie tuvo que leer. |
| 5 | **Generar un video** | Gemini: *"Genera un video de 8 segundos: un colibrí en cámara lenta sobre un frailejón en un páramo colombiano al amanecer."* (o mostrar uno pregenerado si tarda) | Lo que hace 3 años costaba una productora. Y por eso la Sesión 6 es sobre deepfakes. |
| 6 | **Analizar una carpeta** | Terminal en `demo/`, escribir `gemini` y luego: *"Lista los archivos de esta carpeta, dime de qué trata cada uno en una línea y agrúpalos por carrera."* | Está leyendo el disco. Nada se modificó. Eso es un **agente** (S14). |
| 7 | **App desde una hoja de cálculo** | Sheets → Extensiones → AppSheet → Crear app. Abrir en el celular, tomar una foto de un objeto y guardarlo. | Sistema de gestión en 3 minutos (S9). |
| 8 | **Investigar con fuentes** | Mostrar el informe de Deep Research terminado; abrir una fuente citada. Luego preguntar al grupo: *"¿y si una de estas fuentes no existiera?"* | Investigar con IA es rápido; **verificar** es el trabajo (S5). |
| 9 | **Otro idioma** | Gemini Live: *"Let's practice: I'm a biologist presenting at a conference. Correct my English as I speak."* Hablar 20 segundos. | Práctica de idioma gratis, 24/7. |
| 10 | **Presentación en 1 minuto** | Gamma: pegar 3 párrafos del PDF → Generar. | 8 diapositivas con diseño (S8). |

Cerrar el tour con: **"¿Cuál de estos les gustaría saber hacer?"** Anotar en el tablero; usarlo para elegir ejemplos en las próximas sesiones.
