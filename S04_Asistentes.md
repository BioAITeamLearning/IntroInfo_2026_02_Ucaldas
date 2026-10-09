---
title: Sesión 4 · Asistentes que trabajan
---
# Sesión 4 · Asistentes que trabajan con tus documentos 📊📄🖼️

En la sesión pasada montaste un asistente que **conversa**. Hoy montas tres que **producen**: uno que convierte una hoja de cálculo en un reporte con métricas, uno que responde documentos siguiendo una plantilla, y uno que escribe presentaciones con el estilo que ya usas.

## 🧰 Herramientas del día

| Herramienta | Para qué | Enlace |
|---|---|---|
| **Gems** (Gemini) | Los tres asistentes | [gemini.google.com/gems](https://gemini.google.com/gems) |
| **Google Sheets** | Donde termina el reporte y se hace la gráfica | [sheets.google.com](https://sheets.google.com) |
| **Google Docs** | Donde termina la respuesta redactada | [docs.google.com](https://docs.google.com) |
| **Google Slides** | Donde termina la presentación | [slides.google.com](https://slides.google.com) |
| **Hoja de prompts** | Todo lo de hoy, listo para copiar | <a href="_static/sesion04/prompts.html" target="_blank">Abrir</a> |

## 📂 Archivos de práctica

Descárgalos antes de empezar, o ábrelos desde la <a href="https://drive.google.com/drive/folders/1oI8JRGYerC4jTC-ZUiaRM6Ur5YfdRoWx" target="_blank">carpeta de Drive del curso</a> (ahí están en formato Google, listos para *Añadir desde Drive*). Son ficticios, hechos para la clase.

| Archivo | Para qué caso |
|---|---|
| <a href="_static/sesion04/archivos/registro-solicitudes.xlsx">📊 registro-solicitudes.xlsx</a> | Caso 1 · 62 filas de solicitudes atendidas, con errores a propósito |
| <a href="_static/sesion04/archivos/plantilla-respuesta.docx">📄 plantilla-respuesta.docx</a> | Caso 2 · la plantilla con sus cinco secciones y sus reglas de redacción |
| <a href="_static/sesion04/archivos/ejemplo-respuesta-diligenciada.docx">📄 ejemplo-respuesta-diligenciada.docx</a> | Caso 2 · una respuesta ya escrita, para que el asistente copie el tono |
| <a href="_static/sesion04/archivos/solicitudes-para-responder.docx">📄 solicitudes-para-responder.docx</a> | Caso 2 · tres solicitudes reales para contestar |
| <a href="_static/sesion04/archivos/presentacion-base.pptx">🖼️ presentacion-base.pptx</a> | Caso 3 · la presentación cuyo estilo vamos a reutilizar |

---

## 🧱 Lo mínimo: qué puede y qué no puede un Gem

| Puede | No puede |
|---|---|
| Leer los archivos que le subas y trabajar con ellos | **Modificar** tus archivos. No te devuelve el Excel corregido ni el PowerPoint rediseñado |
| Guardar documentos como **conocimiento permanente**: los tiene siempre a mano | Acordarse de un archivo que adjuntaste suelto en una conversación anterior |
| Calcular, comparar, clasificar y redactar sobre esos datos | Garantizar que la cuenta está bien: eso lo verificas tú |
| Devolverte el resultado listo para exportar a Docs, Sheets o Slides | Saber cosas que no estén ni en los documentos ni en su entrenamiento |

Dos lugares distintos para poner un archivo, y conviene no confundirlos:

* **Conocimiento del Gem**: lo que define cómo trabaja siempre. Ahí va la plantilla, la guía de estilo, el instructivo. Se carga una vez.
* **Adjunto en el chat**: el material de hoy. Ahí va el Excel de este mes, la solicitud de este estudiante.

### La pantalla de creación, campo por campo

Entra a [gemini.google.com/gems/create](https://gemini.google.com/gems/create). Vas a ver esto:

| Campo | Qué poner |
|---|---|
| **Nombre** | `Analista de reportes`. Sin nombre no te deja ni probarlo |
| **Descripción** | Una frase. Es lo que verás en tu lista de Gems dentro de un mes |
| **Instrucciones** | La ficha completa. Es el campo que importa |
| **Herramienta predeterminada** | Una herramienta que se activa sola en cada mensaje. Ver abajo |
| **Conocimientos** | *Subir archivos* o *Añadir desde Drive*. Los documentos permanentes |
| **Inhabilitar citas de conocimiento** | **Déjalo sin marcar.** Así el Gem señala de qué documento sacó cada cosa |

A la derecha tienes una **vista previa**: pruebas el Gem sin salir de la pantalla de edición.

### La herramienta predeterminada

Es una lista con seis opciones. Fijar una significa que el Gem la usa en **todos** los mensajes:

| Opción | Para qué te sirve |
|---|---|
| **No hay herramienta predeterminada** | Lo normal. El Gem conversa y tú activas lo que necesites desde el chat |
| **Canvas** | El Gem entrega un documento editable en vez de un mensaje. Útil cuando el resultado es un informe o una carta |
| **Deep Research** | Investiga por su cuenta antes de responder. Lo usaremos en la sesión de investigación |
| **Aprendizaje guiado** | En vez de darte la respuesta, te lleva paso a paso. Buenísimo para un Gem de estudio |
| **Crear imagen** · **Crear música** | Para Gems dedicados a producir ese tipo de material |

Para los tres casos de hoy, **déjala en "No hay herramienta predeterminada"**: los Gems necesitan conversar contigo antes de producir. Cuando quieras el entregable final como documento, activas Canvas desde el chat.

### El modelo también se elige

Dentro del chat del Gem hay un selector de modelo. Hoy en la cuenta institucional aparecen tres:

| Modelo | Lo que dice Google | Cuándo usarlo aquí |
|---|---|---|
| **Flash** | Ayuda completa | Revisión de calidad, redacción, armar láminas |
| **Thinking** | Resuelve problemas complejos | Cuando el cálculo tiene varios pasos encadenados |
| **Pro** | Razonamiento avanzado | Cuando el resultado te huele mal y quieres contrastarlo |

Es exactamente lo que vimos la sesión pasada: liviano, intermedio y grande. Ahora ya sabes dónde se cambia.

```{admonition} Si compartes un Gem
:class: warning
Al compartirlo se ven los **títulos** de sus archivos de conocimiento. El contenido se comparte aparte y te lo pregunta por separado. No le pongas como conocimiento nada que no quieras que otros sepan que existe.
```

---

## 📊 Caso 1 · De una hoja de cálculo a un reporte

**El encargo:** te pasan `registro-solicitudes.xlsx` y te piden "un informe de cómo vamos".

### Monta el Gem

Nombre: `Analista de reportes`. Sin herramienta predeterminada. Pega esto en **Instrucciones**:

```
QUIÉN ERES
Eres analista de datos de una oficina universitaria. Trabajas con registros
operativos y preparas reportes cortos para jefes que no leen tablas largas.

QUÉ HACES CUANDO TE PASO UNA HOJA DE CÁLCULO
1. Primero revisas la calidad de los datos y me dices qué encontraste:
   filas duplicadas, celdas vacías, fechas con formatos distintos, categorías
   que son la misma escrita diferente, valores imposibles.
2. Me preguntas qué hago con cada problema antes de calcular nada.
3. Cuando yo te responda, calculas las métricas y armas el reporte.

CÓMO ES EL REPORTE SIEMPRE
- Título que diga el hallazgo principal, no el tema.
- Tabla de métricas: nombre, valor, cómo se calculó.
- Tres hallazgos, cada uno en una frase, con el número que lo sustenta.
- Una alerta: lo que más conviene revisar.
- Limitaciones: qué no se puede concluir con estos datos.

REGLAS
Máximo 400 palabras. Español. Nada de adornos.
Todo número que escribas debe poder rastrearse a una columna de la hoja.
Si un cálculo depende de una decisión mía, no lo adivinas: me preguntas.
Al final, me dices qué gráfico recomiendas y por qué ese y no otro.
```

### Úsalo

| Paso | Qué haces |
|---|---|
| 1 | Adjunta `registro-solicitudes.xlsx` en el chat del Gem y escribe: `Revisa la calidad de estos datos antes de calcular nada.` |
| 2 | Lee lo que encontró. **Compáralo con la hoja**: abre el archivo y busca dos de los problemas que mencionó. ¿Existen de verdad? ¿Se le escapó alguno? |
| 3 | Respóndele qué hacer con cada problema y pídele el reporte |
| 4 | Pídele la gráfica que recomendó. Si tu cuenta no la genera, pídele los datos en tabla y haz el gráfico en Sheets (*Insertar → Gráfico*) |
| 5 | Exporta el reporte a Google Docs y el cuadro de métricas a Sheets |

```{admonition} Verificación obligatoria
:class: warning
Toma **dos** números del reporte y recalcúlalos tú en la hoja con una fórmula (`CONTAR.SI`, `PROMEDIO`, `CONTARA`). ¿Coinciden? Un reporte bonito con una cifra mal calculada es peor que no tener reporte.
```

Los datos traen problemas puestos a propósito: hay filas duplicadas, una dependencia vacía, fechas en tres formatos distintos, un valor de días negativo y una calificación fuera de la escala de 1 a 5. Si tu asistente no los menciona, el que está fallando es el prompt, no los datos.

---

## 📄 Caso 2 · De una plantilla a respuestas

**El encargo:** la oficina tiene una plantilla y un tono propio. Hay que responder tres solicitudes sin que se note que cambió quién escribe.

### Monta el Gem

Nombre: `Redactor de respuestas`. En **Conocimientos** súbele `plantilla-respuesta.docx` y `ejemplo-respuesta-diligenciada.docx` (*Subir archivos* o *Añadir desde Drive*). En **Instrucciones**:

```
QUIÉN ERES
Eres el redactor de la Oficina de Atención al Estudiante. Respondes
solicitudes siguiendo exactamente la plantilla institucional que tienes
en tus documentos.

CÓMO TRABAJAS
Antes de redactar, me haces las preguntas que te falten para llenar la
plantilla: fecha, radicado, nombre, programa y la decisión que se tomó.
No inventas ninguno de esos datos. Nunca.

Si no sé qué decidir, me ayudas a pensarlo: me dices qué información
haría falta y qué opciones hay. Pero la decisión la tomo yo.

LA PLANTILLA
Respetas las cinco secciones, en el mismo orden y con los mismos títulos.
Respetas las reglas de redacción que están al final de la plantilla.
Imitas el tono del ejemplo diligenciado, no el de un chat.

QUÉ NUNCA HACES
No citas normas que no te haya dado yo. Si hace falta una, escribes
[VERIFICAR NORMA] y sigues.
No prometes plazos que no aparezcan en la solicitud o que yo no te dé.
No usas "se le informa que", ni siglas sin explicar.
```

### Úsalo

| Paso | Qué haces |
|---|---|
| 1 | Abre `solicitudes-para-responder.docx`, escoge una y pégale el texto al Gem |
| 2 | Contesta las preguntas que te haga. **Fíjate si te las hizo**: si redactó de una, le falta la instrucción |
| 3 | Revisa la respuesta contra la plantilla: ¿están las cinco secciones? ¿cumple las reglas de redacción? ¿alguna frase pasa de 25 palabras? |
| 4 | Busca los `[VERIFICAR NORMA]`. Esos son los puntos donde tú tienes que trabajar |
| 5 | Exporta a Google Docs y dale el formato final |

Prueba el límite: pídele que responda la **solicitud 3** (la devolución del dinero) sin darle ninguna información sobre la política de reembolsos. Debería decirte que le falta ese dato, no inventarse una política.

---

## 🖼️ Caso 3 · De una presentación base a tu estilo

**El encargo:** existe una presentación institucional y todas las demás deben parecerse a ella.

Aquí hay que ser claro con lo que pasa: **el Gem no rediseña tu PowerPoint**. Lo que hace es sacar las reglas de estilo de la presentación base y escribir el contenido nuevo respetándolas, lámina por lámina. El diseño lo aplicas tú una sola vez, con un tema guardado en Slides.

### Primero, extrae el estilo

Sube `presentacion-base.pptx` a Gemini y pídele:

```
Analiza esta presentación y escríbeme su guía de estilo: colores que usa
y para qué, tipografía, cuántas palabras tiene en promedio cada lámina,
qué tipos de lámina existen (portada, agenda, separador, contenido, cifras,
cierre) y qué reglas de composición se repiten. Devuélvemelo como una lista
de reglas que yo pueda darle a otra persona para que haga una presentación
igual sin ver esta.
```

Esa lista es el documento de conocimiento del siguiente Gem.

### Monta el Gem

Nombre: `Diseñador de presentaciones`. En **Conocimientos**, la guía de estilo que acabas de generar (pégala en un Doc y súbela). En **Instrucciones**:

```
QUIÉN ERES
Preparas presentaciones que siguen la guía de estilo que tienes en tus
documentos. No improvisas un estilo nuevo.

CÓMO ENTREGAS
Una lámina por bloque, así:

LÁMINA 3 · contenido
Título: [el hallazgo, no el tema]
Cuerpo: [máximo 4 viñetas de máximo 12 palabras]
Notas del orador: [lo que se dice en voz alta, 2 o 3 frases]

REGLAS
Respetas el número de láminas que te pida.
Respetas los tipos de lámina de la guía y los usas en el mismo orden lógico.
El título de cada lámina dice el hallazgo, no el tema.
Lo que no cabe en la lámina va a las notas del orador.
Si me ves metiendo mucho texto en una lámina, me lo adviertes y la partes.
```

### Úsalo

| Paso | Qué haces |
|---|---|
| 1 | Pídele: `Con el reporte del Caso 1, arma una presentación de 6 láminas para el jefe de la oficina.` |
| 2 | Abre Slides, crea una presentación, y aplica el tema una vez: colores y tipografía de la guía (*Diapositiva → Cambiar tema*, o edita el patrón) |
| 3 | Pega el contenido lámina por lámina, incluidas las notas del orador |
| 4 | Compara con `presentacion-base.pptx` abierta al lado. ¿Se parecen? |

```{admonition} Atajo
:class: tip
Si en Slides creas **una** presentación con tu estilo y la guardas como plantilla, no vuelves a hacer este paso nunca: abres una copia y pegas el contenido que te dé el Gem.
```

---

## 🔄 Cierre · ¿cuál de los tres te sirve ya?

Escoge **uno** de los tres asistentes y adáptalo a algo que de verdad tengas que hacer este semestre: la base de datos de tu práctica, el formato de informes de tu materia, las presentaciones de tu grupo.

| Área | Qué podrías montar hoy mismo |
|---|---|
| Biología · Ing. de alimentos | Analista de resultados de laboratorio: le pasas la tabla de mediciones y te devuelve el reporte con las alertas |
| Derecho | Redactor de derechos de petición y tutelas, con tus formatos como conocimiento |
| Estudios de familia | Sistematizador de entrevistas: le pasas las notas y te devuelve la matriz de categorías |
| Diseño visual · Artes | Guía de estilo viva: le subes tu portafolio y te mantiene coherente todo lo nuevo |
| Deporte | Analista de cargas: le pasas la planilla semanal y te devuelve las alertas por atleta |

## 📽️ Material

* <a href="_static/sesion04/prompts.html" target="_blank">📋 Todos los prompts y las tres fichas, listos para copiar</a>
* <a href="_static/sesion04/slides.html" target="_blank">Diapositivas de la sesión</a>
* <a href="_static/sesion04/guia.html" target="_blank">Guía de los tres casos</a>

## 📦 Lo que te llevas

Tres asistentes montados y probados con archivos reales, y uno de ellos adaptado a algo tuyo. En el tablero del curso: cuál adaptaste, para qué, y los dos números que recalculaste a mano en el Caso 1.
