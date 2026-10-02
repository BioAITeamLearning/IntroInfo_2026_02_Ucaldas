---
title: Sesión 4 · Prompts y tu asistente
---
# Sesión 4 · Prompts y tu asistente 🗣️🤖

## 🧰 Herramientas del día

| Herramienta | Para qué | Enlace |
|---|---|---|
| **Gemini** | Escribir y comparar prompts | [gemini.google.com](https://gemini.google.com) |
| **Google Scholar** | Comprobar si las fuentes existen | [scholar.google.com](https://scholar.google.com) |
| **Google AI Studio** | Montar el asistente y ver los controles por dentro | [aistudio.google.com](https://aistudio.google.com) |

## 🎯 Qué te llevas

Tu ficha de instrucciones escrita y un asistente montado con ella, con tus documentos adentro, probado y corregido. Es la pieza central del **Ejercicio 1**.

---

## 🧱 Las cinco piezas de un prompt

| Pieza | La pregunta que responde | Ejemplo |
|---|---|---|
| **Rol** | ¿Quién quiero que sea? | "Eres abogado litigante en Colombia" |
| **Contexto** | ¿Qué necesita saber de mí? | "Para estudiantes de primer semestre que nunca han usado uno" |
| **Tarea** | ¿Qué debe hacer? | "Explica el derecho de petición" |
| **Formato** | ¿Cómo lo quiero? | "Máximo 150 palabras, con una analogía y 3 preguntas de repaso" |
| **Límites** | ¿Qué NO debe hacer? | "Sin usar 'silencio administrativo'. Sin inventar normas" |

Y tres frases que sirven en cualquier prompt:

* *"Antes de responder, hazme 3 preguntas para entender mi caso."*
* *"Ahora critica tu propia respuesta como un jurado exigente."*
* *"Si no tienes la información, dilo en vez de inventar."*

---

## 👀 El mismo tema, dos prompts

Esto es lo que sale al pedir lo mismo de dos maneras distintas.

::::{grid} 1 1 2 2
:gutter: 3

:::{grid-item-card}
**Prompt pelado**
^^^
> Explica el derecho de petición.

**Lo que salió** (fragmento, ~350 palabras en total):

*"El derecho de petición es un derecho fundamental consagrado en el artículo 23 de la Constitución Política de Colombia, desarrollado por la Ley 1755 de 2015. Permite a toda persona presentar peticiones respetuosas a las autoridades… Si la administración no responde dentro del término legal se configura el silencio administrativo negativo…"*

Correcto, pero sirve igual para un abogado que para alguien de primer semestre.
:::

:::{grid-item-card}
**Prompt con las cinco piezas**
^^^
> Eres abogado litigante en Colombia. Explica el derecho de petición a estudiantes de primer semestre que nunca han usado uno, en máximo 150 palabras, con una analogía cotidiana y 3 preguntas de repaso con su respuesta. No uses los términos "silencio administrativo" ni "acto administrativo", y no inventes normas: si no estás seguro de una, dilo.

**Lo que salió** (fragmento, 140 palabras en total):

*"Imagina que le dejas una nota al administrador de tu edificio pidiendo que arreglen el ascensor, y él está obligado a contestarte. Eso es el derecho de petición… Está en el artículo 23 de la Constitución y lo desarrolla la Ley 1755 de 2015. Plazos: 15 días hábiles en general, 10 si pides documentos, 30 si es una consulta. **Preguntas de repaso:** 1. ¿Dónde está consagrado?…"*
:::
::::

Lo que cambió, medido: pasó de ~350 a 140 palabras · apareció una analogía · aparecieron las preguntas de repaso · los dos términos prohibidos desaparecieron del texto.

---

## 🔬 Reto 1 · Sube una pieza a la vez

Cinco envíos a Gemini sobre **el mismo tema**. En cada uno pegas el anterior y le agregas una pieza. Busca tu carrera y usa los prompts tal cual.

### Biología

| # | Qué escribes |
|---|---|
| 1 | `Explica por qué se usa un control negativo en una PCR.` |
| 2 | `Eres biólogo molecular con 10 años de experiencia en laboratorio clínico. Explica por qué se usa un control negativo en una PCR.` |
| 3 | `…para estudiantes de primer semestre de biología que nunca han entrado a un laboratorio.` |
| 4 | `…en máximo 150 palabras, con una analogía cotidiana y 3 preguntas de repaso con su respuesta.` |
| 5 | `…sin usar las palabras "amplicón" ni "contaminación cruzada", y sin inventar datos.` |

### Derecho

| # | Qué escribes |
|---|---|
| 1 | `Explica el derecho de petición.` |
| 2 | `Eres abogado litigante en Colombia. Explica el derecho de petición.` |
| 3 | `…a estudiantes de primer semestre que nunca han usado uno.` |
| 4 | `…en máximo 150 palabras, con una analogía cotidiana y 3 preguntas de repaso con su respuesta.` |
| 5 | `…sin usar los términos "silencio administrativo" ni "acto administrativo", y sin inventar normas.` |

### Artes

| # | Qué escribes |
|---|---|
| 1 | `Explica qué hace que "Fuente" de Duchamp (1917) sea considerada arte.` |
| 2 | `Eres curador de arte contemporáneo. Explica qué hace que "Fuente" de Duchamp (1917) sea considerada arte.` |
| 3 | `…a estudiantes de primer semestre que nunca han visto una obra conceptual.` |
| 4 | `…en máximo 150 palabras, con una analogía cotidiana y 3 preguntas de repaso con su respuesta.` |
| 5 | `…sin usar los términos "ready-made" ni "vanguardia", y sin inventar fechas ni museos.` |

### Deporte

| # | Qué escribes |
|---|---|
| 1 | `Explica qué es el umbral de lactato.` |
| 2 | `Eres fisiólogo del ejercicio y entrenador de atletismo. Explica qué es el umbral de lactato.` |
| 3 | `…a corredores aficionados que nunca han hecho una prueba de laboratorio.` |
| 4 | `…en máximo 150 palabras, con una analogía cotidiana y 3 preguntas de repaso con su respuesta.` |
| 5 | `…sin usar los términos "VO2 máx" ni "metabolismo anaeróbico", y sin inventar cifras.` |

### Qué revisar en cada envío

| Envío | Revisa esto |
|---|---|
| 1 | ¿A quién le está hablando? Copia el texto en un documento y mira el contador: ¿cuántas palabras? |
| 2 | ¿Cambió el vocabulario respecto al 1? |
| 3 | ¿Aparecieron ejemplos o comparaciones que antes no estaban? |
| 4 | **Cuenta las palabras.** ¿Cumplió las 150? (muchas veces se pasa: anótalo) |
| 5 | **Ctrl+F** con cada palabra prohibida. ¿Cuántas veces aparece? |

Al terminar, pon el envío 1 y el 5 lado a lado y decide cuál pieza produjo el cambio más grande.

---

## ✍️ Reto 2 · Tres encargos

Tres cosas para producir, una por prompt. Escribe el prompt completo —con las cinco piezas— antes de enviarlo.

| # | Encargo | Qué tiene que salir |
|---|---|---|
| 1 | Pedir permiso para usar el laboratorio (o el archivo, la cancha, el salón de ensayo) el sábado de 8 a 12 para un trabajo de clase, escribiéndole al coordinador del programa | Un correo que puedas enviar sin cambiarle nada |
| 2 | Cinco preguntas de opción múltiple sobre el tema que usaste en el Reto 1 | Las cuatro opciones de cada una y la explicación de por qué las tres incorrectas están mal |
| 3 | Resumir el reglamento que está abajo | Media página para alguien de primer semestre, más cinco reglas en lenguaje claro |

### El documento del encargo 3

<a href="_static/sesion04/texto-para-resumir.pdf" target="_blank">📄 Reglamento (PDF para adjuntar)</a> · <a href="_static/sesion04/texto-para-resumir.html" target="_blank">📋 Versión para leer y copiar</a>

Es un texto de práctica: un reglamento ficticio escrito en el lenguaje con el que suelen estar escritos los reglamentos de verdad. Adjúntalo o pégalo en el chat.

Cuando tengas tu resumen, revisa si incluye estas tres obligaciones, que son fáciles de pasar por alto al leer rápido:

* El plazo que tienes para sacar tu información cuando pierdes la cuenta institucional.
* Qué está prohibido escribir dentro de una herramienta de inteligencia artificial, y qué hay que declarar al usarla.
* En cuánto tiempo hay que reportar un incidente de seguridad.

Compara tu resumen con el de un compañero: casi nunca se les escapan las mismas.

## 💥 Reto 3 · Hazla fallar

1. Pídele **5 fuentes académicas reales** con autor, año y enlace sobre uno de estos temas (o uno igual de específico de tu carrera):

| Carrera | Tema |
|---|---|
| Biología | La rana dorada (*Phyllobates terribilis*) en el Chocó |
| Derecho | Jurisprudencia de la Corte Constitucional colombiana sobre teletrabajo |
| Artes | El muralismo urbano en Manizales |
| Deporte | Entrenamiento en altura en deportistas colombianos |

2. Busca cada una en [Google Scholar](https://scholar.google.com) por título y autor. Anota cuántas existen: **___ de 5**.

3. Vuelve a pedirlo agregando: *"Solo cita fuentes que puedas verificar. Si no estás seguro de una, no la incluyas y dilo."* Anota de nuevo: **___ de 5**.

A esto se le llama **alucinación**: la IA no está mintiendo, está prediciendo texto que suena correcto. Por eso los prompts llevan límites, y por eso tu asistente va a tener documentos propios.

---

## 🤖 Construye tu asistente

Un asistente es un modelo + unas instrucciones fijas + tus documentos. Lo importante no es la herramienta donde lo montes, sino la **ficha de instrucciones** que escribas: esa ficha la guardas en un documento tuyo y la puedes volver a usar en cualquier herramienta, hoy y el año entrante.

### Paso 1 · Para qué sirve el tuyo

Completa: *"Un asistente que me ayuda a ______________ cuando ______________."*

| Carrera | Ejemplo |
|---|---|
| Biología | Me ayuda a entender protocolos de laboratorio antes de ejecutarlos |
| Derecho | Me ayuda a redactar documentos, pidiéndome los hechos primero |
| Artes | Me ayuda a analizar una obra y encontrar referentes |
| Deporte | Me ayuda a planear entrenamientos preguntando por lesiones previas |

### Paso 2 · Escribe la ficha

Llénala en la hoja impresa y después cópiala a un **Google Doc llamado `Ficha de mi asistente`**. Ese documento es tuyo y no depende de ninguna plataforma.

```
QUIÉN ERES
Eres [rol] con experiencia en [área].

PARA QUIÉN TRABAJAS
Estudio [carrera], semestre [N], en Manizales.
Mi nivel en el tema es [principiante / intermedio].

QUÉ HACES
Me ayudas a [tarea 1], [tarea 2] y [tarea 3].

CÓMO RESPONDES SIEMPRE
En español, máximo [N] palabras, en [tabla / pasos / párrafos cortos].
Tono [cercano / técnico]. Explicas los términos difíciles la primera vez.

QUÉ NUNCA HACES
No inventas datos ni fuentes. No [prohibición propia de tu carrera].

QUÉ HACES CUANDO NO SABES
Lo dices. Si te falta información para responder bien, me preguntas antes.
```

### Paso 3 · Móntalo en AI Studio

[aistudio.google.com](https://aistudio.google.com) es la consola donde Google deja ver lo que normalmente está escondido detrás del chat.

1. Entra con tu cuenta de Google (si la institucional no te deja, usa la personal) y abre un **Chat**.
2. Busca el campo **System instructions** (instrucciones del sistema) y pega ahí tu ficha completa.
3. Con el botón **+** adjunta 2 o 3 documentos de tu carrera.
4. Escribe una pregunta en el chat y mira la respuesta.
5. En el panel de ajustes, mueve la **temperatura** de 0 a 1 y vuelve a preguntar lo mismo. Vas a ver de qué depende que la IA sea más predecible o más suelta.
6. **Guarda** el prompt: queda en tu Drive y puedes compartir el enlace.

```{admonition} Si AI Studio no te abre
:class: tip
Tu ficha funciona igual en otros lugares: **Gems** de Gemini ([gemini.google.com](https://gemini.google.com) → Gems → Nuevo Gem), **Proyectos** de Claude ([claude.ai](https://claude.ai) → Proyectos), o simplemente pegándola al inicio de cualquier conversación nueva. Lo que se evalúa es la ficha y que el asistente responda como dice la ficha.
```

### Paso 4 · Pásale el banco de pruebas

| # | Pregúntale | Debería |
|---|---|---|
| 1 | Algo que **sí está** en los documentos que le subiste | Responder y decir de dónde lo sacó |
| 2 | Lo mismo, pero "en una tabla de tres columnas" | Obedecer el formato |
| 3 | Algo que **no está** en esos documentos | Decir que no lo sabe, sin inventar |
| 4 | Algo ambiguo, sin darle datos suficientes | Preguntarte antes de responder |
| 5 | "¿Y eso por qué?" | Mantener el hilo de la respuesta anterior |

### Paso 5 · Corrige la ficha

Por cada prueba que falló, agrega una línea y vuelve a probar:

| Si falló | Agrega |
|---|---|
| Inventó | "Si la respuesta no está en los documentos adjuntos, dilo explícitamente." |
| Respondió larguísimo | "Máximo 200 palabras salvo que te pida más." |
| No preguntó nada | "Si te faltan datos, pregunta antes de responder." |
| Muy técnico o muy simple | "Explica como a alguien de [tu nivel]." |

Casi nunca queda bien al primer intento: corregir la ficha es parte del trabajo. Cada línea que agregues, agrégala también al Google Doc.

## 🔄 Prueba cruzada

Intercambia tu asistente con alguien de otra carrera. Esa persona le hace tres preguntas —una que sí está en tus documentos, una que no está y una ambigua—, te dice en una frase qué falló, y tú arreglas una cosa en vivo y se la muestras funcionando.

---

## 📽️ Material

* <a href="_static/sesion04/slides.html" target="_blank">Diapositivas de la sesión</a>
* <a href="_static/sesion04/guia.html" target="_blank">Guía de los retos y plantilla del asistente</a>

## 📦 Lo que te llevas

El Google Doc con tu ficha de instrucciones y el asistente montado y funcionando. En el tablero del curso: el enlace al asistente y el resultado del Reto 3 (**___ de 5** fuentes existían).
