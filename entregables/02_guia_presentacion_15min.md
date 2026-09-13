# Guía de presentación (15 minutos) — Neuronas humanas como hardware de IA

> **v2 — eje reorientado:** en vez de partir de "ventajas y desventajas técnicas", la charla ahora parte de una comparación pedagógica de **cómo se entrena una IA, cómo aprendemos nosotros, y cómo "aprende" un organoide** — usando esa simetría para disparar la pregunta filosófica de qué es la consciencia, sin cerrarla. Se apoya en el nuevo [`analisis/03`](../analisis/03_entrenamiento_comparado_y_el_debate_de_la_conciencia.md). El bloque técnico de ventajas/desventajas ([`analisis/01`](../analisis/01_ventajas_y_desventajas_tecnicas.md)) y el de gobernanza siguen presentes, pero condensados — ya no son el centro de gravedad de la charla.
>
> **Duración total:** 15:00 · **Diapositivas:** 12 · **Fecha:** 2026-09-13

---

## Objetivo y público

**Objetivo:** que el público termine la charla **sin una respuesta cerrada**, pero con las herramientas conceptuales para discutir por sí mismo si "aprender igual" implica "ser consciente igual" — y que lleve esa pregunta al debate propiamente dicho ([`entregables/01`](01_guia_debate.md)).

**Público asumido:** compañeros de clase / audiencia universitaria sin conocimiento previo — no asumir que saben qué es reinforcement learning, condicionamiento operante, ni el "hard problem" de la consciencia.

**Regla de oro:** la charla no defiende una postura filosófica (fisicalismo, dualismo o panpsiquismo) — las presenta a las tres con el mismo peso. El objetivo explícito es generar debate interno en cada persona del público, no convencerla de una respuesta. Es la diferencia entre "dar una clase" y "abrir una pregunta" — y esta charla es lo segundo.

---

## Timing general

| # | Bloque | Inicio | Duración |
|---|---|---|---|
| 1 | Portada / gancho | 0:00 | 0:45 |
| 2 | Qué es esto | 0:45 | 1:00 |
| 3 | Cómo aprende una IA convencional: premio y castigo | 1:45 | 1:30 |
| 4 | Cómo aprendemos nosotros: el bebé y el caramelo | 3:15 | 1:30 |
| 5 | Cómo "aprende" un organoide: mismo esquema, otra sustancia | 4:45 | 1:30 |
| 6 | La pregunta incómoda: ¿son la misma cosa? | 6:15 | 1:00 |
| 7 | El problema difícil de la consciencia | 7:15 | 2:00 |
| 8 | "¿Alcanza el premio y el castigo para producir consciencia?" | 9:15 | 1:30 |
| 9 | Línea de tiempo y actores comerciales (condensado) | 10:45 | 1:00 |
| 10 | La promesa técnica y su matiz (condensado) | 11:45 | 1:15 |
| 11 | ¿Está regulado? | 13:00 | 0:45 |
| 12 | Cierre: la moción reformulada | 13:45 | 1:15 |

---

## Diapositiva 1 — Portada / gancho (0:45)

**Título:** *"¿Aprender es lo mismo que ser consciente?"*

**Subtítulo:** "Neuronas humanas como hardware de inteligencia artificial"

**Qué decir:** "Hoy existe una computadora de USD 35.000 que en vez de transistores usa 800.000 neuronas humanas vivas — y aprende exactamente con el mismo esquema con el que ustedes aprendieron a no tocar la hornalla caliente. Esa frase no es una metáfora: es literal, y vamos a mostrar por qué en los próximos 15 minutos." Fuente: [03](../sources/03_cortical_labs_cl1.md).

---

## Diapositiva 2 — Qué es esto (1:00)

**Contenido clave (rápido, es solo contexto):**
- Organoide cerebral = cultivo 3D de neuronas humanas, tamaño de la punta de una aguja — no un "mini-cerebro" con anatomía completa.
- Tres nombres, mismo fenómeno: Organoid Intelligence (academia), Synthetic Biological Intelligence (Cortical Labs), wetware computing (FinalSpark).

**Qué decir:** breve, sin detenerse — es la base para poder hablar del mecanismo en la diapositiva 5. Fuente: [research.md §1](../research.md#1-qué-es-el-campo-y-cómo-se-llama).

---

## Diapositiva 3 — Cómo aprende una IA convencional: premio y castigo (1:30)

**Contenido clave:**
- Aprendizaje por refuerzo (RL): un agente prueba acciones, recibe una **señal de recompensa** (positiva o negativa), y ajusta su comportamiento para maximizar la recompensa acumulada a futuro.
- Es un ciclo de 4 pasos: observar → actuar → recibir señal → ajustar. Se repite miles de veces.
- Aclarar: la recompensa es un número que un ingeniero define de antemano — es una elección de diseño humana.

**Qué decir:** "Así aprende, por ejemplo, un programa que juega ajedrez o maneja un auto autónomo: prueba, falla o acierta, y ajusta. No hay ningún 'entendimiento' que le expliquemos — solo consecuencias." Fuente: [17](../sources/17_reinforcement_learning_basics.md).

---

## Diapositiva 4 — Cómo aprendemos nosotros: el bebé y el caramelo (1:30)

**Contenido clave:**
- Condicionamiento operante (B.F. Skinner): la conducta se moldea por sus consecuencias — refuerzo (aumenta la conducta) o castigo (la disminuye).
- El ejemplo concreto: enseñar a un bebé a usar el baño — recompensa (el caramelo) cuando lo hace bien, ausencia de recompensa o corrección cuando no.
- Dato que conviene incluir: Skinner construyó esta teoría **ignorando deliberadamente** la pregunta de qué siente el organismo — describe solo conducta observable.

**Qué decir:** "Noten el paralelo: conducta, consecuencia, ajuste de probabilidad de repetirla. Es, formalmente, el mismo esquema de la diapositiva anterior — solo que acá el 'agente' es un bebé de dos años." Fuente: [18](../sources/18_operant_conditioning_skinner.md).

---

## Diapositiva 5 — Cómo "aprende" un organoide: mismo esquema, otra sustancia (1:30)

**Contenido clave:**
- DishBrain: neuronas conectadas a un chip, reciben un estímulo eléctrico predecible cuando "aciertan" (la paleta golpea la pelota en Pong) y uno impredecible/ruido cuando fallan.
- Marco teórico: el principio de energía libre — el sistema actúa para minimizar la sorpresa/incertidumbre.
- Aprendizaje detectable en **5 minutos** de juego en tiempo real.

**Qué decir:** "Estímulo predecible, estímulo impredecible — llamalo premio y castigo si querés, porque estructuralmente es lo mismo que las dos diapositivas anteriores. Un cultivo de neuronas en una placa aprendió a jugar Pong con el mismo esquema con el que un bebé aprende a no tocar la hornalla." Fuente: [02](../sources/02_kagan_2022_dishbrain_neuron.md).

---

## Diapositiva 6 — La pregunta incómoda: ¿son la misma cosa? (1:00)

**Contenido:** mostrar los tres esquemas de las diapositivas 3-5 uno al lado del otro (mismo diagrama: conducta → consecuencia → ajuste), sin texto adicional. Es una diapositiva de silencio/pausa dramática, no de datos nuevos.

**Qué decir:** "Silicio, cerebro humano en desarrollo, cultivo de neuronas en una placa: los tres ajustan su comportamiento con el mismo esquema formal. Entonces la pregunta que tenemos que hacernos es: si el mecanismo es el mismo, ¿qué es lo que hace que a uno lo llamemos simplemente 'código' y al otro lo llamemos 'una persona'?" — dejar la pregunta flotando, no responderla todavía.

---

## Diapositiva 7 — El problema difícil de la consciencia (2:00)

**Contenido clave:**
- El "hard problem" (Chalmers): incluso explicando toda la función y estructura de un sistema, se puede seguir preguntando "¿por qué hay experiencia?" — ese salto no lo explica la ciencia estándar.
- Distinguir "problemas fáciles" (qué hace un sistema — esto sí lo explican RL, condicionamiento y principio de energía libre) del "problema difícil" (por qué eso se siente desde adentro).
- Las 3 posturas, **sin tomar partido**:
  1. **Fisicalismo/funcionalismo** — la consciencia es 100% física/funcional; en principio replicable en cualquier sustrato que cumpla la función correcta.
  2. **Dualismo** — la consciencia es de otra naturaleza, no reducible a lo físico (aquí encajan muchas tradiciones religiosas y filosóficas — la idea de "alma").
  3. **Panpsiquismo** — la experiencia es una propiedad fundamental de la materia misma, presente en distinto grado en todo, no solo en cerebros complejos.

**Qué decir:** "Noten algo contraintuitivo: bajo la postura dualista, ni la IA de silicio ni el organoide biológico son conscientes nunca — ser de carne no te salva del problema. Y bajo el panpsiquismo, quizás los dos tengan algo, aunque sea mínimo. 'Es biológico' no es, por sí solo, una respuesta." Fuente: [21](../sources/21_hard_problem_consciousness_chalmers.md).

---

## Diapositiva 8 — "¿Alcanza el premio y el castigo para producir consciencia?" (1:30)

**Contenido clave:**
- "Reward is Enough" (DeepMind, 2021): hipótesis de que maximizar una señal de recompensa alcanza, por sí sola, para producir *todas* las capacidades que asociamos a la inteligencia — sin que el argumento excluya explícitamente la experiencia subjetiva.
- Contrapeso: la réplica académica "Scalar reward is not enough" (2022) — cuestiona que una recompensa de un solo número alcance siquiera para explicar la inteligencia biológica, y advierte de los riesgos de asumir que sí.

**Qué decir:** "Uno de los laboratorios de IA más importantes del mundo apostó, en un paper serio, a que el mismo esquema de premio y castigo que vimos hoy alcanza para producir toda forma de inteligencia. No dijeron que eso incluye consciencia — pero tampoco dijeron que la excluye. Y no todo el mundo en el campo está de acuerdo." Fuentes: [19](../sources/19_reward_is_enough_2021.md), [20](../sources/20_scalar_reward_not_enough_2022.md).

---

## Diapositiva 9 — Línea de tiempo y actores comerciales (condensado) (1:00)

**Contenido clave (rápido):** 2019 Cortical Labs fundada → 2022 DishBrain → 2023 paper fundacional OI + Brainoware → 2025 CL1 comercial (USD 35.000) → 2025-26 la propia comunidad advierte sobre el hype.

**Qué decir:** "Esto pasó de laboratorio a producto con precio de lista en 4 años — mucho más rápido que cualquier respuesta seria a la pregunta que acabamos de plantear." Fuente: [research.md §2](../research.md#2-línea-de-tiempo-hitos-verificados).

---

## Diapositiva 10 — La promesa técnica y su matiz (condensado) (1:15)

**Contenido clave:**
- La promesa: eficiencia energética "un millón de veces mejor" (cerebro completo vs. supercomputadora).
- El matiz: el CL1 real consume 850-1.000W por rack — comparable a un servidor GPU convencional. La cifra de marketing nunca se midió en el producto real.

**Qué decir:** rápido — "cada vez que alguien les diga que esto es radicalmente más eficiente, pregunten: ¿comparado con qué, exactamente?" Fuentes: [analisis/01](../analisis/01_ventajas_y_desventajas_tecnicas.md), [03](../sources/03_cortical_labs_cl1.md).

---

## Diapositiva 11 — ¿Está regulado? (0:45)

**Contenido clave:** marco de 3 niveles en EE.UU. para quimeras/trasplantes, pero ninguna norma regula al organoide en sí una vez creado.

**Qué decir:** "Hay regulación — pero protege al donante, no a lo que el donante ayudó a crear." Fuente: [10](../sources/10_national_academies_neural_organoids_chimeras.md).

---

## Diapositiva 12 — Cierre: la moción reformulada (1:15)

**Contenido:** la moción original del debate, ahora precedida por la pregunta que abrió la charla:

> "Si una IA de silicio, un bebé humano y un organoide de neuronas aprenden con el mismo esquema de premio y castigo — ¿qué distingue a uno de ser 'solo código' y a otro de ser 'alguien'? Con esa pregunta abierta, empezamos el debate: ¿debería el desarrollo de 'organoid intelligence' continuar sin restricciones adicionales a las ya existentes?"

**Qué decir:** cerrar sin resolver la pregunta filosófica — es la transición directa al debate. "No les voy a dar la respuesta, porque no la hay todavía. Se las paso a ustedes."

---

## Notas de entrega

- **El corazón de la charla son las diapositivas 3 a 8** (5:30 minutos de los 15) — si el tiempo se acorta, recortar de las diapositivas 9-11 (contexto comercial/regulatorio, ya cubierto con más detalle en `research.md` y disponible para preguntas), nunca del bloque de entrenamiento/consciencia.
- **Diapositiva 6 es deliberadamente una pausa** — no llenarla de texto ni apurarla; el silencio es parte del efecto.
- **No tomar partido en la diapositiva 7.** Si alguien del público pregunta directamente "¿vos qué pensás?", la respuesta correcta en el momento es devolver la pregunta al público, no resolverla — es coherente con el objetivo de la charla.
- Evitar los errores ya detectados en el corpus: no decir "reconoce voz como Alexa" (Brainoware clasifica 8 hablantes en un set cerrado) ni presentar "Reward is Enough" como consenso científico — ver [`entregables/01 §9`](01_guia_debate.md#9-qué-no-decir-en-el-debate-errores-frecuentes-en-cobertura-mediática-ya-detectados-en-el-corpus) y [`analisis/03 §5`](../analisis/03_entrenamiento_comparado_y_el_debate_de_la_conciencia.md#5-riesgos-argumentales-a-evitar-en-la-presentación).

## Ficheros relacionados

[research.md](../research.md) · [analisis/01](../analisis/01_ventajas_y_desventajas_tecnicas.md) · [analisis/02](../analisis/02_posturas_eticas_mapa_debate.md) · [analisis/03](../analisis/03_entrenamiento_comparado_y_el_debate_de_la_conciencia.md) (nuevo — sostiene el eje central de esta versión) · [entregables/01_guia_debate.md](01_guia_debate.md) · [entregables/04_prompt_claude_design_edicion.md](04_prompt_claude_design_edicion.md) (prompt para editar el canvas ya diseñado con esta nueva estructura)
