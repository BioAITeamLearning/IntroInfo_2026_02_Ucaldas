---
title: Sesión 3 · Tu vida digital
---
# Sesión 3 · Tu vida digital: segura, ordenada y con IA 🔐📂

> *"Tu información vale más que tu computador. Hoy la protegemos, la ordenamos y le ponemos una IA encima."*

## 🧰 Herramientas del día

| Herramienta | Para qué la usamos hoy | Enlace | Costo |
|---|---|---|---|
| **Gandalf** (Lakera) | Juego: engañar a una IA para que revele su contraseña | [gandalf.lakera.ai](https://gandalf.lakera.ai) | Gratis |
| **Have I Been Pwned** | Saber si tu correo está en filtraciones | [haveibeenpwned.com](https://haveibeenpwned.com) | Gratis |
| **Bitwarden** | Gestor de contraseñas (computador + celular) | [bitwarden.com](https://bitwarden.com) | Gratis |
| **Gemini en Drive** | Preguntarle a una carpeta entera de documentos | [drive.google.com](https://drive.google.com) | Gratis (institucional) |
| **NotebookLM** | Tu biblioteca personal consultable, con 10+ fuentes | [notebooklm.google.com](https://notebooklm.google.com) | Gratis |
| **Scaniverse** / **Sketchfab** | Realidad extendida: escanear un objeto en 3D con el celular y verlo en AR | [scaniverse.com](https://scaniverse.com) · [sketchfab.com](https://sketchfab.com) | Gratis |

## 🎯 Objetivos

* Entender cómo se roba una cuenta y blindar las tuyas: contraseñas únicas, gestor y verificación en dos pasos.
* Saber dónde vive tu información (local, nube, celular), qué hace el sistema operativo con ella y organizarla con un sistema que sirva.
* Hacer tu **primer análisis de una carpeta** de documentos con IA (Gemini en Drive y NotebookLM).
* Probar realidad extendida con tu celular.

## 🧙 Calentamiento: Gandalf

Entra a [gandalf.lakera.ai](https://gandalf.lakera.ai). Gandalf es una IA que tiene una contraseña secreta y la instrucción de no revelarla. Tu misión: **que te la diga**. Intenta pasar los niveles 1 a 3.

Lo que estás haciendo tiene nombre (*prompt injection*) y lo vas a volver a ver: una IA se puede engañar con palabras, igual que a una persona se le engaña con un correo falso. Por eso importa lo que viene ahora.

## 🔓 Cómo te roban una cuenta (lo mínimo)

No hace falta un hacker con capucha. Casi siempre es esta cadena:

| Paso | Qué pasa | Ejemplo |
|---|---|---|
| 1. **Filtración** | Una empresa pierde su base de datos y tu correo + contraseña quedan en listas que se venden o se publican | LinkedIn (2012), Adobe (2013), Canva (2019), Dropbox, MyFitnessPal… |
| 2. **Reuso** | Alguien prueba esa misma contraseña en tu Gmail, Instagram, banco, plataforma de la U | Se llama *credential stuffing* y es automático: millones de intentos por hora |
| 3. **Entran** | Si reusaste la contraseña y no tienes segundo factor, ya está | Cambian la clave, piden préstamos a tus contactos, borran tus archivos |

Y el atajo cuando no hay filtración: **phishing**. Un correo o WhatsApp que parece de la universidad, del banco o de una entrega, con un enlace a una página idéntica a la real donde tú mismo escribes tu contraseña.

### Lo que de verdad protege

| Defensa | Por qué funciona |
|---|---|
| **Una contraseña distinta por sitio** | Una filtración deja de abrir todas tus puertas |
| **Un gestor de contraseñas** | Es la única forma humana de tener 80 contraseñas distintas y largas. Tú recuerdas una sola (la maestra) |
| **Verificación en dos pasos (2FA)** | Aunque tengan tu contraseña, les falta tu celular. Mejor con app o *llave de acceso (passkey)* que con SMS |
| **Longitud > complejidad** | `Tr0ub4dor&3` se rompe en horas; `caballo correcto batería grapa` tarda siglos. Una frase larga que recuerdes vence a un símbolo raro |
| **Revisar sesiones y permisos** | Google → Seguridad → *Tus dispositivos*: si hay algo que no reconoces, ciérralo |
| **Desconfiar del enlace** | Antes de escribir una contraseña, mira la URL. Si llegó por mensaje, entra por tu cuenta, no por el enlace |

## 🔐 Actividad 1: Blindaje digital

Lista de chequeo (se hace en clase, con acompañamiento):

- [ ] Revisar tu correo en [Have I Been Pwned](https://haveibeenpwned.com). ¿En cuántas filtraciones apareces? ¿Alguna con contraseña que todavía usas?
- [ ] Instalar **Bitwarden** (extensión del navegador + app del celular) y crear la contraseña maestra: una frase larga de 4–5 palabras que recuerdes y que no esté en ningún otro sitio.
- [ ] Cambiar la contraseña de tu correo institucional y personal por una **generada** por Bitwarden.
- [ ] Activar **verificación en dos pasos** en Google: llave de acceso (*passkey*) o app de autenticación (Google Authenticator / Bitwarden).
- [ ] Revisar en Google → Seguridad → *Tus dispositivos* qué sesiones están abiertas y cerrar las que no reconoces.
- [ ] Celular: bloqueo con huella/rostro, copia de seguridad activada, *Buscar mi dispositivo* activado.
- [ ] Revisar los **permisos de las apps** (cámara, micrófono, ubicación): ¿cuáles no tienen por qué tenerlos?
- [ ] Revisar el panel de **bienestar digital** del celular: ¿cuántas horas y en qué?

```{warning}
Regla de oro para el resto del curso: **nada confidencial en un chat de IA**: datos de pacientes, expedientes con nombres, contraseñas, cuentas bancarias. Si necesitas analizar datos sensibles, se anonimizan primero (lo vemos en la Unidad 4).
```

## 📂 ¿Dónde vive tu información?

Tu información está en tres lugares a la vez, y cada uno falla distinto:

| Lugar | Qué guarda | Cómo se pierde | Cómo se protege |
|---|---|---|---|
| **Local** (disco del computador) | Lo que descargas, tus proyectos, fotos importadas | Se daña el disco, te roban el equipo, borras sin querer | Copia en la nube + un disco externo |
| **Nube** (Drive, iCloud, OneDrive) | Documentos, fotos sincronizadas, correo | Te roban la cuenta (por eso el blindaje), la empresa cierra tu cuenta | 2FA + exportar de vez en cuando (Google Takeout) |
| **Celular** | Fotos, chats, autenticación, todo | Se pierde, se rompe, se moja | Copia automática + bloqueo + *Buscar mi dispositivo* |

Regla **3-2-1** en versión estudiante: tres copias de lo importante (computador, nube, disco externo o segundo servicio), en dos tipos de medio, una fuera de tu casa.

### El sistema operativo: el portero de tus archivos

Windows, macOS y Linux en el computador; Android e iOS en el celular. Hacen lo mismo con tu información: la guardan en carpetas, deciden qué programa puede tocar qué (permisos), la respaldan si se lo pides y la cifran si lo activas (BitLocker / FileVault / cifrado del celular). Dos hábitos que valen más que cualquier antivirus: **actualizar** cuando lo pide y **revisar permisos** de lo que instalas.

### Un sistema de carpetas que funcione: PARA

Las carpetas "Cosas", "Nueva carpeta (2)" y "Descargas" no son un sistema. Este sí, y sirve igual en Drive y en el computador:

| Carpeta | Qué va ahí | Ejemplo |
|---|---|---|
| **P · Proyectos** | Lo que tiene fecha de entrega | `Tesis`, `Exposición-noviembre`, `Caso-Pérez`, `Temporada-2026` |
| **A · Áreas** | Responsabilidades sin fecha final | `Laboratorio`, `Clientes`, `Colectivo`, `Atletas` |
| **R · Recursos** | Referencias que consultas | `Artículos`, `Leyes`, `Referentes`, `Plantillas` |
| **A · Archivo** | Lo terminado o inactivo | Proyectos cerrados de semestres pasados |

Y un nombre de archivo que se entienda dentro de un año: `AAAA-MM-DD_tema_tipo` → `2026-09-13_protocolo-PCR_guia.pdf`. En la Sesión 14 un agente va a renombrar y organizar tu carpeta con esta regla; hoy la empiezas tú.

## 🤖 Actividad 2: Pregúntale a tu carpeta

**Parte A — Gemini en Drive.** Crea en Drive la estructura PARA y pon en `Recursos/` al menos 5 documentos de tu carrera (PDFs de tu correo, del Drive viejo, o buscados con `filetype:pdf`). Abre el panel de Gemini en Drive, dentro de esa carpeta, y prueba:

* "Resume los documentos de esta carpeta en una tabla: título, tema, fecha."
* "¿Cuáles de estos documentos hablan de [concepto]?"
* "Propón un nombre para cada archivo con el formato AAAA-MM-DD_tema_tipo."
* "Escribe un correo a mi profesor pidiendo aclaración sobre lo que dice el documento X."

**Parte B — NotebookLM como biblioteca.** En tu cuaderno de la Sesión 2 agrega primero **7–10 fuentes más**: usa *Descubrir fuentes* de NotebookLM con un tema de tu carrera y suma los PDFs de tu carpeta `Recursos/`. Luego:

* Pide un **Informe** tipo "guía de estudio" de todo el cuaderno.
* Pide una **Tabla de datos** comparando las fuentes según un criterio de tu carrera (por ejemplo: método, población, año).
* Pide un **Mapa mental** y expándelo: ¿qué conexiones no habías visto?
* Reto: toma **una afirmación** del informe y verifica en la cita si realmente lo dice la fuente.

```{admonition} Ruta pro 🧗
:class: tip
Si ya instalaste Node y Gemini CLI, abre la terminal **dentro** de tu carpeta `Recursos/` y escribe `gemini`. Luego: *"Lista los archivos de esta carpeta y dime de qué trata cada uno en una línea. No modifiques nada."* Ese es un agente leyendo tu disco. Lo hacemos todos en la Sesión 14.
```

## 🥽 Actividad 3: Tu objeto en 3D

1. Instala **Scaniverse** en el celular y escanea un objeto (un hueso de la colección, un libro, una escultura, un balón): gira despacio alrededor, 1–2 minutos.
2. Explóralo en **realidad aumentada** sobre la mesa y compártelo como enlace.
3. Entra a [Sketchfab](https://sketchfab.com) desde el celular, busca un modelo de tu área (anatomía, patrimonio, arquitectura, biomecánica) y ábrelo en AR.

Para pensar: *¿qué cambia en tu profesión cuando cualquier objeto se puede digitalizar en 2 minutos y cualquier documento se puede consultar en lenguaje natural?*

## 📽️ Material

* <a href="_static/sesion03/slides.html" target="_blank">Diapositivas de la sesión</a>
* <a href="_static/sesion03/guia.html" target="_blank">Guía de las actividades</a>

## 📦 Lo que te llevas

Tu cuenta blindada (gestor + 2FA), tu Drive con estructura PARA y tu cuaderno de NotebookLM con 10+ fuentes: la biblioteca de tu **Ejercicio 1**. En el tablero: la afirmación que verificaste (¿era cierta?) y el enlace a tu objeto en 3D.
