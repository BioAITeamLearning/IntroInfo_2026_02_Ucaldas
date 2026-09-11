---
title: Sesión 9 · Sistemas de gestión sin código
---
# Sesión 9 · Tu sistema de gestión (sin código) + tu primera automatización 📱⚙️

> *"Lo que hoy gestionas en un grupo de WhatsApp y un Excel, en 2 horas es una app en tu celular con notificaciones."*

## 🧰 Herramientas del día

| Herramienta | Para qué la usamos hoy | Enlace | Costo |
|---|---|---|---|
| **Google AppSheet** | Convertir una hoja de cálculo en una app móvil/web, con IA | [appsheet.com](https://www.appsheet.com) | Gratis (institucional) |
| **Google Forms + Sheets** | Captura de datos y base de datos | [forms.google.com](https://forms.google.com) | Gratis |
| **Google Apps Script** | Automatizar: correos, recordatorios, cálculos (código generado por Gemini) | [script.google.com](https://script.google.com) | Gratis |
| **Gemini en Sheets** | Generar fórmulas, limpiar y clasificar datos | [sheets.google.com](https://sheets.google.com) | Gratis |
| **Notion** / **Airtable** (alternativa) | Bases de datos visuales con IA | [notion.so](https://notion.so) · [airtable.com](https://airtable.com) | Gratis (básico) |

## 🎯 Objetivos

* Entender qué es un **sistema de información**: datos (tabla) → reglas → vistas → acciones → notificaciones.
* Modelar tus datos: qué es una tabla, un registro, una clave, una relación (¡sin decir SQL!).
* Publicar una **app de gestión** funcionando en el celular con AppSheet.
* Crear tu **primera automatización**: un correo o recordatorio que se envía solo.

```{admonition} Cobertura PIIA
:class: note
Unidad 3 · c. Herramientas de gestión y seguimiento de información · Unidad 4 · a. Obtención y manipulación de información · Unidad 5 · c.b. Planeación.
```

## ⏱️ Agenda (2h30)

| Tiempo | Bloque | Qué pasa |
|---|---|---|
| 0:00 – 0:20 | 🧩 **¿Qué es un sistema de gestión?** | Juego con tarjetas: entidades (Atleta, Caso, Muestra, Obra) y relaciones. Del Excel caótico a la tabla limpia: una fila = un registro, una columna = un atributo, una columna que identifica (ID) |
| 0:20 – 0:40 | 🧹 **Actividad 1: Tu tabla, bien hecha** | Limpiar la hoja del reto con Gemini en Sheets; agregar ID, listas desplegables y validaciones |
| 0:40 – 1:15 | 📱 **Actividad 2: De la hoja a la app** | AppSheet: crear app, vistas, formulario, fotos, GPS, filtros |
| 1:15 – 1:25 | ☕ Pausa | |
| 1:25 – 1:45 | ⚙️ **¿Qué es una automatización?** | Disparador → condición → acción. Ejemplos en su vida. Demo: Apps Script escrito por Gemini |
| 1:45 – 2:15 | 🤖 **Actividad 3: Tu primera automatización** | Correo automático o bot en AppSheet |
| 2:15 – 2:30 | 📲 **Demo cruzada** | Instala la app de un compañero de otra carrera. Feedback y cierre |

## 🧹 Actividad 1: Tu tabla, bien hecha (20 min)

Abre la hoja del reto y aplica:

1. Fila 1 = nombres de columna cortos y sin tildes (`nombre`, `fecha_ingreso`, `estado`).
2. Columna `id` única (puedes usar `=ROW()` o dejar que AppSheet la genere).
3. **Validación de datos** en `estado` (lista: *activo, pendiente, cerrado*).
4. Gemini en Sheets: *"Detecta inconsistencias en esta tabla (fechas mal escritas, duplicados, mayúsculas) y sugiere correcciones."*
5. Prueba la función `=AI("Clasifica esta nota como urgente o normal", E2)` si está disponible en tu cuenta.

## 📱 Actividad 2: De la hoja a la app (35 min)

1. En Sheets: *Extensiones → AppSheet → Crear una app*. AppSheet detecta tipos (fecha, correo, imagen) y crea la app.
2. Ajusta: en *Data* revisa tipos; en *Views* crea una vista **tarjetas** o **calendario** y un **formulario**.
3. Agrega una columna `foto` (tipo Image) y `ubicacion` (tipo LatLong): tu app ya toma fotos y GPS.
4. Agrega un **filtro** (slice): "solo pendientes".
5. Prueba en el celular con la app de AppSheet. **Ya tienes un sistema de gestión.**

Ideas por carrera:

| Carrera | App | Tablas |
|---|---|---|
| Biología | Colecta de campo | Muestra (foto, GPS, especie, fecha) · Sitio |
| Derecho | Seguimiento de casos | Caso (cliente, estado, próxima audiencia) · Actuación |
| Artes | Inventario de obras / catálogo de exposición | Obra (foto, técnica, dimensiones, ubicación) · Exposición |
| Deporte | Control de atletas | Atleta (peso, lesiones) · Sesión (fecha, carga, RPE) |

## 🤖 Actividad 3: Tu primera automatización (30 min)

**Opción A — AppSheet Automation (sin código):** *Automation → New bot*: cuando se agregue un registro con `estado = urgente` → enviar correo al responsable. Pruébalo.

**Opción B — Apps Script escrito por Gemini:** en Sheets, *Extensiones → Apps Script*. Pídele a Gemini:

> *"Escribe un Google Apps Script para esta hoja (columnas: nombre, correo, fecha_limite, estado) que cada día a las 7 a.m. envíe un correo a cada persona cuya fecha_limite sea mañana y estado sea 'pendiente'. Explícame cómo instalarlo y cómo crear el disparador diario."*

Pega el código, autoriza, crea el *trigger* diario. Cambia una fecha para mañana y ejecuta manualmente: llega el correo.

```{admonition} Ruta pro 🧗
:class: tip
Conecta un **Google Form** público a la misma hoja: cualquier persona puede registrar un dato (inscripción, reporte, solicitud) sin tener la app, y tu bot responde. En la Sesión 15 este mismo flujo se convierte en un bot de Telegram con IA.
```

## 📦 Entregable

Enlace a tu app de AppSheet (compartida con el docente) + captura del correo automático recibido + enlace publicado en tu página web.

## 🏠 Reto para la casa (~3h)

1. Usa tu app durante la semana con datos reales (mínimo 20 registros).
2. Explora [datos.gov.co](https://www.datos.gov.co) y descarga **un dataset** de tu área (salud, justicia, cultura, deporte, ambiente). Tráelo en CSV.
3. Anota 3 **preguntas** que te gustaría responder con esos datos.
