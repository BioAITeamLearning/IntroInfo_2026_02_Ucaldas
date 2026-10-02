# Sesiones pendientes · guía de trabajo para Santiago

Hola Santiago. Este documento resume qué es este curso, qué decisiones ya están tomadas, en qué estado está cada sesión y cómo seguir. Léelo antes de tocar cualquier archivo.

## 1. Qué es esto

**Introducción a la Informática (40G8F)** · Universidad de Caldas · 2026-2 · Johan Piña. Estudiantes de carreras muy variadas (biología, derecho, artes, deporte…), **no ingenieros**. 16 semanas, una sesión semanal de **2h30**.

Johan tiene libertad de cátedra y decidió **renovar el PIIA oficial** (5 unidades: TIC · Sociedad de la información · Uso y apropiación · Datos · IA profesional) con una idea rectora:

> **Cada sesión conocemos y usamos una herramienta de IA distinta, haciendo algo real aplicado a la carrera de cada estudiante, y saliendo de clase con algo construido.**

Lo que queremos que sepan hacer al final: usar asistentes con criterio, chatear con sus PDFs, publicar su página web, montar un sistema de gestión sin código, analizar datos con IA, crear agentes y automatizar. Y que agentes / análisis de carpetas / automatizaciones aparezcan **desde la Unidad 1**, no solo al final.

* Libro publicado: https://bioaiteamlearning.github.io/IntroInfo_2026_02_Ucaldas/
* Repo: https://github.com/BioAITeamLearning/IntroInfo_2026_02_Ucaldas
* Estilo: Jupyter Book (MyST), igual que el repo de Técnicas de Programación (`TecDeProg_2026_02_Ucaldas`).

## 2. Decisiones ya tomadas (no reabrir sin hablar con Johan)

| Tema | Decisión |
|---|---|
| **Evaluación** | Tres ejercicios, tres notas, y ya (así lo pide el PIIA: talleres, sustentación en grupo, práctica en computador, internet como difusión). **Ejercicio 1 · Mi asistente de carrera** (30%, se sustenta en S6) · **Ejercicio 2 · Mi sistema publicado** (35%, S12) · **Ejercicio 3 · Mi agente** (35%, S16 Demo Day). Los talleres de cada sesión **no se califican**: son las piezas de los ejercicios. |
| **Sin tareas para la casa** | Todo se hace en clase: cuentas, instalaciones, documentos, datos, fotos. Si una sesión necesita algo, se consigue dentro de la sesión. |
| **Lo que ven los estudiantes** | Las páginas del libro llevan **solo contenido y actividades**: herramientas del día, objetivos, contenido conceptual mínimo, actividades, material, "lo que te llevas". **Nada** de agenda, tiempos, minutos, tips de clase, "conclusión guiada", cobertura PIIA ni menciones al docente. |
| **Lo que solo ve el docente** | Carpeta `docente/` (está en `.gitignore`, **solo existe en el Mac de Johan**): `SNN_guia.md` con cobertura PIIA, agenda 2h30, preparación previa, prompts exactos de las demos, notas por diapositiva, tiempos, riesgos y plan B. Pídele a Johan que te la comparta por Drive. |
| **Sesiones apagadas** | Solo se publica hasta la sesión que se va a dictar. Las demás viven en `pendientes/` (esta carpeta), excluida del build. Se "prenden" una a una (ver §5). |
| **Nombre del curso** | "Introducción a la Informática" (el del PIIA), aunque la carpeta local se llame IntroIngenieria. |
| **Herramientas** | Solo con plan gratuito, y preferiblemente las que ya vienen con la cuenta institucional de Google (Gemini, NotebookLM, Drive, AppSheet, Looker Studio, AI Studio, Colab). Se verifican la semana anterior porque cambian. |
| **Regla de oro** | "Nada confidencial en un chat de IA". Aparece en cada sesión donde aplique. |

## 3. Estado de cada sesión

| # | Sesión | Estado | Qué le falta |
|---|---|---|---|
| 1 | Fundamentos de TIC | ✅ Dictada (formato clásico, ya publicada) | — |
| 2 | Tu nuevo kit de superpoderes | ✅ Dictada el 11 sep. Publicada con diapositivas y guía (`_static/sesion02/`) | Recoger qué "superpoder" quisieron aprender (está en el tablero) para ajustar ejemplos |
| 3 | Tu vida digital: segura, ordenada y con IA | 🟡 **Completa, sin prender**: página + `sesion03/slides.html` + `sesion03/guia.html` + guía docente | Probar Gemini en Drive y 2FA con la cuenta institucional antes de dictarla |
| 4 | Prompts pro y tu primer agente (Gems) | 🔵 Página lista y limpia | Diapositivas, guía imprimible (tarjetas de la Prompt Battle), guía docente con demos |
| 5 | Investigar con IA (Deep Research, Consensus, Zotero) | 🔵 Página lista y limpia | Diapositivas, las 10 afirmaciones de la "carrera de verificación" (5 reales, 3 falsas, 2 medio ciertas), guía docente |
| 6 | Ética, deepfakes y planeta · **sustentación Ejercicio 1** | 🔵 Página lista y limpia | Diapositivas, formato de sustentación en parejas, guía docente |
| 7 | Tu página web (Sites + Lovable + GitHub Pages) | 🔵 Página lista y limpia | Diapositivas, guía docente, probar Lovable/Bolt con cuentas gratuitas |
| 8 | Multimedia con IA (Canva, Gamma, Veo, ElevenLabs, CapCut) | 🔵 Página lista y limpia | Diapositivas, guía docente, verificar límites gratuitos de ElevenLabs/Suno |
| 9 | Sistemas de gestión sin código (AppSheet + Apps Script) | 🔵 Página lista y limpia | Diapositivas, hoja de ejemplo por carrera, script de Apps Script probado, guía docente |
| 10 | Obtener y limpiar datos (Sheets + Gemini, datos.gov.co) | 🔵 Página lista y limpia | Diapositivas, 4 datasets de datos.gov.co pre-seleccionados (uno por carrera), guía docente |
| 11 | Analizar con IA (Colab Data Science Agent, Gemini CLI) | 🔵 Página lista y limpia | Diapositivas, notebook de Colab plantilla, guía docente |
| 12 | Dashboards y data storytelling · **sustentación Ejercicio 2** | 🔵 Página lista y limpia | Diapositivas, "8 gráficos: ¿cuál miente?", guía docente |
| 13 | Cómo funciona la IA (Teachable Machine, Transformer Explainer, AI Studio) | 🔵 Página lista y limpia | Diapositivas, guía docente |
| 14 | Agentes (Gemini CLI / Claude Code + Opal) | 🔵 Página lista y limpia | Diapositivas, carpeta `agente/` de ejemplo, `GEMINI.md` de ejemplo, guía docente |
| 15 | Automatizaciones y bots (n8n + Telegram + Gemini API) | 🔵 Página lista y limpia | Diapositivas, **plantilla de n8n exportada** (bot Telegram + PDFs), alternativa Apps Script probada, guía docente |
| 16 | Demo Day · **sustentación Ejercicio 3** | 🔵 Página lista y limpia | Formulario de retroalimentación entre pares, orden de demos |
| — | Unidades 2–5 y Proyecto final | 🔵 Páginas listas | Se prenden con la primera sesión de cada unidad |

"Página lista y limpia" = ya tiene la estructura estándar y ya se le quitó todo lo orientado al docente (agenda, tiempos, PIIA), que quedó en `docente/SNN_guia.md` (versión mínima: cobertura PIIA + agenda + tiempos; falta enriquecerla como la de S2 y S3).

## 4. Cómo se arma una sesión (el patrón de S2 y S3)

Para cada sesión, **cuatro piezas**:

1. **Página del estudiante** (`SNN_Slug.md`), en este orden: frase gancho · 🧰 Herramientas del día (tabla: herramienta, para qué, enlace, costo) · 🎯 Objetivos · contenido conceptual mínimo (tablas, comparativas, "lo mínimo") · actividades numeradas con pasos y prompts listos para copiar, con ejemplos **por carrera** (biología, derecho, artes, deporte) · caja "Ruta pro 🧗" opcional (normalmente terminal/agentes) · 📽️ Material (enlaces a slides y guía) · 📦 Lo que te llevas (siempre conectado con el ejercicio del corte).
2. **Diapositivas** (`_static/sesionNN/slides.html`): HTML autocontenido, sin dependencias externas (funciona sin internet). Copiar el `<head>`, el CSS y el `<script>` de `_static/sesion02/slides.html` y cambiar solo las `<section>`. Teclas: flechas, `F` pantalla completa, `T` cronómetro. **Sin notas de docente ni duraciones.**
3. **Guía imprimible** (`_static/sesionNN/guia.html`): páginas A4 por actividad con pasos, prompts, casillas y espacios para anotar. Base: `_static/sesion02/tarjetas.html`.
4. **Guía docente** (`docente/SNN_guia.md`, no versionada): cobertura PIIA · agenda 2h30 · preparar antes de clase · demos con prompt exacto y "qué señalar" · notas por diapositiva · tiempos · riesgos y plan B. Modelo: `docente/S03_guia.md`.

Mientras la sesión esté apagada, las piezas 1–3 viven en `pendientes/` (`pendientes/SNN_Slug.md` y `pendientes/sesionNN/`).

### Para que sean dinámicas (lo que ha funcionado)

* **Empezar con un juego** relacionado (Quick Draw, Gandalf, Moral Machine, Detect Fakes, Gapminder, Seeing Theory, Teachable Machine…). Ya hay uno asignado por sesión en la página.
* **Nunca más de ~25 minutos seguidos** de docente hablando. El contenido conceptual va en tablas cortas, no en párrafos.
* **Demo en vivo antes de la actividad**: "yo hago, ustedes miran" → "hacemos juntos" → "ustedes lo aplican a su carrera".
* **Todo aplicado a la carrera del estudiante**: cada actividad trae ejemplos para biología, derecho, artes y deporte (si aparecen otras carreras en el grupo, agregar).
* **Puesta en común al final**: mostrar, votar, reírse de lo que la IA inventó.
* **Salir con algo construido** y saber para qué ejercicio sirve.

## 5. Flujo de trabajo

```bash
# construir localmente (usa el venv del repo de Técnicas)
/Users/johanpina/dev/tecnicas/.venv/bin/jupyter-book build .
open _build/html/index.html

# publicar: GitHub Actions construye y despliega en cada push a main (~40 s)
git add <archivos que tocaste>     # no usar git add -A: cualquier .md en la raíz se publica aunque no esté en el _toc.yml
git commit -m "..."
git push
```

**Prender una sesión** (cuando se va a dictar):

```bash
mv pendientes/S04_Prompts.md .
mv pendientes/sesion04 _static/sesion04        # si existe
# primera sesión de una unidad: también mv pendientes/UnidadN.md .
```

Luego: agregar `- file: "S04_Prompts"` en `_toc.yml` bajo su unidad; en `MapaDelCurso.md` volver a poner el enlace (`{doc}`S04_Prompts``) en la fila de la sesión; en `intro.md`, si es unidad nueva, devolverle `:link: UnidadN` / `:link-type: doc` a la card; en `UnidadN.md` enlazar la sesión en la tabla. Construir, revisar, push.

**Ojo con el historial**: las sesiones 3–16 están en el historial de git (commits del 10–11 sep) y ahora también en `pendientes/`; el repo es público, así que un estudiante curioso podría leerlas en GitHub. Johan lo sabe; lo que importa es que no estén en el libro.

## 6. Pendientes concretos, en orden

1. **Sesión 3** (próxima): Johan prueba Gemini en Drive y 2FA con la cuenta institucional. Si algo no está disponible, aplicar el plan B de `docente/S03_guia.md`. Prender y publicar el día de la clase.
2. **Sesión 4**: diapositivas + tarjetas de la Prompt Battle (3 rondas, por carrera) + guía docente. Es la sesión donde crean el Gem: corazón del Ejercicio 1.
3. **Sesión 5**: preparar las 10 afirmaciones de la carrera de verificación con fuentes primarias; diapositivas; guía docente.
4. **Sesión 6**: diseñar la sustentación del Ejercicio 1 (parejas de carreras distintas, 3 preguntas: una que está, una que no, una trampa) y cómo registrar la nota.
5. De la 7 en adelante, mismo patrón. Prioridad a lo que requiere prueba técnica previa: Lovable/Bolt (S7), AppSheet + Apps Script (S9), Colab Data Science Agent y Gemini CLI (S11), n8n + Telegram (S15).
6. **Transversal**: crear el "tablero compartido del curso" donde pegan enlaces y respuestas (hoy es informal; puede ser un Google Sheet o un Padlet).
7. **Transversal**: Santiago en la card de "El equipo" en `intro.md` (falta foto en `_static/images/` y correo).
