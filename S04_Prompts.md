---
title: Sesión 4 · Prompts pro y tu primer agente
---
# Sesión 4 · Prompts de nivel pro y tu primer agente 🗣️🤖

> *"La IA no lee tu mente. Lee tu prompt."*

## 🧰 Herramientas del día

| Herramienta | Para qué la usamos hoy | Enlace | Costo |
|---|---|---|---|
| **Gems** (Gemini) | Crear un asistente con instrucciones y archivos propios | [gemini.google.com/gems](https://gemini.google.com/gems) | Gratis |
| **Proyectos** (Claude) | Lo mismo, en Claude, con documentos de contexto | [claude.ai/projects](https://claude.ai/projects) | Gratis |
| **Gandalf** (Lakera) | Entender qué es la inyección de prompts jugando | [gandalf.lakera.ai](https://gandalf.lakera.ai) | Gratis |
| **Google AI Studio** | Ver la *temperatura* y las *instrucciones de sistema* por dentro | [aistudio.google.com](https://aistudio.google.com) | Gratis |

## 🎯 Objetivos

* Dominar la estructura de un buen prompt: **rol + contexto + tarea + formato + ejemplos + restricciones**.
* Conocer técnicas: cadena de pensamiento, iteración, pedir preguntas antes de responder, *few-shot*.
* Crear tu **primer agente** (v0.1): un Gem o Proyecto con instrucciones y documentos de tu carrera.
* Entender por qué las instrucciones de sistema se pueden hackear (y por qué importa).

```{admonition} Cobertura PIIA
:class: note
Unidad 2 · c.iii. Redacción de prompts en IA · a. Conceptos generales.
```

## ⏱️ Agenda (2h30)

| Tiempo | Bloque | Qué pasa |
|---|---|---|
| 0:00 – 0:15 | 🧙 **Gandalf, nivel 4** | Todos intentan el nivel 4 (10 min). Quien lo pase explica cómo. Nombramos la técnica: *prompt injection* |
| 0:15 – 0:45 | 📐 **Anatomía de un prompt** | Del prompt malo al prompt pro en vivo, con el mismo problema |
| 0:45 – 1:15 | ⚔️ **Actividad 1: Prompt Battle** | Torneo por parejas: mismo objetivo, gana el mejor resultado |
| 1:15 – 1:25 | ☕ Pausa | |
| 1:25 – 1:45 | 🎛️ **Por dentro: AI Studio** | Instrucciones de sistema, temperatura, tokens. Qué es un "agente" y por qué un Gem ya lo es (v0.1) |
| 1:45 – 2:20 | 🤖 **Actividad 2: Tu primer agente** | Crear un Gem / Proyecto para tu carrera |
| 2:20 – 2:30 | 🏁 Cierre | Qué construimos hoy: tu Gem es el corazón del Ejercicio 1. La próxima sesión le exigimos fuentes reales |

## 📐 Anatomía de un prompt

| Pieza | Pregunta que responde | Ejemplo |
|---|---|---|
| **Rol** | ¿Quién quiero que sea? | "Eres un fisioterapeuta deportivo con 15 años de experiencia" |
| **Contexto** | ¿Qué necesita saber? | "Trabajo con corredores amateur de 40–55 años en Manizales (2.150 msnm)" |
| **Tarea** | ¿Qué debe hacer exactamente? | "Diseña un plan de fortalecimiento de 4 semanas" |
| **Formato** | ¿Cómo lo quiero? | "En una tabla: semana, ejercicio, series, repeticiones, señal de alarma" |
| **Ejemplos** | ¿Cómo se ve un buen resultado? | "Por ejemplo: Semana 1 · Sentadilla · 3 × 12 · dolor de rodilla" |
| **Restricciones** | ¿Qué NO debe hacer? | "No uses ejercicios que requieran gimnasio. Máximo 400 palabras" |
| **Verificación** | ¿Cómo sé que es confiable? | "Al final, di qué afirmaciones deberían confirmarse con un médico" |

Técnicas extra que veremos en vivo:

* **Pregúntame primero:** "Antes de responder, hazme 3 preguntas para entender mejor mi caso."
* **Paso a paso:** "Razona paso a paso antes de dar la respuesta final."
* **Iterar:** "Ahora hazlo más corto / más técnico / para un niño de 10 años."
* **Crítico:** "Ahora critica tu propia respuesta como si fueras un jurado exigente."

## ⚔️ Actividad 1: Prompt Battle (30 min)

En parejas, con el mismo objetivo y la misma IA. Tres rondas de 7 minutos; entre rondas, cada pareja mejora su prompt.

| Ronda | Reto (elige por carrera) |
|---|---|
| 1 | Explicar un concepto difícil de tu carrera a un estudiante de primer semestre, en 150 palabras, con una analogía cotidiana |
| 2 | Redactar un correo formal de 5 líneas a una institución pidiendo acceso a datos / a un archivo / a una instalación deportiva |
| 3 | Generar un examen de 5 preguntas de opción múltiple con retroalimentación por opción |

El grupo vota el mejor resultado de cada ronda. **Regla:** el ganador debe mostrar su prompt y explicar qué pieza de la anatomía hizo la diferencia.

## 🤖 Actividad 2: Tu primer agente (35 min)

Un agente, en su versión más simple, es **un modelo + instrucciones permanentes + documentos de contexto + (después) herramientas**. Hoy montamos los tres primeros.

1. Entra a **Gems** (o a **Proyectos** en Claude) y crea uno llamado `Tutor de [tu carrera]` o `Asistente de [tu trabajo]`.
2. Escribe las instrucciones usando la anatomía: rol, contexto (quién eres tú, qué estudias), cómo debe responder siempre (idioma, formato, nivel), qué **nunca** debe hacer (inventar fuentes, dar diagnósticos, etc.).
3. Adjunta 2–3 documentos de tu carrera (el PDF de la Sesión 2 sirve).
4. Pruébalo con 5 preguntas. Ajusta las instrucciones hasta que responda como quieres.
5. Comparte el Gem con un compañero de otra carrera: que lo pruebe y te diga qué falló.

Ideas por carrera:

* *Biología:* "Asistente de laboratorio" que conoce tus protocolos y responde en pasos.
* *Derecho:* "Redactor de derechos de petición" que siempre pide los hechos antes de redactar.
* *Artes:* "Curador crítico" que analiza referentes y propone lecturas.
* *Deporte:* "Planificador de entrenamiento" que siempre pregunta lesiones previas.

```{admonition} Ruta pro 🧗
:class: tip
En **Google AI Studio** replica tu Gem: pega las mismas instrucciones en *System instructions*, sube 0.2 → 1.0 la **temperatura** y compara. Luego pide *Get code*: ese código es tu agente listo para vivir fuera del chat (lo usaremos en S13 y S15).
```

## 📦 Lo que te llevas

Tu Gem/Proyecto (el corazón del **Ejercicio 1**) y tu mejor prompt de la Prompt Battle en el tablero, con una línea explicando por qué funcionó.
