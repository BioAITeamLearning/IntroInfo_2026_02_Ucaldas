---
title: Sesión 11 · Analizar con IA
---
# Sesión 11 · Analizar datos con IA en lenguaje natural 🔬📈

> *"No necesitas saber programar para analizar datos. Necesitas saber preguntar y saber leer la respuesta."*

## 🧰 Herramientas del día

| Herramienta | Para qué la usamos hoy | Enlace | Costo |
|---|---|---|---|
| **Google Colab + Gemini** (Data Science Agent) | Describes el análisis, la IA escribe y ejecuta el código Python | [colab.research.google.com](https://colab.research.google.com) | Gratis |
| **Seeing Theory** | Simuladores visuales de estadística | [seeing-theory.brown.edu](https://seeing-theory.brown.edu) | Gratis |
| **PhET** / **Spurious Correlations** | Simulaciones y el juego de correlación ≠ causalidad | [phet.colorado.edu](https://phet.colorado.edu) · [tylervigen.com/spurious-correlations](https://tylervigen.com/spurious-correlations) | Gratis |
| **Claude / ChatGPT (análisis de archivos)** | Subir un CSV y conversar con él | [claude.ai](https://claude.ai) · [chatgpt.com](https://chatgpt.com) | Gratis |
| **Gemini CLI** | Analizar una carpeta entera de CSV desde la terminal | [github.com/google-gemini/gemini-cli](https://github.com/google-gemini/gemini-cli) | Gratis |

## 🎯 Objetivos

* Entender **intuitivamente** promedio, mediana, dispersión, distribución, correlación y por qué correlación no es causalidad.
* Hacer un análisis completo en **Colab** con el agente de ciencia de datos: cargar, describir, agrupar, comparar, graficar.
* Leer críticamente lo que la IA concluye: ¿el código hizo lo que dijo? ¿la muestra permite esa conclusión?
* Ruta pro: analizar una **carpeta** de datos con un agente en la terminal.

```{admonition} Cobertura PIIA
:class: note
Unidad 4 · b. Utilidades de análisis e interpretación de datos · c. Obtención y representación de resultados.
```

## ⏱️ Agenda (2h30)

| Tiempo | Bloque | Qué pasa |
|---|---|---|
| 0:00 – 0:25 | 🎲 **Estadística jugando** | Seeing Theory en vivo: promedio vs mediana (¿cuánto gana "en promedio" un salón donde entra un futbolista?), distribución, muestreo. Spurious Correlations: reírse y entender |
| 0:25 – 0:45 | 🤖 **Colab en 20 min** | Qué es un notebook, qué es Python (solo lo necesario), cómo pedirle al agente de Gemini. Demo con un dataset del grupo |
| 0:45 – 1:15 | 🔬 **Actividad 1: Tus 3 preguntas, parte 1** | Cargar, describir, primera pregunta |
| 1:15 – 1:25 | ☕ Pausa | |
| 1:25 – 2:00 | 🔬 **Actividad 1: parte 2** | Preguntas 2 y 3, con gráficos. Verificación cruzada en Claude |
| 2:00 – 2:20 | 🧗 **Ruta pro: la carpeta** | Gemini CLI sobre `datos/` (demo + quien quiera lo hace) |
| 2:20 – 2:30 | 🏁 Cierre | Cada uno escribe en dos líneas **quién** debería ver estos resultados y qué **decisión** tomaría. Exporta los 3 gráficos como PNG |

## 🔬 Actividad 1: Tus 3 preguntas (65 min)

Abre [Colab](https://colab.research.google.com), sube tu CSV limpio y usa el panel de Gemini (o escribe en una celda de texto y pide *Generar*). Guion sugerido de prompts:

| # | Prompt | Qué esperas ver |
|---|---|---|
| 1 | *"Carga `limpio.csv` con pandas y muestra: número de filas, tipos de columnas, valores nulos, y 5 filas."* | Que entendió tu dataset |
| 2 | *"Para las columnas numéricas calcula promedio, mediana, mínimo, máximo y desviación. Explica en español qué significa cada uno para este dataset."* | Que los números tienen sentido con tu contexto |
| 3 | *"Pregunta 1: [tu pregunta]. Responde con una tabla agrupada y un gráfico de barras con título y ejes en español."* | Un resultado + un gráfico |
| 4 | *"Pregunta 2: [tu pregunta]. Si implica comparar grupos, muestra un boxplot y di si la diferencia parece grande respecto a la dispersión."* | Comparación honesta |
| 5 | *"Pregunta 3: [tu pregunta]. Si implica dos variables numéricas, muestra un diagrama de dispersión y la correlación, y advierte explícitamente sobre causalidad."* | Correlación con cautela |
| 6 | *"Resume los tres hallazgos en 5 líneas para alguien que no ve los datos. Indica qué limitaciones tiene este análisis."* | Tu párrafo de conclusiones |

**Verificación cruzada (10 min):** sube el mismo CSV a Claude o ChatGPT y haz la pregunta 1. ¿Coinciden los números? Si no, ¿quién tiene razón? (Pista: mira el código.)

```{tip}
Lee siempre el código que genera el agente aunque no sepas Python: busca los nombres de tus columnas y los números que aparecen. Si el agente "filtró" algo que no pediste, lo verás ahí.
```

## 🧗 Ruta pro: analizar una carpeta con un agente (20 min)

En tu computador, en la carpeta `datos/` con varios CSV:

```bash
cd datos
gemini
```

Y dentro del agente:

> *"Revisa todos los CSV de esta carpeta. Para cada uno dime: número de filas, columnas, si tiene vacíos y de qué parece tratar. Luego dime cuáles se podrían unir por una columna en común y propón un análisis conjunto. No modifiques ningún archivo."*

Después: *"Escribe un script `resumen.py` que genere un archivo `resumen.md` con esa información y ejecútalo."* Abre `resumen.md`. **Acabas de correr un agente sobre tu disco.** La Sesión 14 es toda sobre esto.

## 📦 Lo que te llevas

Notebook de Colab (compartido) con las 3 preguntas, gráficos y el párrafo de conclusiones y limitaciones. Enlace en tu página.
