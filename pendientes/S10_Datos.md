---
title: Sesión 10 · Obtener y limpiar datos
---
# Sesión 10 · Obtener y limpiar datos con IA 🧹📥

> *"El 80 % del trabajo con datos es limpiarlos. La IA hace el 80 % de ese 80 %."*

## 🧰 Herramientas del día

| Herramienta | Para qué la usamos hoy | Enlace | Costo |
|---|---|---|---|
| **datos.gov.co** | Datos abiertos de Colombia (salud, justicia, deporte, cultura, ambiente) | [datos.gov.co](https://www.datos.gov.co) | Gratis |
| **Our World in Data** / **Kaggle** | Datasets del mundo, listos para usar | [ourworldindata.org](https://ourworldindata.org) · [kaggle.com/datasets](https://www.kaggle.com/datasets) | Gratis |
| **Google Sheets + Gemini** | Limpiar, clasificar y extraer con IA (`=AI()`) | [sheets.google.com](https://sheets.google.com) | Gratis |
| **Gemini (multimodal)** | Sacar tablas de PDFs, fotos de formularios, capturas | [gemini.google.com](https://gemini.google.com) | Gratis |
| **Google Forms** | Recolectar datos propios (encuestas) | [forms.google.com](https://forms.google.com) | Gratis |
| **Gapminder Tools** | Juego: ¿qué tan bien conoces el mundo con datos? | [gapminder.org/tools](https://www.gapminder.org/tools/) | Gratis |

## 🎯 Objetivos

* Conocer las **fuentes** de datos: abiertos, propios (encuestas, tu app de la S9), extraídos de documentos.
* Distinguir tipos de datos (categórico, numérico, fecha, texto) y por qué importa.
* Aplicar los pasos de limpieza: duplicados, vacíos, formatos, categorías inconsistentes, anonimización.
* Documentar el dataset: de dónde salió, qué significa cada columna, qué le hiciste.

## 📸 Actividad 1: Del papel/PDF a la tabla

1. Toma una foto de una tabla en papel (una planilla de asistencia, resultados de laboratorio, una lista de precios, un acta) o abre un PDF con tablas de tu área.
2. En Gemini: *"Extrae la tabla de esta imagen en formato CSV. Marca con `?` las celdas que no leas con seguridad."*
3. Pega en Sheets (*Datos → Dividir texto en columnas*). Cuenta los `?`: ese es el margen de error que debes revisar a mano.
4. Repite con una tabla de 3 páginas de un PDF: pide *"une las tablas de las páginas en una sola"*.

## 🧹 Actividad 2: Limpieza con IA

Con el dataset de datos.gov.co que descargaste, en Google Sheets:

| Paso | Qué hacer | Prompt a Gemini en Sheets / función |
|---|---|---|
| 1. Entender | ¿Qué es cada columna? | *"Explica qué significa cada columna de esta hoja y qué tipo de dato es"* |
| 2. Duplicados | Filas repetidas | *Datos → Limpieza de datos → Quitar duplicados* |
| 3. Vacíos | ¿Cuántos y dónde? | *"¿Qué columnas tienen celdas vacías y cuántas? ¿Sugieres eliminar la fila, rellenar o dejar?"* |
| 4. Formatos | Fechas, números con texto, mayúsculas | *"Convierte la columna fecha a AAAA-MM-DD y la columna valor a número"* |
| 5. Categorías | "Manizales", "MANIZALES", "manizales " | *"Unifica las variantes de la columna municipio"* · `=TRIM(PROPER(A2))` |
| 6. Clasificar | Crear una columna nueva con IA | `=AI("Clasifica esta descripción en: leve, moderado, grave", D2)` |
| 7. Anonimizar | Nombres, cédulas, correos | Eliminar o reemplazar por un código: `="P"&ROW()` |
| 8. Documentar | Diccionario de datos | Hoja nueva: columna · significado · tipo · unidad · fuente · transformación |

```{admonition} Ruta pro 🧗
:class: tip
Sube el CSV a **Google Colab** y escribe en una celda: *"Carga este CSV con pandas, muestra los tipos de columna, los valores nulos por columna y 5 filas de ejemplo."* Deja que Gemini en Colab genere y ejecute el código. La próxima sesión hacemos todo el análisis así.
```

## 🔒 Anonimizar y documentar

| Dato | Riesgo | Qué hacer |
|---|---|---|
| Nombre, cédula, correo, teléfono | Identifica directamente | Eliminar o reemplazar por código |
| Fecha de nacimiento exacta | Reidentificación | Convertir a edad o rango de edad |
| Dirección | Reidentificación | Dejar solo barrio/comuna o municipio |
| Diagnóstico, antecedentes penales, orientación | Dato sensible (Ley 1581) | Solo con consentimiento y anonimizado |

## 📦 Lo que te llevas

Hoja de Google con: pestaña `original`, pestaña `limpio`, pestaña `diccionario` + tus 3 preguntas de investigación al final. Descarga `limpio` como CSV a una carpeta `datos/` en tu computador (lo usas la próxima sesión). Enlace en tu página.
