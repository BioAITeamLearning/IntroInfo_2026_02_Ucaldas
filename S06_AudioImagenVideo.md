---
title: Sesión 6 · Audio, imagen y video
---
# Sesión 6 · Tu voz, tu cara y tu historia 🎙️🖼️🎬

Un taller de producción. Sales con un video de 60 a 90 segundos en el que un personaje tuyo, en un lugar que elegiste, con una voz que escogiste, le explica algo de tu carrera a alguien que no sabe nada del tema.

Así se ve el resultado. Son **dos clips de diez segundos** generados por separado y pegados después; el video completo son seis. Fíjate en que es la misma persona, la misma camisa y el mismo salón en los dos: eso lo logra adjuntar la misma foto, nada más.

*Guion, imagen y voz generados con IA (Gemini). Clips unidos con ChatGPT.*

```{raw} html
<video controls preload="metadata" poster="_static/sesion06/S06_ejemplo_portada.jpg" style="width:100%; max-width:820px; border-radius:0.6rem; display:block; margin:1.2rem auto;">
  <source src="_static/sesion06/S06_ejemplo_clips.mp4" type="video/mp4">
</video>
```

## 🧰 Herramientas del día

| Para qué | Herramienta |
|---|---|
| **Guion** | [Gemini](https://gemini.google.com) |
| **Los clips de video** | [Gemini](https://gemini.google.com) → *Crear video* |
| **Unir los clips** | [ChatGPT](https://chatgpt.com) |
| **Voz aparte** *(opcional)* | [ElevenLabs](https://elevenlabs.io) |
| **Subtítulos y música** *(opcional)* | [CapCut](https://capcut.com) |

```{warning}
**Esto necesita una cuenta de Gmail personal.** La cuenta institucional de la Universidad **no tiene** *Crear video*: se comprobó en las cuentas de UCaldas y de la UAM, y en ambas el menú solo llega hasta Deep Research. Si solo tienes la institucional, sáltate al final de la página: hay una ruta B que funciona igual.

El cupo de video cambia seguido y Google no lo publica. En una cuenta Pro son unos 3 videos al día. En una cuenta gratuita puede ser poco o ninguno ese día: pruébalo **antes** de contar con él.
```

## 📽️ Material

* <a href="_static/sesion06/S06_audio_imagen_video.pptx">⬇️ Presentación de la sesión (PowerPoint)</a> — los prompts completos están en las notas de cada diapositiva
* <a href="_static/sesion06/guia.html" target="_blank">Hoja de trabajo</a>
* <a href="_static/sesion06/S06_ejemplo_clips.mp4">⬇️ Video de ejemplo</a> — el de arriba, para descargar

---

## ⛔ Antes de producir nada

Tres reglas que no se negocian:

| | |
|---|---|
| **Tu cara y tu voz** | Solo las tuyas. De nadie más, aunque sea un chiste, aunque sea tu amigo, aunque sea un famoso. |
| **Se declara** | En el video o en su descripción: qué parte se hizo con IA y con qué herramienta. |
| **Nada confidencial** | Ni datos de pacientes, ni de clientes, ni de menores, ni expedientes. |

Hacer un video con la cara o la voz de otra persona sin su consentimiento no es una travesura: en Colombia puede constituir un delito. Si no quieres usar tu propia cara, el paso 3 tiene una ruta alterna.

---

## 1 · El guion

Primero qué se dice. Siempre. El error más común es empezar por la imagen bonita y después no saber qué contar.

Tres piezas: **una primera frase que enganche**, **una idea central explicada con una comparación cotidiana**, y **un cierre que deje una pregunta**.

```
Eres guionista de videos educativos cortos. Escríbeme un guion de 150 palabras
para un video de 60 segundos.

Tema: [lo que haces en tu carrera, o un concepto que te costó entender].
Para: alguien que no sabe nada del tema y no es de tu área.

Estructura: una primera frase que enganche, una idea central explicada con una
comparación cotidiana, y un cierre que deje una pregunta.

Reglas: frases cortas, para decir en voz alta. Sin tecnicismos sin explicar.
Nada de "en el mundo actual" ni "hoy en día". Al final, dime cuántas palabras tiene.
```

**La prueba:** léelo en voz alta y cronométrate. Se habla a unas 150 palabras por minuto: 150 palabras son un minuto, 80 son medio. Si te trabas al leerlo, está mal escrito: pídele que lo simplifique.

**Después, pártelo.** Cada clip dura 10 segundos, así que necesitas frases de unas 25 palabras:

```
Parte este guion en 6 frases de unas 25 palabras cada una. Cada frase tiene que
poder decirse sola en 10 segundos y entenderse sin la anterior. Numéralas.
```

### Truco: dicta el guion en vez de escribirlo

Un texto dictado suena a persona hablando; uno escrito suena a texto escrito. En Google Docs: **Herramientas → Dictado por voz**. Hablas treinta segundos y aparece escrito. O grabas una nota de voz en el celular y se la subes a Gemini pidiéndole la transcripción.

Después lo pules: *"Limpia este dictado, quita las muletillas y déjalo en 150 palabras."*

## 2 · Tu foto

Una sola foto tuya, de frente, con la cara bien iluminada y sin gafas de sol. Esa misma foto la vas a adjuntar en **todos** los clips: es lo que hace que seas la misma persona en los seis y no seis desconocidos distintos.

```{admonition} Si no quieres usar tu cara
:class: tip
No adjuntes foto y describe un personaje inventado: *"un ingeniero de alimentos de unos 40 años, pelo corto, bata blanca"*. Repite **la misma descripción, palabra por palabra**, en cada clip. Queda menos consistente que con foto, pero funciona. Nadie está obligado a poner su cara.
```

## 3 · Los clips

Uno por frase. En Gemini: botón **+** → **Crear video**. Después adjuntas la foto y escribes el prompt.

```
La persona de la foto, en plano medio dentro de [el lugar: un laboratorio, una
sala de audiencias, un taller, una cancha, un afloramiento rocoso], con luz
natural suave.

Mira a la cámara y dice en español latinoamericano, tono cercano y pausado:
«[aquí va una de tus frases]»

Cámara fija, sin texto en pantalla.
```

Cada clip sale de **10 segundos, con la voz ya puesta**, y tarda unos dos minutos y medio.

```{admonition} El orden importa
:class: warning
Activa **Crear video primero** y adjunta la foto **después**. Si lo haces al revés, Gemini se sale del modo video y te contesta por escrito en vez de generarte el clip.

Antes de enviar, comprueba que abajo diga **Videos** y aparezca el selector **Horizontal**. Si no están, no vas a recibir un video.
```

## 4 · Unirlos

Gemini **no** puede unir videos: ejecuta código pero su entorno no tiene herramientas de video, así que te devuelve un comando de terminal. ChatGPT sí.

En ChatGPT, sube los clips y pídeselo:

```
Une estos clips en un solo video, en este orden: clip1, clip2, clip3...
Conserva el audio de cada uno. Déjame el archivo mp4 para descargar.
```

Tarda unos quince segundos y te devuelve el MP4 completo. Recodifica el video, así que pierde algo de calidad: para la clase no se nota.

## 5 · La voz *(opcional)*

Los clips ya vienen con voz, pero no la eliges tú. Si quieres otra, genera la narración aparte y móntala encima en CapCut.

| Ruta | Cómo es |
|---|---|
| **ElevenLabs** | Plan gratis de unos 10 minutos de audio al mes: de sobra. Tiene voces en español sin pedir tarjeta. Sin licencia comercial: hay que mencionar la herramienta, cosa que ya haces igual. |
| **Google AI Studio** | Modo *Generate speech*. Ojo: las voces filtradas como *Spanish* piden clave de pago. Filtra por **Gender** y usa una genérica: leen español perfectamente. |
| **Tu propia voz** | El celular. Gratis, es tuya, y a veces suena mejor que cualquier generada. |

La indicación de estilo cambia mucho el resultado:

```
Español latinoamericano, tono cercano y pausado, como quien le explica algo a un
amigo. No leas como noticiero.
```

## 6 · Los remates *(opcional)*

En CapCut, sobre el video ya unido:

1. **Subtítulos automáticos** — y revísalos: siempre hay dos o tres palabras mal.
2. Música de fondo al 10 o 15 % del volumen. Si compite con la voz, está muy alta.
3. Corta los silencios largos entre clip y clip.

Música muy alta y subtítulos sin revisar son las dos marcas de un video amateur. Arreglar esas dos cosas te sube el resultado más que cualquier efecto.

---

## 🅱️ Ruta B: sin cupo de video

Si no tienes *Crear video*, o se te acabó el cupo, el video se arma igual y queda bien:

1. **El ambiente**: pídele a Gemini una imagen 16:9 del lugar, *sin personas, sin texto, con espacio libre a un lado*.
2. **Tu personaje**: *"Con esta foto mía como referencia, genera un retrato de medio cuerpo del mismo personaje. Fondo gris liso y uniforme, sin sombras. Formato vertical."* El fondo liso es lo que te deja recortarlo.
3. **La voz**: ElevenLabs con el guion completo.
4. **El montaje** en CapCut: ambiente de fondo, avatar encima con *quitar fondo*, la voz debajo, subtítulos y un zoom lento sobre la imagen.

Sale un video quieto pero bien contado. Y lo bien contado pesa más que el movimiento.

---

## 🎬 El encargo

Elige uno de los dos:

| | |
|---|---|
| **Qué hago en mi carrera** | Un día normal de trabajo de alguien de tu programa. Lo que nadie se imagina que haces. |
| **Lo que me costó entender** | Un concepto que te costó, explicado como te hubiera gustado que te lo explicaran. |

Un minuto, en seis clips de diez segundos, con tu cara y tu voz. Y al final, una línea diciendo qué hiciste con IA.
