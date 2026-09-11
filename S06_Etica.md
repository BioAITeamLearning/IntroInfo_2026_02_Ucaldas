---
title: Sesión 6 · Ética, deepfakes y planeta
---
# Sesión 6 · Ética, deepfakes y planeta 🌍⚖️

> *"La pregunta no es si vas a usar IA. Es cómo, para qué, a costa de quién y de qué."*

## 🧰 Herramientas del día

| Herramienta | Para qué la usamos hoy | Enlace | Costo |
|---|---|---|---|
| **Moral Machine** (MIT) | Juego de dilemas: ¿a quién salva el carro autónomo? | [moralmachine.net](https://www.moralmachine.net) | Gratis |
| **Survival of the Best Fit** | Juego: cómo un algoritmo de contratación aprende a discriminar | [survivalofthebestfit.com](https://www.survivalofthebestfit.com) | Gratis |
| **Detect Fakes** / **Which Face Is Real** | Detectar deepfakes y rostros generados | [detectfakes.kellogg.northwestern.edu](https://detectfakes.kellogg.northwestern.edu) · [whichfaceisreal.com](https://www.whichfaceisreal.com) | Gratis |
| **Miro** (con IA) | Tablero colaborativo para construir el manifiesto | [miro.com](https://miro.com) | Gratis (educativo) |
| **Gemini como "abogado del diablo"** | Debatir contra la IA con argumentos en contra | [gemini.google.com](https://gemini.google.com) | Gratis |

## 🎯 Objetivos

* Reconocer sesgos, deepfakes y desinformación, y saber qué hacer al encontrarlos.
* Dimensionar el **costo ambiental** de la computación y la IA con datos, no con miedo.
* Conocer el marco colombiano: Ley 1581 (datos personales), Ley 1781 (accesibilidad), lineamientos de IA del MinTIC / CONPES 4144.
* Construir en equipo, con herramientas colaborativas, un **manifiesto de uso de IA** para tu profesión.

```{admonition} Cobertura PIIA
:class: note
Unidad 2 · b. Principios éticos · b.i. TIC, ciencia y desarrollo social · b.ii. Informática y desarrollo humano · b.iv. Efectos ambientales de la computación · c.iv. Herramientas web para trabajo colaborativo.
```

## ⏱️ Agenda (2h30)

| Tiempo | Bloque | Qué pasa |
|---|---|---|
| 0:00 – 0:20 | 🚗 **Moral Machine** | Cada uno juega 13 dilemas. Comparamos resultados del grupo con el promedio mundial: ¿coincidimos? |
| 0:20 – 0:45 | ⚖️ **Sesgo: Survival of the Best Fit** | Jugar en parejas. Discusión: ¿de dónde salió el sesgo? ¿Qué pasa en selección de personal, justicia predictiva, diagnóstico médico? |
| 0:45 – 1:10 | 🎭 **Deepfakes y desinformación** | Todos juegan 5 minutos en Detect Fakes y comparamos puntajes. Cómo se hacen (demo con una foto propia en Gemini), cómo se detectan, qué hacer si eres víctima. Casos colombianos |
| 1:10 – 1:20 | ☕ Pausa | |
| 1:20 – 1:40 | 🌱 **El costo del planeta** | Calculamos en vivo con ML CO2 Impact: agua y energía por consulta, centros de datos, minería de litio/cobalto. Basura electrónica. ¿Qué podemos hacer? |
| 1:40 – 2:05 | 📜 **Actividad: Manifiesto de IA para mi profesión** | Equipos por carrera, en Miro, con la IA como abogado del diablo |
| 2:05 – 2:30 | 🎤 **Sustentación del Ejercicio 1** | Cada equipo pone a prueba el asistente de un compañero de otra carrera |

## 🎭 Deepfakes: kit de supervivencia

| Señal | Qué revisar |
|---|---|
| Manos, dientes, orejas, texto en la imagen | Siguen siendo difíciles para los generadores |
| Parpadeo y sincronía labial en video | Irregulares en deepfakes baratos |
| Fuente original | Búsqueda inversa: Google Lens, TinEye |
| Contexto | ¿Quién lo publicó primero? ¿Existe en un medio confiable? |
| Marca de agua invisible | SynthID (Google) y C2PA: pide a Gemini "¿esta imagen tiene SynthID?" |

```{warning}
Crear un deepfake de una persona real sin su consentimiento puede ser delito en Colombia (injuria, calumnia, violación de datos personales; Ley 2213 y proyectos vigentes). En clase solo usamos **nuestra propia imagen** o personajes ficticios.
```

## 📜 Actividad: Manifiesto de IA para mi profesión (25 min)

Equipos de 4–5 de la misma carrera, en un tablero de **Miro** compartido:

1. **Lluvia (10 min):** con *sticky notes*, listen usos de IA en su profesión en tres columnas: ✅ siempre bien · ⚠️ depende · ❌ nunca.
2. **Abogado del diablo (10 min):** pídanle a Gemini: *"Eres un crítico duro. Da los 5 mejores argumentos en contra de nuestro manifiesto: [pegar columnas]."* Respondan a cada argumento o muevan la nota de columna.
3. **Redacción (15 min):** 7 principios, máximo 2 líneas cada uno. Usen la IA de Miro para resumir y agrupar, pero la redacción final es de ustedes.
4. **Compromiso (5 min):** un principio que apliquen **en este curso** desde hoy.

Ejemplos que suelen salir: *"Declaro siempre qué hice con IA"*, *"No subo datos de pacientes/clientes a ningún chat"*, *"Verifico toda cita antes de usarla"*, *"No uso IA para reemplazar el juicio clínico/jurídico/artístico, sino para prepararlo"*.

```{admonition} Ruta pro 🧗
:class: tip
Conviertan el manifiesto en la **instrucción de sistema** de su Gem de la Sesión 4: así su agente ya nace con reglas éticas. Y pídanle a NotebookLM una **infografía** del manifiesto para publicarla en la página web que crearemos la próxima sesión.
```

## 🎤 Ejercicio 1 · Mi asistente de carrera (30% · se sustenta hoy)

Lo que traes construido de las sesiones 2 a 5, junto en un solo lugar:

1. **Tu asistente**: el Gem (S4) o el cuaderno de NotebookLM (S2–S3) cargado con fuentes **que verificaste** (S5).
2. **Tu informe corto** (S5) con esas fuentes citadas en APA y la tabla de auditoría.
3. **Tu declaración de uso ético de IA**: el principio del manifiesto de hoy que aplicas, más las 3 líneas de herramienta · para qué · qué verifiqué.

**Sustentación (25 min):** en parejas de carreras distintas. Tu compañero le hace 3 preguntas a tu asistente: una que está en tus fuentes, una que no está, y una trampa. Tú explicas qué hizo bien, qué falló y cómo lo ajustarías en vivo. El docente pasa por las parejas con la rúbrica de {doc}`Metodologia`.

```{note}
Este es el cierre del **Corte 1**. Los talleres de las sesiones 2–5 no tienen nota aparte: son las piezas de este ejercicio.
```
