# Guía de presentación (15 minutos) — Neuronas humanas como hardware de IA

> Estructura lista para exponer, con timing por bloque, contenido de cada diapositiva y qué decir. Pensada como introducción/contexto **previo al debate** ([`entregables/01_guia_debate.md`](01_guia_debate.md)), no como el debate en sí — por eso el cierre termina lanzando la moción, no tomando posición.
>
> **Duración total:** 15:00 · **Diapositivas:** 11 · **Fecha:** 2026-09-13

---

## Objetivo y público

**Objetivo:** que el público entienda, en 15 minutos, (1) qué es esto realmente (sin sensacionalismo), (2) qué se puede sostener con evidencia y qué es marketing, y (3) por qué el debate ético no es un simple sí/no — para llegar preparado a discutirlo.

**Público asumido:** compañeros de clase / audiencia universitaria sin conocimiento previo del tema — no asumir que saben qué es un organoide o un MEA.

**Regla de oro para la exposición:** cada vez que se menciona una cifra fuerte (ej. "millón de veces más eficiente"), inmediatamente decir el matiz. Es el hilo conductor de toda la charla — no dejarlo solo para el final.

---

## Timing general

| # | Bloque | Inicio | Duración |
|---|---|---|---|
| 1 | Portada / gancho | 0:00 | 0:45 |
| 2 | Qué es esto | 0:45 | 1:30 |
| 3 | Cómo funciona | 2:15 | 2:00 |
| 4 | Línea de tiempo | 4:15 | 1:30 |
| 5 | Los dos jugadores comerciales | 5:45 | 1:00 |
| 6 | La promesa: ventajas | 6:45 | 1:30 |
| 7 | El matiz: lo que no se dice tanto | 8:15 | 1:45 |
| 8 | La ética no es una sola pregunta | 10:00 | 2:00 |
| 9 | ¿Está regulado? | 12:00 | 1:00 |
| 10 | Cierre y moción del debate | 13:00 | 1:00 |
| 11 | Preguntas / margen | 14:00 | 1:00 |

---

## Diapositiva 1 — Portada / gancho (0:45)

**Título:** *"¿Y si la computadora que entrena tu IA... estuviera viva?"*

**Contenido visual:** título + subtítulo ("Neuronas humanas como hardware de inteligencia artificial") + imagen conceptual (organoide sobre un chip).

**Qué decir:** abrir con el hecho concreto, no con la pregunta retórica sola — "Desde 2025 existe una computadora que se vende por USD 35.000 y que en vez de transistores usa 800.000 neuronas humanas vivas. No es ciencia ficción: se llama CL1 y la fabrica una empresa australiana." Fuente: [03](../sources/03_cortical_labs_cl1.md).

---

## Diapositiva 2 — Qué es esto (1:30)

**Contenido clave:**
- Definición simple: cultivos 3D de neuronas humanas (derivadas de células madre) del tamaño de la punta de una aguja, conectados a electrodos.
- Aclarar de entrada: **no es un "mini-cerebro" con anatomía completa** — es un cultivo celular.
- Tres nombres para lo mismo, según quién lo dice: **Organoid Intelligence** (academia, Johns Hopkins), **Synthetic Biological Intelligence** (Cortical Labs), **wetware computing** (FinalSpark).

**Qué decir:** remarcar que la variedad de nombres no es casualidad — cada término viene de un actor con un interés distinto (investigación académica vs. producto comercial vs. plataforma de acceso remoto). Fuente: [research.md §1](../research.md#1-qué-es-el-campo-y-cómo-se-llama).

---

## Diapositiva 3 — Cómo funciona (2:00)

**Contenido visual:** el diagrama de flujo de [`research.md §3`](../research.md#3-cómo-funciona-técnicamente-denominador-común) (donante → iPSC → organoide → MEA → estímulo/respuesta → aprendizaje).

**Contenido clave:**
- El organoide se conecta a un array de microelectrodos (MEA) que estimula y registra actividad eléctrica.
- Dos formas de usarlo: (1) que la propia neurona "aprenda" por feedback (DishBrain, principio de energía libre), o (2) usarlo como "caja negra" que transforma señales, sin que aprenda nada — solo se entrena una capa externa (Brainoware, reservoir computing).

**Qué decir:** este es el momento técnico más denso — ir despacio. "No hace falta entender la neurociencia de fondo, solo esto: hay un cultivo de neuronas, un chip que le manda pulsos eléctricos y lee su respuesta, y un algoritmo que interpreta esa respuesta como resultado de cómputo." Fuentes: [02](../sources/02_kagan_2022_dishbrain_neuron.md), [04](../sources/04_brainoware_2023.md).

---

## Diapositiva 4 — Línea de tiempo: de laboratorio a producto en 4 años (1:30)

**Contenido visual:** timeline horizontal 2019→2026 (ver tabla completa en [`research.md §2`](../research.md#2-línea-de-tiempo-hitos-verificados)).

**Hitos a mostrar (los 6 más importantes, no los 10 de la tabla completa):**
- 2019 — Fundación de Cortical Labs
- 2022 — DishBrain aprende Pong en 5 minutos
- 2023 — Paper fundacional de "Organoid Intelligence" + Brainoware reconoce voz
- 2025 — Cortical Labs lanza el CL1 (primer producto comercial)
- 2025-26 — Los propios científicos del campo advierten sobre el exceso de promesas

**Qué decir:** el punto de esta diapositiva es la **velocidad**: "en menos de 4 años pasó de un experimento de laboratorio a un producto con precio de lista — mucho más rápido de lo que tardó en aparecer cualquier discusión seria de regulación." Es el gancho hacia el bloque de ética.

---

## Diapositiva 5 — Los dos jugadores comerciales (1:00)

**Contenido visual:** tabla comparativa Cortical Labs (CL1) vs. FinalSpark (Neuroplatform) — usar la tabla de [`research.md §4`](../research.md#4-actores-comerciales-comparación) simplificada a 4 filas: modelo de negocio, escala, consumo declarado, precio de acceso.

**Qué decir:** rápido, sin detenerse mucho — es contexto de mercado, no el núcleo de la charla. "Uno vende el hardware, el otro alquila acceso remoto — dos modelos de negocio distintos para la misma tecnología base."

---

## Diapositiva 6 — La promesa: ventajas argumentadas (1:30)

**Contenido clave (3 argumentos, con cifra):**
1. **Eficiencia energética:** cerebro humano completo ≈ 1 exaFLOPS a 10-20W, vs. 21 megavatios de una supercomputadora equivalente → ventaja de ~10⁶.
2. **Eficiencia de datos:** DishBrain aprende en 5 minutos; AlphaGo necesitó 160.000 partidas de entrenamiento.
3. **Ya hay demanda comercial real:** CL1 vendido, Neuroplatform con suscriptores pagos.

**Qué decir:** presentar estos argumentos **con toda su fuerza**, sin adelantar el matiz todavía — el contraste con la diapositiva siguiente es el punto dramático de la charla. Fuentes: [01](../sources/01_smirnova_2023_organoid_intelligence.md), [14](../sources/14_orf_overview_ventajas_desafios.md).

---

## Diapositiva 7 — El matiz: lo que no se dice tanto (1:45)

**Esta es la diapositiva más importante de la charla — dedicarle el tiempo que pide.**

**Contenido clave (contrarresta cada punto de la diapositiva 6, en el mismo orden):**
1. La cifra de "10⁶ veces más eficiente" compara el **cerebro humano completo** (86.000 millones de neuronas) contra una supercomputadora — **no** un organoide real de laboratorio (100.000-800.000 células) contra un chip equivalente.
2. El CL1 real, con todo su sistema de soporte, consume **850-1.000 W por rack de 30 unidades** — comparable a un servidor GPU convencional. La ventaja teórica no se mide nunca en el producto real.
3. Montar un laboratorio de este tipo cuesta **USD 50.000 a 250.000+** de infraestructura — no es una tecnología barata hoy.
4. Límite físico duro: sin vascularización, el organoide necrosa su núcleo a partir de ~300 micrones — **no hay solución conocida a corto plazo**, no es solo falta de escala.

**Qué decir:** "Cada una de estas cifras de eficiencia es real — el problema es a qué la comparan. Ninguna fuente pública mide el sistema completo contra un chip haciendo la misma tarea." Fuentes: [analisis/01](../analisis/01_ventajas_y_desventajas_tecnicas.md), [03](../sources/03_cortical_labs_cl1.md), [16](../sources/16_starting_sbi_lab_patterns_2025.md).

---

## Diapositiva 8 — La ética no es una sola pregunta (2:00)

**Contenido visual:** los 5 ejes de [`analisis/02 §6`](../analisis/02_posturas_eticas_mapa_debate.md#6-tabla-resumen-para-armar-equipos-de-debate) en formato de lista o diagrama radial — no leer las tablas completas, solo nombrar cada eje con su pregunta.

**Los 5 ejes (una frase cada uno):**
1. ¿Puede el organoide **sufrir**? (Milford, Shaw & Starke — el propio marco teórico de DishBrain podría implicar displacer al fallar)
2. ¿Es válido el **consentimiento** del donante si ni la ciencia sabe qué está autorizando?
3. ¿Daña la **dignidad humana** aunque el organoide nunca sufra? (Hanna — objeción que no depende de resolver la consciencia)
4. ¿Es un problema de **marketing**, no de ética? (los propios científicos del campo lo advierten)
5. ¿Está bien **encuadrado el debate público** mismo? (el framing cambia el apoyo más que los hechos)

**Qué decir:** "No hay un bando 'a favor' y uno 'en contra' — hay cinco preguntas distintas, y alguien puede responder sí a unas y no a otras sin contradecirse." Este es el mensaje que el público debe llevarse antes del debate.

---

## Diapositiva 9 — ¿Está regulado? (1:00)

**Contenido clave:**
- En EE.UU. existe un marco de **tres niveles** (verde/amarillo/rojo) para quimeras y trasplantes neuronales.
- **Pero:** ninguna norma regula directamente al **organoide en sí** una vez creado — toda la regulación protege al donante humano. Una propuesta del NIH de 2016 para reforzar esto nunca se finalizó.

**Qué decir:** breve y directo — "sí hay regulación, pero tiene un agujero específico: nadie regula qué se le puede hacer al organoide una vez que existe." Fuente: [10](../sources/10_national_academies_neural_organoids_chimeras.md).

---

## Diapositiva 10 — Cierre y moción del debate (1:00)

**Contenido:** resumir la tensión central en una frase, y lanzar la moción textual del debate (ver [`entregables/01 §1`](01_guia_debate.md#1-moción-sugerida)):

> *"Este foro considera que el desarrollo de 'organoid intelligence' debería continuar sin restricciones adicionales a las ya existentes."*

**Qué decir:** "La evidencia técnica es real pero acotada, la promesa de eficiencia está sobrevendida, y la ética no se resuelve con un sí o un no. Con eso como punto de partida, empezamos el debate."

---

## Diapositiva 11 — Preguntas / margen (1:00)

Colchón de tiempo. Si no hay preguntas del público, usar el minuto para repetir la moción y anunciar el formato del debate (roles, tiempo por equipo).

---

## Notas de entrega

- **No se puede improvisar la diapositiva 7** (el matiz) — es el corazón argumental de toda la charla; si el tiempo se acorta, recortar de la diapositiva 5 (jugadores comerciales) o la 9 (regulación), nunca de la 6-7.
- Evitar los errores de cobertura mediática ya detectados: no decir "reconoce voz como Alexa" (es clasificación cerrada de 8 hablantes, no reconocimiento abierto) ni repetir "un millón de veces más eficiente" sin el matiz — ver [`entregables/01 §9`](01_guia_debate.md#9-qué-no-decir-en-el-debate-errores-frecuentes-en-cobertura-mediática-ya-detectados-en-el-corpus).
- Practicar el diagrama de la diapositiva 3 en voz alta — es el punto donde más fácil se pierde al público si se habla muy rápido.

## Ficheros relacionados

[research.md](../research.md) · [analisis/01](../analisis/01_ventajas_y_desventajas_tecnicas.md) · [analisis/02](../analisis/02_posturas_eticas_mapa_debate.md) · [entregables/01_guia_debate.md](01_guia_debate.md) · [entregables/03_prompt_claude_design.md](03_prompt_claude_design.md) (prompt para generar el diseño visual de estas 11 diapositivas)
