---
title: Sesión 7 · Tus datos, con IA
---
# Sesión 7 · Tus datos, con IA 📊📂

Excel, correos, chats, fotos y audios: la IA hace el trabajo pesado —leer mil filas, treinta correos, diecinueve fotos— y tú haces lo que ella no puede: revisar, decidir y firmar.

Todo el material es de **un mismo negocio inventado**, Café de Altura La Cumbre, una tostadora de Manizales. Los archivos se cruzan entre sí: lo que se ve raro en uno se explica en otro.

## 🧰 Herramientas del día

| Para qué | Herramienta |
|---|---|
| Excel, correos, chats, fotos y formatos | [ChatGPT](https://chatgpt.com) |
| Trabajar dentro de la hoja de cálculo | ChatGPT para Excel y Google Sheets |
| Las notas de voz | [Gemini Notebook](https://notebooklm.google.com) (antes NotebookLM) |

```{warning}
**ChatGPT gratis permite solo 3 subidas de archivos al día.** Por eso cada caso viene en un solo archivo: el negocio entero en un Excel con varias hojas, las 19 fotos dentro de un PDF, los 30 correos en un `.txt`. Hoy eliges **tres casos**.

**ChatGPT gratis no recibe audio.** Las notas de voz van por Gemini Notebook.
```

## 📽️ Material

* <a href="_static/sesion07/materiales-sesion07.zip">⬇️ Todos los archivos de la sesión (ZIP)</a>
* <a href="_static/sesion07/S07_datos_con_IA.pptx">⬇️ Presentación (PowerPoint)</a>

| Archivo | Qué es |
|---|---|
| `cafe_la_cumbre_2026.xlsx` | Ventas, cosecha, proveedores y compras, de enero a septiembre |
| `competencia_por_completar.xlsx` | Las marcas de la competencia, con casillas vacías |
| `bandeja_entrada.txt` | 30 correos de julio a septiembre |
| `chat_equipo_atencion.txt` | El grupo de WhatsApp del equipo de atención |
| `fotos_visita_Buenavista.pdf` | 19 fotos de una visita técnica a una finca |
| `bitacoras_completas.mp3` | 4 notas de voz de los técnicos de campo |
| `formato_FT07_informe_visita.docx` | El formato de informe que hay que llenar |
| `plantilla_carta_practica.docx` | Una carta de solicitud de práctica |

---

## 🧠 Antes de empezar: ¿calculó o interpretó?

Cuando le das un archivo a ChatGPT hace una de dos cosas:

* **Calcula.** Con un Excel escribe un pequeño programa, lo ejecuta y te da el resultado. Es exacto. Lo reconoces porque aparece **«Analizado»**.
* **Interpreta.** Con un chat, un correo o una foto lee y entiende, como una persona apurada. La historia suele salir bien; los números, aproximados.

Si vas a decidir con esos números, pídele que los **calcule con código**. Y si te dice *"no encontré otros problemas"*, no lo tomes como garantía: pregúntale por cosas concretas.

## ⛔ Antes de subir nada

| Regla | Por qué |
|---|---|
| **Nada confidencial** | Ni historias clínicas, ni expedientes, ni datos de clientes. Si hay que hacerlo, cambia nombres por códigos |
| **Ojo al conectar tu correo** | En los planes personales, si tienes activada la opción *Mejorar el modelo para todos*, OpenAI puede usar la información de las apps conectadas para entrenar. Desactívala en Configuración → Controles de datos |
| **Los números se revisan** | Si interpretó en vez de calcular, puede estar lejos |
| **Lo que firmas es tuyo** | El informe lo firma quien lo entrega, no ChatGPT |

---

## Los casos

### 1 · Revisar antes de calcular · `cafe_la_cumbre_2026.xlsx`

```
Este archivo es de una tostadora de café. Antes de calcular nada, revisa la hoja
Ventas y dime qué problemas de calidad de datos encuentras: duplicados, vacíos,
nombres mal escritos, valores imposibles. Dime cuántas filas afecta cada uno.
No corrijas nada todavía.
```

Cuando te responda, pregúntale por algo concreto que no haya mencionado: precios fuera de lo normal, errores de ortografía. ¿Cuántos problemas encontró la primera vez y cuántos después?

### 2 · Preguntas y gráficas · *misma conversación*

```
Quita los duplicados y haz tres gráficas: ventas por mes, ventas por canal y los
cinco productos que más venden. Después dime en tres líneas qué le recomendarías
al dueño.
```

Para comprobarlo: *"¿cuántas filas usaste para esta suma?"*

### 3 · El tablero · *misma conversación*

```
Arma un tablero de una sola página para el dueño: arriba cuatro números grandes
(ventas totales, mejor mes, canal principal, ticket promedio) y abajo tres
gráficas. Que se entienda en diez segundos.
```

### 4 · Cruzar dos tablas · *misma conversación*

```
En la hoja Compras calcula para cada proveedor el promedio de días de retraso
(entrega real menos entrega pactada) y el porcentaje de pedidos no conformes.
Cruza eso con la calificación de la hoja Proveedores. ¿La calificación refleja
lo que muestran los datos?
```

Y en la hoja **Cosecha** (lee primero la pestaña *Cómo leer esta hoja*): ¿qué lote tiene la humedad fuera de norma? ¿Qué finca tiene el factor de rendimiento empeorando? Los datos dicen *qué* pasa. El *por qué* está en los audios del caso 10.

### 5 · El Excel conectado · `competencia_por_completar.xlsx`

Aquí ChatGPT no recibe un archivo: vive **dentro de la hoja**, como barra lateral. En Google Sheets: **Extensiones → Complementos → buscar «ChatGPT»**. No gasta tus subidas del día.

```
Completa las casillas vacías buscando en internet. En una columna nueva pon la
fuente de cada dato. Si no lo encuentras, escribe "No encontrado".
```

Un dato buscado sin fuente no se puede verificar: abre tres fuentes al azar y compruébalas.

### 6 · La bandeja de correo · `bandeja_entrada.txt`

```
Es la exportación de la bandeja de correo de compras de una tostadora de café.
Haz una tabla con todos los correos: fecha, quién lo manda, asunto en pocas
palabras y una categoría (factura o gasto, pedido de cliente, queja, proveedor,
interno, publicidad, sospechoso). Si algún correo te parece peligroso, dime por qué.
```

### 7 · Los gastos que llegan por correo · *misma conversación*

```
Haz un resumen de gastos: suma de las facturas por mes y por tipo de gasto, con
una gráfica. Dime también cuáles vencen en los próximos 15 días a partir del
25 de septiembre.
```

¿Sumó por la fecha del correo o por el mes del servicio? Para el flujo de caja sirve una; para saber cuánto cuesta producir, la otra.

### 8 · La conversación, convertida en historia · `chat_equipo_atencion.txt`

```
Es la exportación de un grupo de WhatsApp del equipo de atención al cliente de
una tostadora, de julio a septiembre. Clasifica cada caso en un tema (envío tarde,
producto equivocado, empaque dañado, pregunta por suscripción, felicitación,
precio, exportación). Haz una gráfica de cuántos casos hubo de cada tema por mes,
y después cuéntame en cinco líneas qué historia cuentan los datos: qué empeoró,
qué mejoró y qué oportunidad de negocio aparece.
```

Para que los números sean exactos: *"usa código para contar los casos, y muéstrame qué palabras usaste para identificar cada tema"*.

### 9 · De fotos a informe de campo · `fotos_visita_Buenavista.pdf` + `formato_FT07_informe_visita.docx`

```
Eres el técnico que hizo la segunda visita a la finca Buenavista (Neira, Caldas)
el 23 de septiembre de 2026. El PDF tiene las 19 fotos que tomaste, cada una con
su nombre. Llena el formato FT-07 con lo que se ve en las fotos. Reglas: en cada
hallazgo cita la foto (IMG_xxxx) que lo respalda; si algo no se puede saber por
las fotos, escribe "No registrado" y no lo inventes. Al final dime qué fotos no
aportaron nada.
```

¿Firmarías este informe?

### 10 · De notas de voz a informe · `bitacoras_completas.mp3` + el formato FT-07

En **Gemini Notebook**: crea un cuaderno, agrega el MP3 como fuente y también el formato FT-07.

```
Las fuentes son cuatro notas de voz de técnicos que visitaron fincas cafeteras y
el formato FT-07. Diligencia un formato FT-07 por cada visita, usando solo lo que
dicen los audios. Si un campo no se menciona, escribe "No registrado". Indica en
qué parte del audio se dice cada cosa.
```

### 11 · La carta, con tus propios datos · `plantilla_carta_practica.docx`

```
Llena esta plantilla con lo que sabes de mí. No inventes nada: si te falta un
dato, pregúntamelo antes de escribir. En "por qué esa empresa", no escribas
elogios genéricos: pregúntame qué me interesa de verdad. Al final, señala las
frases que suenan a plantilla para que yo las cambie.
```

La cédula y el teléfono, mejor escríbelos tú al final.

---

## 🎬 Tu turno

Elige **tres casos**. Algunas combinaciones que caben en las tres subidas del día:

| Perfil | Casos |
|---|---|
| **El analista** | Excel (1 a 4) + correos (6 y 7) + chat (8) |
| **El de campo** | Excel (1 a 4) + fotos con formato (9) |
| **El de oficina** | Correos (6 y 7) + chat (8) + carta (11) |

Los audios (10) y el Excel conectado (5) no gastan subidas de ChatGPT.

**Lo que entregas:** por cada caso, el prompt que usaste, el resultado, y **una cosa que comprobaste por tu cuenta** —una suma, una foto, un dato buscado—.

**Para tu carrera:** repite uno de los casos con un archivo de tu área, siempre con datos inventados o anonimizados.

```{admonition} Créditos
:class: note
Las fotografías provienen de Wikimedia Commons, con licencias libres. Los créditos están en `CREDITOS.txt`, dentro del ZIP. Los datos del negocio, los correos, el chat y las voces de los audios son inventados.
```
