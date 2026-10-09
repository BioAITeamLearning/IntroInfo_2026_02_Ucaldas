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
| **Fichas de Gems** | Once asistentes listos para montar, uno por programa | <a href="_static/sesion05/gems.html" target="_blank">Abrir</a> |

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
| Leer los archivos que le subas y trabajar con ellos | **Escribir dentro** de tus archivos de Drive. No te añade la fila al Excel ni rediseña el PowerPoint |
| Con **Canvas**, devolverte un documento editable que vas puliendo en la conversación y exportas a Docs | Recordar lo que hiciste en otra conversación |
| Guardar documentos como **conocimiento permanente**: los tiene siempre a mano | Acordarse de un archivo que adjuntaste suelto en una conversación anterior |
| Calcular, comparar, clasificar y redactar sobre esos datos | Garantizar que la cuenta está bien: eso lo verificas tú |
| Devolverte el resultado listo para exportar a Docs, Sheets o Slides | Saber cosas que no estén ni en los documentos ni en su entrenamiento |

Dos lugares distintos para poner un archivo, y conviene no confundirlos:

* **Conocimiento del Gem**: lo que define cómo trabaja siempre. Ahí va la plantilla, la guía de estilo, el instructivo. Se carga una vez. Si lo vinculas **desde Drive**, el Gem lee siempre la versión más reciente: tú editas el archivo y él lo ve al instante.
* **Adjunto en el chat**: el material de hoy. Ahí va el Excel de este mes, la solicitud de este estudiante.

```{admonition} ¿Y si quiero que la bitácora se escriba sola?
:class: note
El Gem no escribe dentro de tu hoja. Las rutas que sí funcionan, de menos a más trabajo: que el Gem te **devuelva la fila lista** y tú la pegues · un **Google Form** que añade la fila solo · **Gemini en Sheets** desde el panel lateral de la hoja abierta · un **Apps Script** con `appendRow`, que el propio Gemini te escribe · o una app de **AppSheet**. Las tres últimas son la sesión de sistemas de gestión.

Lo que sí cambia el juego hoy es **Canvas**: el Gem mantiene el documento abierto y le va agregando, y tú lo exportas a Docs cuando quieras. Es lo más cerca que vas a estar de "ir dictándole y que se vaya escribiendo".
```

### Varios archivos a la vez

Puedes adjuntar **más de un archivo en el mismo mensaje**: la hoja de cálculo, la plantilla y las solicitudes juntas. Quedan disponibles durante toda la conversación y el asistente puede cruzarlas.

Dos cosas que aprendimos probándolo:

* **Una petición por mensaje.** Si le pides tres cosas numeradas de una vez, es muy probable que responda *"solo soy un modelo de lenguaje"* y no haga nada. Separado en tres mensajes, funciona sin problema.
* **Verás un enlace "Mostrar código"** encima de la respuesta. Ahí está el programa que escribió para leer tu archivo y hacer las cuentas. Ábrelo: es la forma de comprobar qué filas usó y cuáles excluyó.

### Elige Flash, no Thinking

```{admonition} Esto importa hoy
:class: warning
Probado el 9 de octubre en la cuenta institucional: con el modelo **Thinking** seleccionado, Gemini respondió *"No puedo ayudarte porque solo soy un modelo de lenguaje"* a cualquier pregunta sobre los archivos adjuntos. Con **Flash**, la misma pregunta y los mismos archivos funcionaron perfecto: auditoría completa, métricas y gráfica.

Si tu asistente se niega a trabajar con un archivo, **lo primero que debes mirar es el selector de modelo**.
```

Con Flash, y con los mismos tres archivos adjuntos, el resultado fue este:

* Encontró los **dos duplicados exactos** (SOL-008 y SOL-041), indicando en qué filas están.
* Encontró la dependencia vacía (SOL-023), los **tres formatos de fecha** con ejemplos, las variantes *Bienestar / BIENESTAR / "Bienestar "* y hasta la inconsistencia en el nombre del responsable.
* Encontró los valores imposibles: días en −3 y satisfacción de 9 sobre 5.
* Encontró dos incoherencias que **no estaban en la lista**: una solicitud cerrada sin días de respuesta y una "en trámite" que sin embargo tiene calificación.
* Cuando se le pidió limpiar y graficar, **generó una gráfica de barras de verdad** con la demora promedio por dependencia: Biblioteca 11,71 días · Registro Académico 11,00 · Bienestar 9,29.

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

## 🧠 Cómo se plantea un asistente antes de montarlo

Montar un Gem toma diez minutos. Pensarlo bien es lo que decide si lo vas a seguir usando en dos semanas o si lo vas a abandonar. Antes de abrir Gemini, piénsalo **como si fueras a contratar a alguien**.

### Un asistente es como un empleado nuevo

Es capaz, pero no sabe nada de tu trabajo hasta que se lo das:

| Pieza | En un empleado nuevo | En el Gem |
|---|---|---|
| **El modelo** | La persona que llega | Gemini |
| **Instrucciones** | Su inducción y su descripción de cargo | El campo Instrucciones |
| **Conocimiento** | Los manuales y formatos de la oficina | El campo Conocimientos |
| **Herramientas** | Su computador, su teléfono | Canvas, imagen, música, Deep Research |
| **Memoria** | Su libreta de notas | La conversación actual |
| **Disparador** | El horario o el aviso que lo pone a trabajar | Que tú le escribas |
| **Control** | La firma del jefe | Tú, antes de usar lo que produjo |

Casi siempre que un asistente "no sirve", lo que falta no es el modelo: es la inducción o los manuales.

### ¿Esto necesita un asistente, o algo más simple?

| | Qué es | Ejemplo |
|---|---|---|
| **Una pregunta suelta** | Le pides una cosa puntual y listo | "Reescribe este correo en tono formal" |
| **Un flujo** | Pasos fijos, siempre los mismos | Formulario → fila en la hoja → aviso por correo |
| **Un asistente** | Recibe un objetivo y decide los pasos | "Toma esta consulta, busca lo que aplica, redacta y dime si hay que derivarla" |

La diferencia no es la tecnología: es **quién decide el camino**. Si los pasos son siempre iguales, no necesitas un asistente, necesitas un flujo — y eso lo vemos en la sesión de sistemas de gestión.

### Los cinco pasos para diseñarlo

**Paso 0 · Elige el proceso.** Lista cinco cosas repetitivas que haces y escoge una. Buen candidato: pasa seguido, te cuesta tiempo, si sale mal no es grave, y no exige juicio profesional insustituible.

| Qué preguntarte | Buen candidato | Mal candidato |
|---|---|---|
| ¿Cada cuánto lo hago? | Varias veces por semana | Una vez al año |
| ¿Cuánto me cuesta? | Media hora o más | Dos minutos |
| ¿Qué pasa si sale mal? | Lo corrijo y ya | Afecta a una persona o a un derecho |
| ¿Exige mi criterio profesional? | Poco: es ordenar y redactar | Todo: es decidir |

**Paso 1 · El problema que resuelve.** ¿Qué te quita más de media hora cada semana? ¿Qué se te olvida y luego te arrepientes? ¿Qué información revisas en tres lugares distintos?

**Paso 2 · Rol y tono.** Elige qué clase de asistente necesitas:

| Rol | Cómo se comporta |
|---|---|
| **Asistente cuidadoso** | Formal, atento al detalle, revisa dos veces antes de entregar |
| **Jefe de gabinete** | Directo, prioriza por ti, te quita de encima lo que no importa |
| **Coach honesto** | Te confronta, no te endulza nada |
| **Compañero de trabajo** | Informal, te habla de tú, comparte el contexto |
| **Curador silencioso** | Solo aparece cuando hay algo que de verdad importa |

Ojo: hay **dos tonos** en juego. Cómo te habla a ti, y cómo escribe lo que va a leer otra persona. No tienen por qué ser el mismo.

**Paso 3 · La tarea principal.** Completa esta frase y no sigas hasta que quede concreta:

> *"Mi asistente va a **[verbo]** **[objeto específico]** **[cuándo o con qué disparador]** para que yo pueda **[resultado para mí]**."*

**La prueba de claridad:** ¿alguien que no te conoce entendería exactamente qué hace y para quién? Si no, está demasiado abstracto. "Me ayuda con los correos" no pasa la prueba.

**Paso 4 · La métrica.** Dos frases:

> *"Está funcionando si en una semana típica ______ pasa al menos ______ veces."*
> *"Claramente NO está funcionando si ______."*

La segunda es la línea roja. Casi siempre es *"si inventa un dato"* o *"si promete algo que no puedo cumplir"*.

**Paso 5 · La caja de herramientas.** Lista todo lo que te gustaría que hiciera y después **recorta a lo mínimo que ya te ahorra tiempo**. Por cada capacidad pregúntate: ¿si solo tuviera esta, ya me sirve? Lo que no pase el filtro, fuera de la primera versión.

### ¿Cuánta autonomía le das?

| Nivel | Qué hace | Cuándo |
|---|---|---|
| **1 · Sugiere** | Te propone, tú decides y haces | Lo normal al empezar |
| **2 · Prepara** | Deja el borrador listo, tú apruebas | Donde vive casi todo lo útil |
| **3 · Actúa e informa** | Lo hace y te avisa | Cosas sin consecuencias |
| **4 · Actúa solo** | Sin revisión | Casi nunca, y nunca con personas de por medio |

Regla para este curso: **todo lo que afecte a otra persona se queda en nivel 1 o 2**. Un informe a un cliente, una respuesta a una familia, una ficha de un paciente, un concepto jurídico: borrador y revisión. Siempre.

### El semáforo de los datos

| | Qué es | Dónde puede ir |
|---|---|---|
| 🟢 **Verde** | Datos públicos o inventados para practicar | Cualquier herramienta |
| 🟡 **Amarillo** | Información interna sin personas: procedimientos, plantillas, totales | Tu cuenta institucional |
| 🔴 **Rojo** | Datos personales o sensibles: nombres, cédulas, historias clínicas, expedientes, datos de menores | **No entran.** Se anonimizan antes |

En Colombia esto no es una recomendación: la Ley 1581 de 2012 regula el tratamiento de datos personales, y los datos sensibles tienen protección reforzada. Si vas a trabajar con información de personas reales —pacientes, clientes, familias, atletas, estudiantes— **se anonimiza primero**.


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

```{admonition} Probado el 9 de octubre
:class: note
Con la plantilla y las solicitudes adjuntas, devolvió la carta con **las cinco secciones y sus títulos exactos**, frases cortas, `[VERIFICAR]` en la fecha y en la firma, y en el punto 2 escribió *"No existe un procedimiento ni norma específica citada"* en vez de inventarse una norma.

Dos cosas que sí hay que vigilar: **decidió por su cuenta** conceder la solicitud (nadie se lo dijo), y escribió "adjuntamos el documento" cuando nadie mencionó un adjunto. Por eso la ficha del Gem lleva la línea *"la decisión la tomo yo"*: sin ella, decide él.
```

---

## 🖼️ Caso 3 · De una presentación base a tu estilo

**El encargo:** existe una presentación institucional y todas las demás deben parecerse a ella.

```{admonition} Lo que probamos y no funcionó
:class: warning
Le subimos la presentación a Gemini con la cuenta institucional y le pedimos la guía de estilo. Respondió: *"Lo que me pides está fuera de mis capacidades programadas. Solo genero texto."* Lo mismo al subirle una **imagen** de la lámina.

En cambio, **sí lee el texto** del archivo: le preguntamos cuántas láminas tiene y qué dice cada título, y respondió bien (aunque se saltó una lámina: hay que verificar).

Conclusión: en esta cuenta, **la IA no te va a describir colores ni tipografías**. El diseño lo miras tú. Ella se encarga del contenido.
```

Así que el trabajo se reparte: **tú escribes las reglas visuales mirando la presentación**, y **Gemini extrae las reglas de estructura** desde el texto del archivo. Las dos juntas son la guía de estilo.

### Paso 1 · Las reglas visuales las escribes tú

Abre `presentacion-base.pptx` y llena esto mirando (está también en la guía impresa):

| Elemento | Lo que ves |
|---|---|
| Color de fondo de la portada y los separadores | |
| Color de fondo de las láminas de contenido | |
| Color de los acentos: cifras, barras, detalles | |
| Tipografía | |
| ¿Qué elemento gráfico se repite en todas las láminas? | |

Mirar y nombrar lo que ves es la mitad del oficio de quien diseña. Hoy te toca a ti.

### Paso 2 · Las reglas de estructura las saca Gemini

Sube la presentación y pídele:

```
Lee el texto de esta presentación y dime: cuántas láminas tiene, qué dice
el título de cada una, qué tipos de lámina identificas (portada, agenda,
separador, contenido, cifras, cierre) y cuántas palabras tiene en promedio
cada una. Solo el texto, no me describas el diseño.
```

**Verifica**: abre la presentación y cuenta. En nuestra prueba se saltó una lámina.

### Paso 3 · Monta el Gem

Nombre: `Diseñador de presentaciones`. En **Conocimientos**, un documento con las dos listas: tus reglas visuales y las reglas de estructura. En **Instrucciones**:

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
Nunca describes ni cambias el diseño: de eso me encargo yo en Slides.
```

### Paso 4 · Úsalo

| Paso | Qué haces |
|---|---|
| 1 | `Con el reporte del Caso 1, arma una presentación de 6 láminas para el jefe de la oficina.` |
| 2 | En Slides, aplica **una vez** los colores y la tipografía que anotaste en el paso 1 |
| 3 | Pega el contenido lámina por lámina, incluidas las notas del orador |
| 4 | Guarda esa presentación como tu plantilla: no vuelves a hacer el paso 2 nunca |

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

* <a href="_static/sesion05/gems.html" target="_blank">🧩 Once fichas de Gems listas para montar</a> — una por programa, con su herramienta, su documento de conocimiento y sus pruebas
* <a href="_static/sesion04/prompts.html" target="_blank">📋 Todos los prompts y las tres fichas, listos para copiar</a>
* <a href="_static/sesion04/slides.html" target="_blank">Diapositivas de la sesión</a>
* <a href="_static/sesion04/guia.html" target="_blank">Guía de los tres casos</a>

## 📦 Lo que te llevas

Tres asistentes montados y probados con archivos reales, y uno de ellos adaptado a algo tuyo. En el tablero del curso: cuál adaptaste, para qué, y los dos números que recalculaste a mano en el Caso 1.
