---
title: Sesión 12 · Dashboards y data storytelling
---
# Sesión 12 · Dashboards y contar historias con datos 📊🗣️

> *"Un gráfico que nadie entiende es un dato que nadie usa."*

## 🧰 Herramientas del día

| Herramienta | Para qué la usamos hoy | Enlace | Costo |
|---|---|---|---|
| **Looker Studio** | Dashboard conectado a tu hoja de Google, se actualiza solo | [lookerstudio.google.com](https://lookerstudio.google.com) | Gratis |
| **Flourish** / **Datawrapper** | Gráficos animados e interactivos listos para publicar | [flourish.studio](https://flourish.studio) · [datawrapper.de](https://www.datawrapper.de) | Gratis |
| **Claude Artifacts** / **Gemini Canvas** | Dashboard interactivo hecho a medida desde un prompt | [claude.ai](https://claude.ai) | Gratis |
| **RAWGraphs** | Visualizaciones no convencionales (para artes y ciencias) | [rawgraphs.io](https://www.rawgraphs.io) | Gratis |
| **Gemini** | Elegir el gráfico correcto y redactar la historia | [gemini.google.com](https://gemini.google.com) | Gratis |

## 🎯 Objetivos

* Elegir el **gráfico correcto** para cada pregunta (comparar, evolucionar, distribuir, relacionar, componer).
* Reconocer y evitar **gráficos engañosos** (ejes truncados, 3D, colores manipuladores).
* Publicar un **dashboard** conectado a datos vivos.
* Contar una **historia con datos**: contexto → hallazgo → implicación → decisión.

```{admonition} Cobertura PIIA
:class: note
Unidad 4 · c. Representación de resultados · d. Herramientas para visualización de datos · Unidad 5 · c.a. Redacción de documentos.
```

## ⏱️ Agenda (2h30)

| Tiempo | Bloque | Qué pasa |
|---|---|---|
| 0:00 – 0:20 | 🎯 **El gráfico correcto (y el incorrecto)** | Juego: 8 gráficos, ¿cuál miente? Luego la tabla "pregunta → gráfico" |
| 0:20 – 0:55 | 📊 **Actividad 1: Dashboard en Looker Studio** | Conectar tu hoja `limpio`, 4 tarjetas de indicadores + 3 gráficos + 1 filtro |
| 0:55 – 1:15 | ✨ **Actividad 2: Un gráfico que se mueva** | Flourish: carrera de barras o mapa con tus datos |
| 1:15 – 1:25 | ☕ Pausa | |
| 1:25 – 1:50 | 🤖 **Actividad 3: Dashboard a medida con IA** | Claude Artifacts con tu CSV |
| 1:50 – 2:15 | 🗣️ **Actividad 4: Tu historia de datos** | Estructura + ensayo en parejas |
| 2:15 – 2:30 | 🎤 **Sustentación del Ejercicio 2** | Historias de datos de 2 minutos frente al grupo (el resto sustenta en parejas con el docente durante las actividades) |

## 🎯 Pregunta → gráfico

| Quiero… | Gráfico | Evita |
|---|---|---|
| Comparar categorías | Barras (horizontales si son muchas) | Torta con más de 4 partes |
| Ver evolución en el tiempo | Líneas | Barras 3D |
| Ver cómo se distribuye | Histograma, boxplot | Promedios sin dispersión |
| Relacionar dos variables | Dispersión | Líneas que sugieren causa |
| Mostrar partes de un todo | Barras apiladas 100 % (o torta ≤ 4 partes) | Donas múltiples |
| Ubicar geográficamente | Mapa coroplético / de puntos | Mapas sin normalizar por población |

Reglas de honestidad: eje Y desde cero en barras · misma escala al comparar · fuente y fecha visibles · título que diga el hallazgo, no la variable ("Las lesiones suben en pretemporada", no "Lesiones por mes").

## 📊 Actividad 1: Looker Studio (35 min)

1. *Crear → Informe → Hojas de cálculo de Google* → tu pestaña `limpio`.
2. Agrega **4 tarjetas de indicador** (total de registros, promedio clave, máximo, % de una categoría).
3. Agrega 3 gráficos siguiendo la tabla anterior, con títulos que digan el hallazgo.
4. Agrega un **control de filtro** (por fecha o categoría).
5. *Compartir → cualquiera con el enlace puede ver*. Pega el enlace en tu página. Cambia un dato en la hoja: el dashboard se actualiza solo.

## ✨ Actividad 2: Flourish (20 min)

Elige una plantilla (*bar chart race*, *scatter*, *map*) → sube tu CSV → publica → inserta el `<iframe>` en tu página (Google Sites: *Insertar → Incorporar*).

## 🤖 Actividad 3: Dashboard a medida con IA (25 min)

En Claude, adjunta tu CSV y pide:

> *"Crea un dashboard interactivo en un solo archivo HTML con estos datos: 4 indicadores arriba, un gráfico de barras y uno de líneas, un filtro por [columna], colores sobrios, en español, que se vea bien en celular. Los datos van embebidos en el archivo."*

Itera dos veces. Descarga el HTML y súbelo a tu página (Netlify Drop / GitHub Pages). Compara con Looker: ¿cuál usarías para qué?

## 🗣️ Actividad 4: Tu historia de datos (25 min)

Estructura de 2 minutos:

1. **Contexto** (20 s): quién, qué datos, de dónde.
2. **Hallazgo** (40 s): un gráfico, una frase-titular.
3. **Así que…** (40 s): qué implica, con una limitación honesta.
4. **Decisión** (20 s): qué debería hacer la audiencia mañana.

Pide a Gemini: *"Aquí están mis 3 hallazgos y mi audiencia es [X]. Escribe un guion de 2 minutos con esta estructura y luego critícalo: ¿qué objeción haría alguien escéptico?"* Ensaya con tu pareja cronometrando.

## 🎤 Ejercicio 2 · Mi sistema publicado (35% · se sustenta hoy)

Tu **página web** (S7) con, como mínimo:

1. Tu **sistema de gestión** en AppSheet con datos reales y su automatización funcionando (S9).
2. Tu **dashboard** (Looker Studio o HTML) conectado al dataset que limpiaste y analizaste (S10–S12).
3. Tu **declaración de uso de IA** para cada pieza.

**Sustentación:** tu historia de datos de 2 minutos frente al grupo o en pareja con el docente, y una pregunta en vivo del tipo *"agrega un registro en tu app y muéstrame que el dashboard cambia"*. Rúbrica en {doc}`Metodologia`.

```{note}
Cierre del **Corte 2**. Los talleres de S7–S11 (multimedia, dataset, notebook) no tienen nota aparte: son las piezas de este ejercicio y viven en tu página.
```

## 🏠 Reto para la casa (~3h)

1. Entrena 5 minutos con [Quick, Draw!](https://quickdraw.withgoogle.com) y mira qué dibujaron **otras personas** en el mismo concepto ("mira los datos"). ¿De dónde aprende la IA?
2. Ve el video [But what is a neural network?](https://www.youtube.com/watch?v=aircAruvnKk) (3Blue1Brown, con subtítulos).
3. Trae 30 fotos (o prepárate para tomarlas con la cámara) de **dos cosas que quieras que una IA distinga**: dos especies, dos posturas deportivas, dos estilos de obra, dos tipos de documento.
