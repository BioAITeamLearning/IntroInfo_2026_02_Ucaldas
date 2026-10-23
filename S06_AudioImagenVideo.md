---
title: Sesión 6 · Audio, imagen y video
---
# Sesión 6 · Tu voz, tu cara y tu historia 🎙️🖼️🎬

Un taller de producción. Sales con un video de 60 a 90 segundos en el que un personaje tuyo, en un lugar que elegiste, con una voz que escogiste, le explica algo de tu carrera a alguien que no sabe nada del tema.

Así se ve el resultado. Todo lo que hay aquí adentro —guion, salón, avatar, voz— se hizo con las herramientas de esta sesión:

```{raw} html
<video controls preload="metadata" poster="_static/sesion06/S06_ejemplo_portada.jpg" style="width:100%; max-width:820px; border-radius:0.6rem; display:block; margin:1.2rem auto;">
  <source src="_static/sesion06/S06_ejemplo_que_es_la_IA.mp4" type="video/mp4">
</video>
```

## 🧰 Herramientas del día

Todas tienen capa gratuita. Si alguna no te abre, usa la alternativa de la misma fila.

| Para qué | Principal | Alternativa |
|---|---|---|
| **Guion** | [Gemini](https://gemini.google.com) | ChatGPT · Claude |
| **Voz a texto** | Dictado por voz de [Google Docs](https://docs.google.com) | Subir el audio a Gemini |
| **Imagen** | [Gemini](https://gemini.google.com) | [Bing Image Creator](https://www.bing.com/images/create) · [Ideogram](https://ideogram.ai) |
| **Texto a voz** | [Google AI Studio](https://aistudio.google.com) | [ElevenLabs](https://elevenlabs.io) · [TTSMaker](https://ttsmaker.com) |
| **Que el avatar hable** | [HeyGen](https://heygen.com) | [Hedra](https://hedra.com) · [Vidnoz](https://vidnoz.com) · Google Vids |
| **Montaje** | [CapCut](https://capcut.com) | Clipchamp · Canva |

```{warning}
Los cupos gratuitos de estas herramientas **cambian cada mes**, y casi todas las capas gratis ponen marca de agua y no dan derechos de uso comercial. Para una tarea de clase está bien; para el portafolio de un cliente, no.
```

## 📽️ Material

* <a href="_static/sesion06/S06_audio_imagen_video.pptx">⬇️ Presentación de la sesión (PowerPoint)</a> — los prompts completos están en las notas de cada diapositiva
* <a href="_static/sesion06/guia.html" target="_blank">Hoja de trabajo</a>
* <a href="_static/sesion06/S06_ejemplo_que_es_la_IA.mp4">⬇️ Video de ejemplo</a> — el de arriba, para descargar

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

### Truco: dicta el guion en vez de escribirlo

Un texto dictado suena a persona hablando; uno escrito suena a texto escrito. En Google Docs: **Herramientas → Dictado por voz**. Hablas treinta segundos y aparece escrito. O grabas una nota de voz en el celular y se la subes a Gemini pidiéndole la transcripción.

Después lo pules: *"Limpia este dictado, quita las muletillas y déjalo en 150 palabras."*

## 2 · El ambiente

La imagen del lugar donde ocurre lo que cuentas.

```
Genera una imagen horizontal, formato 16:9, de [el lugar: un laboratorio de
microbiología, una sala de audiencias, un taller de pintura, una planta de
alimentos, una cancha de atletismo, un afloramiento rocoso].

Estilo: fotografía realista, luz natural suave, profundidad de campo.
Sin personas en la escena.
Sin texto ni letreros.
Deja espacio libre en el lado derecho para colocar un personaje después.
```

Ese último renglón es el que casi nadie pide y el que más importa: si no lo dices, la imagen queda llena y tu avatar no cabe.

## 3 · Tu avatar

```
Con esta foto mía como referencia, genera un retrato de medio cuerpo del mismo
personaje, mirando al frente, con expresión amable.

Vestuario: [bata de laboratorio / toga / ropa de taller / uniforme deportivo /
camisa formal].
Fondo: gris liso y neutro.
Estilo: [ilustración digital limpia / fotografía realista].
Formato vertical. Hombros y cabeza completos, sin cortar la coronilla.
```

**Por qué el fondo liso:** es lo que te permite recortarlo y montarlo sobre el ambiente del paso 2. Con un fondo lleno de detalles, el recorte queda feo.

```{admonition} Si no quieres usar tu cara
:class: tip
Describe un personaje inventado y listo: *"un ingeniero de alimentos de unos 40 años, pelo corto, bata blanca"*. Funciona igual de bien. Nadie está obligado a poner su cara.
```

## 4 · La voz

| Ruta | Cómo |
|---|---|
| **Google AI Studio** | Modo *Speech / TTS*. Pegas el guion, eliges voz y le das una indicación de estilo. Las voces en español están marcadas como *preview*. |
| **ElevenLabs** | Plan gratuito de unos 10 minutos de audio al mes: de sobra para 60 segundos. Sin derechos comerciales. |
| **Tu propia voz** | El celular. Gratis, es tuya, y a veces suena mejor que cualquier generada. |

La indicación de estilo cambia mucho el resultado:

```
Léelo en español latinoamericano, tono cercano y pausado, como quien le explica
algo a un amigo. No lo leas como noticiero.
```

Prueba a generar la misma frase con dos voces distintas y pregúntale a alguien a cuál le cree más.

## 5 · Que hable *(opcional)*

Imagen + voz = un personaje que mueve la boca. Este es el paso frágil de la sesión: las herramientas de *lip sync* tienen cupos gratuitos pequeños que cambian seguido.

| Herramienta | Cómo es su capa gratis |
|---|---|
| **HeyGen** | Pocos videos al mes, con marca de agua |
| **Hedra** | Gratis, pero con audio corto |
| **Vidnoz** | Más cupo diario, siempre con marca de agua |
| **Google Vids** | Avatares gratis para cuentas personales, pero el despliegue va por países |

Prueba una. Si no funciona, la siguiente. **Si ninguna te funciona hoy, no pasa nada**: el video queda bien con el personaje quieto, un zoom lento y buenos subtítulos. No te quedes veinte minutos peleando con un cupo.

## 6 · El montaje

En CapCut, en este orden:

1. El ambiente como fondo.
2. Encima, tu avatar. Si tiene fondo gris, usa **quitar fondo**.
3. Debajo de todo, el audio de la voz.
4. **Corta los silencios largos.** Es lo que más mejora un video.
5. **Subtítulos automáticos** — y revísalos: siempre hay dos o tres palabras mal.
6. Música de fondo al 10 o 15 % del volumen. Si compite con la voz, está muy alta.
7. Un zoom lento sobre la imagen hace que algo quieto se vea vivo.

Música muy alta y subtítulos sin revisar son las dos marcas de un video amateur. Arreglar esas dos cosas te sube el resultado más que cualquier efecto.

---

## 🎬 El encargo

Elige uno de los dos:

| | |
|---|---|
| **Qué hago en mi carrera** | Un día normal de trabajo de alguien de tu programa. Lo que nadie se imagina que haces. |
| **Lo que me costó entender** | Un concepto que te costó, explicado como te hubiera gustado que te lo explicaran. |

De 60 a 90 segundos, con tu personaje, tu ambiente y tu voz. Y al final, una línea diciendo qué hiciste con IA.
