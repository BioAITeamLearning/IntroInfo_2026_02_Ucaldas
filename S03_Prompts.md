---
title: Sesión 3 · Prompts y tu asistente
---
# Sesión 3 · Técnicas de prompt y tu asistente 🗣️🤖

## 🧰 Herramientas del día

| Herramienta | Para qué | Enlace | Costo |
|---|---|---|---|
| **Gemini** | Escribir y comparar prompts | [gemini.google.com](https://gemini.google.com) | Gratis |
| **Gems** (dentro de Gemini) | Montar tu asistente | [gemini.google.com/gems](https://gemini.google.com/gems) | Gratis |
| **ChatGPT** | El equivalente, para comparar | [chatgpt.com](https://chatgpt.com) | Gratis |
| **Google Scholar** | Comprobar si las fuentes existen | [scholar.google.com](https://scholar.google.com) | Gratis |
| **Hoja de prompts** | Copiar y pegar todo lo de hoy | <a href="_static/sesion03/prompts.html" target="_blank">Abrir</a> | — |

## 🎯 Qué te llevas

Tu ficha de instrucciones escrita, un asistente montado con ella y probado, y cinco técnicas de prompt que vas a usar el resto del semestre.

---

## 🏋️ No todos los modelos son iguales

Cuando abres Gemini o ChatGPT hay un selector de modelo. Vale la pena saber qué estás eligiendo, porque **el mismo prompt da resultados distintos según el modelo**.

### Qué es un parámetro

Un modelo aprende ajustando millones de números internos durante el entrenamiento. Cada uno de esos números es un **parámetro**. Piensa en perillas: el entrenamiento consiste en girar todas las perillas hasta que el modelo acierte lo más posible al predecir el texto siguiente.

Un modelo abierto como Llama viene en versiones de **8 mil millones**, **70 mil millones** y **405 mil millones** de parámetros. Los modelos de Gemini, ChatGPT y Claude no publican esa cifra, pero están en ese orden de magnitud o más.

```{admonition} Ojo con la palabra "billón"
:class: warning
En inglés *billion* son **mil millones** (1 000 000 000). En español un **billón** es un millón de millones, mil veces más. Cuando leas "70B parameters", son **70 mil millones**, no 70 billones. Es un error de traducción tan común que vale la pena tenerlo presente.
```

### Liviano contra grande

Cada empresa ofrece dos o tres tamaños de la misma generación. Los nombres cambian cada pocos meses; la lógica no:

| | Modelos livianos y rápidos | Modelos grandes |
|---|---|---|
| Cómo se llaman | *Flash*, *Lite*, *mini*, *Haiku* | *Pro*, *Opus*, y los modos de **razonamiento** o **pensamiento** |
| Velocidad | Responden casi al instante | Se demoran, a veces bastante |
| En qué son buenos | Resumir, traducir, reescribir, clasificar, contestar lo frecuente | Problemas con varios pasos, análisis de documentos largos, redacción exigente, código |
| En qué fallan | Se enredan en problemas que exigen encadenar razonamientos | En nada grave, pero gastan tu cuota |
| En un plan gratuito | Es el que te dan por defecto, con uso amplio | Tienes una cuota limitada por día |

Dos cosas que conviene no olvidar:

* **Más parámetros no es automáticamente mejor.** Un modelo pequeño y reciente suele ganarle a uno grande de hace dos años.
* **El tamaño no arregla la alucinación.** Un modelo grande inventa menos, pero inventa. Lo vas a comprobar tú mismo más adelante en esta misma clase.

```{admonition} Pruébalo ahora (3 minutos)
:class: tip
Toma este problema y mándaselo primero al modelo rápido y después al grande, sin cambiar una coma:

> *En un salón hay 30 estudiantes. La mitad estudia biología. De los que quedan, dos tercios estudian derecho y el resto, artes. ¿Cuántos estudian artes? Responde solo con el número.*

Resuélvelo tú también en el papel. ¿Coincidieron? ¿Cuál se demoró más? Guarda el dato: en el resto de la clase vas a volver a elegir modelo varias veces.
```

## 🧱 Las cinco piezas de un prompt

| Pieza | La pregunta que responde | Ejemplo |
|---|---|---|
| **Rol** | ¿Quién quiero que sea? | "Eres abogado litigante en Colombia" |
| **Contexto** | ¿Qué necesita saber de mí? | "Para estudiantes de primer semestre que nunca han usado uno" |
| **Tarea** | ¿Qué debe hacer? | "Explica el derecho de petición" |
| **Formato** | ¿Cómo lo quiero? | "Máximo 150 palabras, con una analogía y 3 preguntas de repaso" |
| **Límites** | ¿Qué NO debe hacer? | "Sin usar 'silencio administrativo'. Sin inventar normas" |

---

## 👀 El mismo tema, dos prompts

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

Cinco envíos sobre **el mismo tema**. En cada uno pegas el anterior y le agregas una pieza:

| Envío | Qué agregas |
|---|---|
| 1 | Solo la tarea: `Explica [tu tema].` |
| 2 | **+ rol**: `Eres [profesional de tu área]. Explica [tu tema].` |
| 3 | **+ contexto**: `…para estudiantes de primer semestre que nunca han visto el tema.` |
| 4 | **+ formato**: `…en máximo 150 palabras, con una analogía cotidiana y 3 preguntas de repaso con su respuesta.` |
| 5 | **+ límites**: `…sin usar las palabras "[A]" ni "[B]", y sin inventar datos.` |

Busca tu área y usa este tema y estas palabras prohibidas:

| Área | Tu tema | Palabras prohibidas |
|---|---|---|
| **Biología** | Por qué se usa un control negativo en una PCR | *amplicón* · *contaminación cruzada* |
| **Derecho** | El derecho de petición | *silencio administrativo* · *acto administrativo* |
| **Artes** | Qué hace que "Fuente" de Duchamp (1917) sea considerada arte | *ready-made* · *vanguardia* |
| **Diseño visual** | Por qué un afiche con cinco tipografías distintas se ve mal | *jerarquía* · *contraste* |
| **Ingeniería de alimentos** | Por qué la pasteurización no esteriliza | *termorresistente* · *carga microbiana* |
| **Estudios de familia** | Qué es un genograma y para qué sirve | *sistémico* · *intergeneracional* |
| **Deporte** | Qué es el umbral de lactato | *VO2 máx* · *metabolismo anaeróbico* |

### Qué revisar en cada envío

| Envío | Revisa esto |
|---|---|
| 1 | ¿A quién le está hablando? Pega el texto en un documento y mira el contador: ¿cuántas palabras? |
| 2 | ¿Cambió el vocabulario respecto al 1? |
| 3 | ¿Aparecieron ejemplos o comparaciones que antes no estaban? |
| 4 | **Cuenta las palabras.** ¿Cumplió las 150? (muchas veces se pasa: anótalo) |
| 5 | **Ctrl+F** con cada palabra prohibida. ¿Cuántas veces aparece? |

---

## 🎯 Técnicas de prompt

Son cinco, y se diferencian en **cuántos ejemplos le das** y en **si le pides que desarrolle el razonamiento**.

| Técnica | En qué consiste | Cuándo la usas |
|---|---|---|
| **Zero-shot** | Pedir la tarea sin darle ningún ejemplo | Tareas comunes: resumir, traducir, explicar |
| **One-shot** | Darle **un** ejemplo del resultado que quieres | Cuando te importa el formato y es difícil describirlo con palabras |
| **Few-shot** | Darle **entre dos y cinco** ejemplos | Cuando quieres que copie un estilo, una estructura o un criterio de clasificación |
| **Cadena de pensamiento** | Pedirle que muestre el desarrollo antes de concluir | Cuando necesitas **ver** y verificar el procedimiento |
| **Modo de razonamiento** | El modelo arma esa cadena por dentro, sin que se lo pidas | Problemas difíciles, cuando puedes esperar unos segundos más |

Ejemplo de **few-shot** para clasificar comentarios de una encuesta:

```
Clasifica cada comentario como POSITIVO, NEGATIVO o SUGERENCIA.

"La clase estuvo muy clara" → POSITIVO
"No se escuchaba nada al fondo" → NEGATIVO
"Sería bueno tener las diapositivas antes" → SUGERENCIA

"El laboratorio estaba muy frío" →
```

Los tres ejemplos no explican la regla: la muestran. Eso es lo que hace el few-shot.

---

## ✍️ Reto 2 · La misma tarea en zero, one y few shot

Vas a resumir el mismo documento tres veces.

**El documento:** <a href="_static/sesion03/texto-para-resumir.pdf" target="_blank">📄 Reglamento (PDF para adjuntar)</a> · <a href="_static/sesion03/texto-para-resumir.html" target="_blank">📋 Versión para leer y copiar</a>

Es un texto de práctica: un reglamento ficticio, escrito como están escritos los reglamentos de verdad.

| Intento | Qué le pides |
|---|---|
| **Zero-shot** | `Resume este reglamento para un estudiante de primer semestre.` |
| **One-shot** | Lo mismo, pero antes le pegas **un ejemplo** de resumen de otro reglamento con la forma que quieres (título, cinco reglas en lenguaje claro, una advertencia) |
| **Few-shot** | Lo mismo con **tres ejemplos** del mismo tipo, para fijar el estilo |

Compara los tres. ¿Cuál se parece más a lo que necesitabas? ¿Cuánto esfuerzo costó cada uno?

Después revisa si tu mejor resumen incluye estas tres obligaciones, que son fáciles de pasar por alto al leer rápido:

* El plazo que tienes para sacar tu información cuando pierdes la cuenta institucional.
* Qué está prohibido escribir dentro de una herramienta de inteligencia artificial, y qué hay que declarar al usarla.
* En cuánto tiempo hay que reportar un incidente de seguridad.

Compara con un compañero: casi nunca se les escapan las mismas.

---

## 🧠 ¿La IA piensa?

No. Genera texto **una pieza a la vez**, eligiendo cada vez la continuación más probable según lo que ya escribió. No tiene un plan previo ni revisa lo que dijo, salvo que lo vuelva a leer como parte del texto.

Durante años hubo que escribir *"razona paso a paso"* para que acertara en problemas con varios pasos. **Eso ya casi no hace falta**: los modelos actuales traen esa cadena por dentro y resuelven solos la aritmética y la lógica sencilla.

Entonces, ¿para qué sigue sirviendo pedir el desarrollo?

| Para qué | Ejemplo |
|---|---|
| Para **poder verificarlo** | "Muéstrame el procedimiento, no solo el resultado" |
| Para **aprender** del proceso | "Explica cada paso como si me estuvieras enseñando" |
| Para **encontrar dónde se equivocó** | Cuando el resultado te huele mal, el desarrollo te dice en qué paso se torció |

Y hay algo que ningún modelo, por grande que sea, resuelve solo: **cuando la trampa no está en el cálculo sino en la situación**.

```{admonition} Los modos de razonamiento
:class: note
Los modos de "razonamiento" o "pensamiento" de Gemini, ChatGPT y Claude generan por dentro una cadena larga de pasos antes de responderte. Aciertan más en problemas difíciles y tardan más. Siguen sin entender: siguen prediciendo. Y el razonamiento que te muestran es texto generado igual que el resto: puede sonar impecable y estar mal.
```

---

## 💥 Reto 3 · Hazla fallar

### Parte A · La trampa no está en el cálculo

Cópiale esto tal cual:

> Estoy tratando de caminar más y de bajar mi huella de carbono. El lavadero de carros queda a ocho cuadras de mi casa. ¿Me conviene ir caminando o en carro?

Lee la respuesta completa antes de seguir. ¿Te recomendó caminar? ¿Mencionó en algún momento que, si vas caminando, **el carro se queda en tu casa** y no hay nada que lavar?

Ahora pregúntale: *"¿Y qué pasa con mi carro si voy caminando?"*

Lo que acaba de ocurrir: la frase sobre caminar y la huella de carbono empuja la respuesta hacia un consejo que la IA ha leído miles de veces. Nada en el texto le obliga a detenerse a imaginar la escena. No es un error de cálculo: es que no hay nadie imaginando la situación.

Si la pillaste al primer intento, prueba esta otra:

> Tengo que recoger a mi hermana y sus tres maletas en el aeropuerto. Quiero aprovechar para hacer ejercicio. ¿Me voy en bicicleta?

```{tip}
La conclusión no es "la IA es tonta". Es que **el texto puede ser impecable y la respuesta inservible**, y que el único que mira la situación completa eres tú. Por eso en el resto del curso siempre hay un paso de verificación.
```

### Parte B · Fuentes que no existen

1. Pídele **5 fuentes académicas reales** con autor, año y enlace sobre un tema muy específico de tu área:

| Área | Tema |
|---|---|
| Biología | La rana dorada (*Phyllobates terribilis*) en el Chocó |
| Derecho | Jurisprudencia de la Corte Constitucional colombiana sobre teletrabajo |
| Artes · Diseño visual | El muralismo urbano en Manizales |
| Ingeniería de alimentos | Aprovechamiento de subproductos del café en Caldas |
| Estudios de familia | Familias transnacionales y migración en el Eje Cafetero |
| Deporte | Entrenamiento en altura en deportistas colombianos |

2. Búscalas en [Google Scholar](https://scholar.google.com) por título y autor. Anota cuántas existen: **___ de 5**.

3. Vuelve a pedirlo agregando: *"Solo cita fuentes que puedas verificar. Si no estás seguro de una, no la incluyas y dilo."* Anota de nuevo: **___ de 5**.

A esto se le llama **alucinación**. No está mintiendo: está completando texto plausible.

---

## 📚 Dos usos que vas a repetir todo el semestre

### Investigar un tema

Lo que no funciona: *"Investiga sobre X"*. Lo que sí:

```
Eres [profesional de mi área]. Quiero entender [tema] para [para qué te sirve].

1. Antes de responder, hazme 3 preguntas para delimitar el tema.
2. Después dame un panorama de máximo 400 palabras con: qué se sabe,
   qué está en discusión y qué no se sabe todavía.
3. Al final, lista 5 términos de búsqueda que yo debería usar en Google
   Scholar para profundizar.
4. No cites fuentes que no puedas verificar. Si no estás seguro, dilo.
```

Las fuentes las buscas tú con esos términos. La IA te ahorra el mapa, no la lectura.

### Redactar un informe

```
Eres [rol]. Escribe un informe sobre [tema] para [quién lo lee].

Estructura exacta, en este orden:
- Resumen (3 líneas)
- Contexto (1 párrafo)
- Hallazgos (3 viñetas, cada una con el dato que la sustenta)
- Limitaciones (2 viñetas)
- Qué sigue (2 viñetas)

Usa solo la información del documento que te adjunto. Si algo no está
en el documento, escribe [FALTA DATO] en vez de completarlo tú.
```

El `[FALTA DATO]` es el truco: te deja ver de inmediato qué tienes que conseguir tú.

---

## 🤖 Tu asistente

Un asistente es un modelo + unas instrucciones fijas + tus documentos. Lo importante no es la herramienta donde lo montes, sino la **ficha de instrucciones**: la guardas en un documento tuyo y la vuelves a usar donde quieras.

### Paso 1 · Para qué sirve el tuyo

Completa: *"Un asistente que me ayuda a ______________ cuando ______________."*

| Área | Ejemplo |
|---|---|
| Biología | Entender protocolos de laboratorio antes de ejecutarlos |
| Derecho | Redactar documentos, pidiéndome los hechos primero |
| Artes | Analizar una obra y encontrar referentes |
| Diseño visual | Criticar una pieza y proponer tres alternativas |
| Ingeniería de alimentos | Revisar una ficha técnica y señalar qué falta |
| Estudios de familia | Preparar una entrevista y revisar el lenguaje que uso |
| Deporte | Planear entrenamientos preguntando por lesiones previas |

### Paso 2 · Escribe la ficha

Llénala en la hoja impresa y cópiala a un **Google Doc llamado `Ficha de mi asistente`**.

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
Cuando la tarea tenga varios pasos, los desarrollas antes de concluir.

QUÉ NUNCA HACES
No inventas datos ni fuentes. No [prohibición propia de tu área].

QUÉ HACES CUANDO NO SABES
Lo dices. Si te falta información para responder bien, me preguntas antes.
```

### Paso 3 · Móntala en un Gem

[gemini.google.com](https://gemini.google.com) → **Gems** en el menú lateral → **Nuevo Gem** → nombre (`Tutor de [tu área]`) → pega la ficha en las instrucciones → sube 2 o 3 documentos de tu área → pruébalo en la vista previa → **Guardar**.

```{admonition} Todos los prompts de esta sesión, listos para copiar
:class: tip
<a href="_static/sesion03/prompts.html" target="_blank">📋 Abrir la hoja de prompts</a> — cada bloque tiene su botón de copiar: los cinco envíos del Reto 1, los tres intentos del Reto 2, las trampas del Reto 3, la ficha de ejemplo, las cinco pruebas y los prompts de investigar y redactar.
```

### Un ejemplo completo

Así se ve una ficha **ya llena**. Cambia lo que está entre corchetes por lo tuyo y queda lista:

```
QUIÉN ERES
Eres bióloga molecular con quince años de experiencia en laboratorio clínico
y docente de primeros semestres.

PARA QUIÉN TRABAJAS
Estudio Biología, segundo semestre, en la Universidad de Caldas (Manizales).
Mi nivel es principiante: entiendo los conceptos generales pero me pierdo
con los protocolos y la nomenclatura.

QUÉ HACES
Me ayudas a (1) entender protocolos de laboratorio antes de ejecutarlos,
(2) preparar el preinforme de cada práctica y (3) repasar para los parciales
con preguntas que tú me haces a mí.

CÓMO RESPONDES SIEMPRE
En español, máximo 250 palabras, en pasos numerados cuando se trate de un
procedimiento y en tabla cuando se trate de comparar.
Tono cercano, sin dejar de ser preciso.
La primera vez que uses un término técnico, lo explicas entre paréntesis.
Cuando la tarea tenga varios pasos, me muestras el desarrollo y no solo
el resultado.

QUÉ NUNCA HACES
No inventas datos, cifras ni fuentes.
No me das por buenas las concentraciones ni los tiempos: siempre me recuerdas
verificarlos contra el protocolo oficial del laboratorio.
No respondes preguntas de bioseguridad sin remitirme al docente.

QUÉ HACES CUANDO NO SABES
Lo dices con todas las letras: "esto no está en los documentos que me diste".
Si te falta información para responder bien, me haces las preguntas que
necesites antes de responder.
```

Y un ejemplo de respuesta ideal dentro de las instrucciones convierte tu ficha en un *one-shot* permanente. Agrégalo al final:

```
EJEMPLO DE UNA BUENA RESPUESTA
Pregunta: "¿Para qué sirve el control negativo?"
Respuesta:
1. Qué es: un tubo con todo menos la muestra.
2. Para qué: si aparece señal, algo se coló donde no debía.
3. Qué revisar si sale positivo: reactivos, pipetas, superficie de trabajo.
Verifica los volúmenes contra el protocolo del laboratorio.
```

### Lo mismo, en otras herramientas


| Herramienta | Dónde van las instrucciones | Dónde van los documentos | ¿Gratis? |
|---|---|---|---|
| **Gemini · Gems** | Instrucciones del Gem | Archivos del Gem | Sí |
| **ChatGPT · Proyectos** | Instrucciones del proyecto | Archivos del proyecto | Sí (si no te aparece, usa *Personalización → Instrucciones personalizadas*) |
| **ChatGPT · GPT propio** | Configuración del GPT | Conocimiento del GPT | No: crear GPTs requiere plan pago |
| **Claude · Proyectos** | Instrucciones del proyecto | Conocimiento del proyecto | Según tu cuenta |
| **Cualquier chat** | Pegar la ficha al inicio de la conversación | Adjuntar los archivos | Sí |

### Paso 4 · Pásale el banco de pruebas

| # | Escríbele esto | Debería |
|---|---|---|
| 1 | `Resume en cinco puntos lo más importante del documento que te subí.` | Responder y decir de dónde lo sacó |
| 2 | `Lo mismo, pero en una tabla de tres columnas: concepto, para qué sirve, dónde aparece.` | Obedecer el formato |
| 3 | `¿Qué dice el documento sobre [algo que sabes que NO está]?` | Decir que no lo sabe, sin inventar |
| 4 | `Ayúdame con el trabajo.` | Preguntarte qué trabajo antes de responder |
| 5 | `Explícame el procedimiento completo y muéstrame el desarrollo, no solo el resultado.` | Mostrar los pasos |

### Paso 5 · Corrige la ficha

| Si falló | Agrega |
|---|---|
| Inventó | "Si la respuesta no está en los documentos adjuntos, dilo explícitamente." |
| Respondió larguísimo | "Máximo 200 palabras salvo que te pida más." |
| No preguntó nada | "Si te faltan datos, pregunta antes de responder." |
| Saltó al resultado sin mostrar cómo | "Cuando la tarea tenga varios pasos, desarróllalos antes de concluir." |
| Muy técnico o muy simple | "Explica como a alguien de [tu nivel]." |

Casi nunca queda bien al primer intento. Cada línea que agregues, agrégala también al Google Doc.

---

## 🔄 Prueba cruzada

Intercambia tu asistente con alguien de otra área. Esa persona le hace tres preguntas —una que sí está en tus documentos, una que no está y una ambigua—, te dice en una frase qué falló, y tú arreglas una cosa en vivo y se la muestras funcionando.

---

## 📽️ Material

* <a href="_static/sesion03/prompts.html" target="_blank">📋 Todos los prompts de la sesión, listos para copiar</a>
* <a href="_static/sesion03/slides.html" target="_blank">Diapositivas de la sesión</a>
* <a href="_static/sesion03/guia.html" target="_blank">Guía de los retos y plantilla del asistente</a>
* <a href="_static/sesion03/texto-para-resumir.pdf" target="_blank">Reglamento para el Reto 2 (PDF)</a>

## 📦 Lo que te llevas

El Google Doc con tu ficha de instrucciones y el Gem montado con ella, probado y corregido. En el tablero del curso: el enlace al asistente y el resultado del Reto 3 (**___ de 5** fuentes existían).
