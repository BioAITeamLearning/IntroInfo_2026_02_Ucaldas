---
title: Sesión 14 · Agentes
---
# Sesión 14 · Agentes: crearlos y correrlos sobre tus archivos 🤖📂

> *"Un chat responde. Un agente lee tu carpeta, decide qué hacer, lo hace y te cuenta. Hoy sueltas uno en tu computador."*

## 🧰 Herramientas del día

| Herramienta | Para qué la usamos hoy | Enlace | Costo |
|---|---|---|---|
| **Gemini CLI** | Agente en la terminal que lee, escribe y ejecuta en tu carpeta | [github.com/google-gemini/gemini-cli](https://github.com/google-gemini/gemini-cli) | Gratis (cuenta Google) |
| **Claude Code** (alternativa) | Lo mismo, con Claude | [claude.com/claude-code](https://claude.com/claude-code) | Requiere plan / API |
| **Opal** (Google Labs) | Crear mini-apps y flujos de agentes **sin código**, con bloques | [opal.withgoogle.com](https://opal.withgoogle.com) | Gratis |
| **Gems / Proyectos** (repaso) | Agente v0.1: instrucciones + documentos | [gemini.google.com/gems](https://gemini.google.com/gems) | Gratis |
| **NotebookLM** (repaso) | Agente de lectura: 50 fuentes, cita exacta | [notebooklm.google.com](https://notebooklm.google.com) | Gratis |

## 🎯 Objetivos

* Definir agente: **modelo + instrucciones + herramientas + bucle** (observa → piensa → actúa → verifica).
* Correr un agente **en la terminal sobre una carpeta real**: leer, clasificar, renombrar, resumir, generar documentos.
* Aprender a **delegar con seguridad**: modo de solo lectura primero, revisar el plan, confirmar cada cambio, tener respaldo.
* Crear un agente **sin código** con Opal para un flujo de tu carrera.
* Escribir un archivo de instrucciones (`GEMINI.md` / `CLAUDE.md`) que convierte a tu carpeta en un espacio de trabajo con reglas.

```{admonition} Cobertura PIIA
:class: note
Unidad 5 · b. Herramientas esenciales · c.a. Redacción de documentos · c.c. Estructuración del conocimiento · Unidad 3 · a. Agentes inteligentes sobre bases de datos/documentos.
```

## ⏱️ Agenda (2h30)

| Tiempo | Bloque | Qué pasa |
|---|---|---|
| 0:00 – 0:20 | 🩺 **Instalación y carpeta** | Instalar Node.js + Gemini CLI ({doc}`KitDeCuentas`) y crear una carpeta `agente/` con 10–20 archivos reales desordenados (descargar PDFs, imágenes y hojas de Drive/correo). Quien no pueda instalar, trabaja en pareja o con Opal |
| 0:20 – 0:35 | 🔁 **¿Qué es un agente?** | El bucle observa-piensa-actúa con un ejemplo humano (un asistente que ordena tu oficina). Demo en vivo: el docente suelta Gemini CLI en una carpeta caótica |
| 0:35 – 1:15 | 📂 **Actividad 1: El agente ordena tu carpeta** | Solo lectura → plan → ejecutar con confirmación |
| 1:15 – 1:25 | ☕ Pausa | |
| 1:25 – 1:50 | 📝 **Actividad 2: El agente redacta por ti** | Del contenido de la carpeta a un documento estructurado |
| 1:50 – 2:15 | 🧱 **Actividad 3: Agente sin código con Opal** | Un flujo de 3–4 pasos para tu carrera |
| 2:15 – 2:30 | 🛡️ **Seguridad y cierre** | Qué nunca dejar hacer a un agente |

## 🔁 ¿Qué es un agente?

| Pieza | En un chat (S2) | En un Gem (S4) | En AI Studio (S13) | En Gemini CLI (hoy) |
|---|---|---|---|---|
| Modelo | ✅ | ✅ | ✅ | ✅ |
| Instrucciones permanentes | ❌ | ✅ | ✅ | ✅ (`GEMINI.md`) |
| Documentos de contexto | subes uno | ✅ | ✅ | **toda la carpeta** |
| Herramientas | ❌ | ❌ | búsqueda, código | **leer, escribir, ejecutar, buscar** |
| Bucle autónomo | ❌ | ❌ | un paso | **planea y ejecuta varios pasos** |

## 📂 Actividad 1: El agente ordena tu carpeta (40 min)

**Antes de empezar:** copia la carpeta `agente/` a `agente_respaldo/`. Siempre.

```bash
cd agente
gemini
```

**Paso 1 — Solo mirar (nada se modifica):**

> *"No modifiques ningún archivo. Lista todo lo que hay en esta carpeta y, para cada archivo, dime en una línea de qué trata (abre los PDFs e imágenes si hace falta). Al final propón una estructura de subcarpetas y un esquema de nombres `AAAA-MM-DD_tema_tipo` para organizar todo. Preséntame el plan como una tabla: nombre actual → nombre nuevo → carpeta."*

**Paso 2 — Revisar el plan:** lee la tabla. ¿Clasificó bien? Corrige: *"El archivo X no es una factura, es un protocolo; muévelo a…"*.

**Paso 3 — Ejecutar con confirmación:**

> *"Ejecuta el plan. Antes de cada renombrado o movimiento pídeme confirmación."*

**Paso 4 — Verificar:** *"Muéstrame el árbol final de la carpeta y genera un `INDICE.md` con una línea por archivo."*

**Paso 5 — Reglas permanentes:** *"Crea un archivo `GEMINI.md` en esta carpeta con las reglas que seguiste (esquema de nombres, estructura, idioma) para que la próxima vez las apliques automáticamente."* Ábrelo: eso es la **memoria** de tu agente.

```{tip}
Si usas Claude Code el flujo es el mismo: `claude`, y el archivo de reglas se llama `CLAUDE.md`. Ambos preguntan antes de escribir o ejecutar; **nunca actives el modo "sin confirmaciones"** en carpetas que te importan.
```

## 📝 Actividad 2: El agente redacta por ti (25 min)

Sobre la misma carpeta ya ordenada, pide algo de tu carrera:

* *Biología:* *"Lee los protocolos de `laboratorio/` y escribe `resumen_protocolos.md` con una tabla: protocolo, reactivos, tiempo, riesgos."*
* *Derecho:* *"Lee los documentos de `caso_01/` y redacta una cronología de hechos con fecha, hecho y documento fuente."*
* *Artes:* *"Con las imágenes y textos de `obras/`, redacta la ficha técnica de cada obra y un texto curatorial de 300 palabras."*
* *Deporte:* *"Con los CSV de `sesiones/`, calcula la carga semanal por atleta y escribe un informe con alertas."*

Luego: *"Convierte el informe a un archivo `.docx` (o `.html`) y ábrelo."* Revisa **cada afirmación** contra el archivo fuente: el agente cita rutas, tú verificas.

## 🧱 Actividad 3: Agente sin código con Opal (25 min)

En [Opal](https://opal.withgoogle.com) describe un flujo, por ejemplo:

> *"Recibe un tema → busca 5 fuentes recientes → resume cada una en 3 líneas → genera un guion de 60 s para un video → propone 3 títulos."*

Opal lo convierte en bloques conectados que puedes editar. Ejecútalo con un tema de tu carrera y **compártelo como app**: ese enlace es un agente que otros pueden usar. Ponlo en tu página web.

## 🛡️ Seguridad al delegar en agentes

| Regla | Por qué |
|---|---|
| Respaldo antes, siempre | Un `rm` mal entendido no se deshace |
| Primero "solo lectura", luego plan, luego ejecutar | Ves lo que va a hacer antes de que lo haga |
| Confirmar cada acción destructiva | Renombrar/borrar/enviar |
| No darle acceso a carpetas con datos sensibles sin anonimizar | Datos personales (Ley 1581) |
| Nunca pegar claves ni contraseñas en el chat del agente | Quedan en el historial |
| Verificar lo redactado contra la fuente | Sigue siendo un modelo que predice |

## 📦 Lo que te llevas

`INDICE.md` + `GEMINI.md` (o `CLAUDE.md`) + el documento redactado por el agente **con tus correcciones marcadas** + enlace a tu app de Opal. Todo en tu página.
