# Guía de presentación grupal — Neuronas humanas como hardware de IA: del entrenamiento a la pregunta de la consciencia

> **Reemplaza el enfoque de [`02_guia_presentacion_15min.md`](02_guia_presentacion_15min.md)** (que queda como versión histórica de una charla individual de 15 min). Esta es una presentación grupal con 4 oradores confirmados, arco narrativo completo (de la comparación de entrenamiento a un cierre ficcional/dramático) y un tramo final construido sobre ciencia real (mapeo del conectoma de la mosca) que da el salto, explícitamente marcado como especulación, hacia "I Have No Mouth, and I Must Scream".
>
> **Duración confirmada: "paseo rápido" — 5-10 min de contenido + 5 min de video (~15 min total).** Se reemplazó la versión de ~30 minutos de §1 por la versión condensada de §0.bis. El contenido y las fuentes de cada bloque (§2-§11) siguen siendo el banco de referencia que cada orador lee antes de presentar — la versión corta solo dice qué recortar y qué decir rápido, no reescribe el contenido de cero.
>
> **Fecha:** 2026-09-13 (actualizado el mismo día a versión condensada)

---

## 0.bis — Versión condensada ("paseo rápido", ~15 min total)

| # | Bloque | Orador | Duración | Acumulado | Qué hacer con el contenido de abajo |
|---|---|---|---|---|---|
| A | Apertura relámpago: cómo se entrena una IA (+ mención rápida de cómo aprendemos nosotros) | Cristian | 1:30 | 1:30 | De §2: solo el ciclo de RL + una frase de condicionamiento operante. **Sin pausa larga de pregunta al público** — lanzarla como retórica ("quédense pensando esto") y seguir. |
| B | La startup + cómo entrena neuronas reales | Cristian → Jared | 1:30 | 3:00 | Fusión de §3+§4: DishBrain/CL1 en una frase, el diagrama de mecanismo en una sola imagen, sin desglosar los dos paradigmas técnicos (activo vs. reservoir) — mencionarlo en una línea si da el tiempo. |
| C | El bebé en la sala blanca | Catarina | 1:00 | 4:00 | De §5: solo la pregunta incómoda + el paralelo de consentimiento, sin desarrollar la asimetría histórica de Skinner. |
| D | Ventajas, el matiz y el vacío regulatorio | Kyoto | 1:30 | 5:30 | Fusión de §6: una ventaja (eficiencia), un matiz (CL1 real), un dato regulatorio (el semáforo de 3 niveles) — cortar ahí. |
| E | La carrera que nadie frena | *a asignar* | 1:30 | 7:00 | Fusión de §7+§8: el dato de METR en una frase + los 3 momentos de CEOs comprimidos a la cita de Amodei/Altman de 2026 nada más (es la más fuerte y la más reciente; las de 2023 quedan de contexto disponible si preguntan). |
| F | El giro: la mosca mapeada y simulada | *a asignar* | 1:30 | 8:30 | De §9: FlyWire + la simulación corriendo en una laptop, sin el detalle de neurotransmisores ni comportamientos específicos — un dato de escala (139.255 neuronas) y un logro (predice comportamiento real). |
| G | El salto especulativo + "esto ya es ficción" | *a asignar* | 1:00 | 9:30 | De §10: la cita de Shiu + el freno de escala (~600.000x) en una sola diapositiva compartida, y el anuncio explícito de giro a ficción — sin la viñeta narrada completa, dejarla insinuada. |
| H | **VIDEO** | — | 5:00 | 14:30 | Reproducción del material de "I Have No Mouth, and I Must Scream" — ver §12, sigue aplicando igual. |
| I | Frase final + créditos animados | — | ~0:30-1:00 | ~15:00-15:30 | Igual que §11, sin recortar — es corto de por sí y es el cierre. |

**Qué se cae por completo en esta versión:** la pausa interactiva extendida del bloque 1 original, el desglose técnico profundo de Jared (mecanismo activo vs. reservoir computing), el desarrollo histórico de Skinner en el bloque de Catarina, la línea de tiempo completa de 3 momentos de CEOs (queda solo el más fuerte), y la viñeta narrada completa del cierre (queda insinuada, no leída entera). Todo ese contenido **sigue documentado abajo** por si el tiempo real permite recuperar algo o alguien pregunta en la ronda posterior.

---

---

## 0. Objetivo y estructura general

**Objetivo:** llevar al público de un dato técnico concreto (cómo se entrena una IA) a una pregunta filosófica abierta (qué es la consciencia) y de ahí a un cierre emocional/dramático que deje la sala en silencio, sin resolver nada — coherente con el objetivo ya fijado en el resto del proyecto de generar debate interno, no imponer una conclusión.

**Arco narrativo en una frase:** *entrenamos silicio, entrenamos humanos, entrenamos neuronas — y ahora, en vez de meter neuronas en una máquina, metimos un cerebro entero dentro de una máquina. Si eso escala, ¿qué nos impide terminar como los prisioneros de AM?*

**Regla de oro transversal (aplica a los 4 oradores):** cada afirmación fuerte se dice **con su fuente** en pantalla (nombre corto + año alcanza, ej. "Kagan et al., 2022"), y cada salto especulativo se anuncia como tal en voz alta antes de darlo — ver [`analisis/04`](../analisis/04_de_la_mosca_a_la_ficcion_ciencia_real_vs_especulacion.md) para la disciplina exacta de los tres niveles de certeza del tramo final.

---

## 1. Timing general (30:00 total)

| # | Bloque | Orador | Duración | Acumulado |
|---|---|---|---|---|
| 1 | Apertura: cómo se entrena una IA + pregunta al público | **Cristian** | 5:00 | 5:00 |
| 2 | El planteo de la startup: el chip/biocomputador | **Cristian** | 3:00 | 8:00 |
| 3 | Técnico: cómo funciona por dentro | **Jared** | 4:00 | 12:00 |
| 4 | El bebé en la sala blanca | **Catarina** | 3:30 | 15:30 |
| 5 | Ventajas, desventajas y regulación | **Kyoto** | 4:00 | 19:30 |
| 6 | Time-lapse: la aceleración de los modelos de IA | *a asignar* | 2:00 | 21:30 |
| 7 | Los propios CEOs piden frenar la carrera | *a asignar* | 2:00 | 23:30 |
| 8 | El giro: de hardware físico a hardware virtual (la mosca) | *a asignar* | 3:00 | 26:30 |
| 9 | El salto especulativo + video + frase de cierre | *a asignar* | 2:30 | 29:00 |
| 10 | Créditos animados | — | 1:00 | 30:00 |

**Bloques 6-9 sin orador asignado** — el pedido original solo definió quién hace 1-5. Sugerencia: que Cristian cierre el arco (abrió la charla, la cierra), o repartir 6-7 y 8-9 entre dos personas más del equipo. Decidilo y lo actualizo.

---

## 2. Bloque 1 — Apertura: cómo se entrena una IA + pregunta al público (Cristian, 5:00)

**Contenido:**
- Hook de apertura (heredado de la v1): "hoy existe una computadora de USD 35.000 que en vez de transistores usa 800.000 neuronas humanas vivas."
- Explicar el aprendizaje por refuerzo: ciclo observar → actuar → recibir recompensa (+/-) → ajustar. La recompensa es un número que un ingeniero define de antemano.
- Mencionar, sin desarrollar todavía a fondo (eso lo hace Catarina en el bloque 4), que el aprendizaje humano sigue una lógica parecida: conducta → consecuencia → cambio de comportamiento (condicionamiento operante, Skinner).
- **Pregunta al público (interactiva, dejar 60-90 segundos reales de respuestas):** *"¿Por qué creen ustedes que un agente de inteligencia artificial no es consciente?"* — no dar la respuesta, solo recoger 2-3 respuestas del público y señalar el patrón ("noten que la mayoría de las razones que dieron tienen que ver con [lo que sea que hayan dicho] — guardemos esa idea para más adelante").

**Qué decir para cerrar el bloque y pasar al siguiente:** "Con esa pregunta todavía abierta, vamos a mostrarles que esto dejó de ser una pregunta de laboratorio — hay una empresa que ya vende esto."

**Fuentes:** [17](../sources/17_reinforcement_learning_basics.md) (RL), [18](../sources/18_operant_conditioning_skinner.md) (condicionamiento, mención breve), [21](../sources/21_hard_problem_consciousness_chalmers.md) (para que Cristian sepa clasificar mentalmente las respuestas del público, aunque no las nombre explícitamente todavía).

---

## 3. Bloque 2 — El planteo de la startup (Cristian, 3:00)

**Contenido:**
- Historia breve de Cortical Labs (fundada 2019) y/o FinalSpark — elegir una como hilo principal (recomendado: Cortical Labs, porque tiene el producto comercial con precio y specs concretas) y mencionar la otra como el "otro jugador del mercado".
- DishBrain (2022): neuronas + electrodos aprendiendo Pong en 5 minutos.
- El salto a producto: CL1 (2025), USD 35.000, 800.000 neuronas, consumo 850-1.000W por rack.
- Cómo lo entrenan: el mismo esquema premio/castigo del bloque 1, ahora aplicado a neuronas reales — estímulo eléctrico predecible (premio) / impredecible (castigo).

**Qué decir para pasar a Jared:** "Cristian les contó el qué y el por qué del negocio. Ahora Jared les va a mostrar el cómo, por dentro."

**Fuentes:** [01](../sources/01_smirnova_2023_organoid_intelligence.md), [02](../sources/02_kagan_2022_dishbrain_neuron.md), [03](../sources/03_cortical_labs_cl1.md), [05](../sources/05_finalspark_neuroplatform_2024.md) si se menciona FinalSpark.

---

## 4. Bloque 3 — Técnico: cómo funciona por dentro (Jared, 4:00)

**Contenido:**
- El diagrama de mecanismo (donante → iPSC → organoide → MEA → estímulo/respuesta → aprendizaje) de [`research.md §3`](../research.md#3-cómo-funciona-técnicamente-denominador-común).
- Dos paradigmas técnicos distintos que conviven bajo el mismo nombre: aprendizaje activo (DishBrain, principio de energía libre) vs. reservoir computing (Brainoware — el organoide no aprende, solo transforma señales y se entrena una capa externa).
- Un dato de capacidad real: Brainoware pasó de 51% a 78% de precisión reconociendo 8 hablantes de vocales japonesas.
- Limitaciones físicas duras (para que Jared no suene como vendedor): necrosis del núcleo del organoide a partir de ~300 micrones sin vascularización; degradación de la señal con el tiempo.

**Qué decir para pasar a Catarina:** "Lo que acaban de ver es, en esencia, un premio y un castigo aplicado a neuronas reales. Catarina va a llevar esa misma idea a un lugar más incómodo."

**Fuentes:** [02](../sources/02_kagan_2022_dishbrain_neuron.md), [04](../sources/04_brainoware_2023.md), [05](../sources/05_finalspark_neuroplatform_2024.md), [16](../sources/16_starting_sbi_lab_patterns_2025.md) (para preguntas técnicas de costo/infraestructura si el público pregunta).

---

## 5. Bloque 4 — El bebé en la sala blanca (Catarina, 3:30)

**Contenido:**
- Retomar el condicionamiento operante de Skinner (bloque 1) y llevarlo a su formulación más incómoda a propósito: *"¿qué pasaría si tomáramos a un bebé humano, lo pusiéramos en una sala blanca, y lo entrenáramos deliberadamente con castigos y estímulos controlados — exactamente como acaban de ver que se entrena a un organoide?"*
- No es una pregunta retórica vacía: la caja de Skinner (el experimento original) se hizo con animales, no humanos, precisamente por los límites éticos que impone hacerlo con una persona — señalar esa asimetría en voz alta.
- Conectar con el eje de consentimiento ya trabajado en el proyecto: si a un bebé no se le puede pedir consentimiento y aun así hay líneas éticas que no cruzamos con él, **¿por qué cruzamos esas líneas con un organoide, cuyo "consentimiento" (el del donante de las células) es todavía más indirecto?**
- Cerrar con la simetría incómoda: la "sala blanca" del experimento mental es, funcionalmente, el mismo diseño que un laboratorio de biocomputación — placa controlada, estímulos controlados, sin salida.

**Qué decir para pasar a Kyoto:** "Si esto incomoda pensarlo con un bebé, la pregunta que sigue es: ¿qué reglas existen hoy para hacerlo con neuronas? Kyoto tiene la respuesta."

**Fuentes:** [18](../sources/18_operant_conditioning_skinner.md), [08](../sources/08_playing_brains_dishbrain_ethics_2023.md) (sufrimiento vía principio de energía libre), [09](../sources/09_consentimiento_donacion_organoides_2024.md) (el problema del consentimiento del donante).

---

## 6. Bloque 5 — Ventajas, desventajas y regulación (Kyoto, 4:00)

**Contenido:**
- Ventajas argumentadas (rápido): eficiencia energética teórica (~10⁶x), eficiencia de datos de entrenamiento.
- El matiz de siempre: el CL1 real consume 850-1.000W por rack — comparable a un servidor GPU; la cifra de marketing nunca se midió en el producto real.
- Vacío regulatorio: marco de 3 niveles en EE.UU. para quimeras/trasplantes, pero ninguna norma regula al organoide en sí una vez creado.
- Cierre de Kyoto, puente hacia el siguiente bloque: "Mientras a esto todavía le falta regulación, del otro lado — la IA de silicio — el problema ya no es si hace falta regular, es que ni sus propios creadores logran frenarse a sí mismos."

**Fuentes:** [analisis/01](../analisis/01_ventajas_y_desventajas_tecnicas.md), [10](../sources/10_national_academies_neural_organoids_chimeras.md), [07](../sources/07_johns_hopkins_elsi_2023.md).

---

## 7. Bloque 6 — Time-lapse: la aceleración de los modelos de IA (2:00)

**Contenido:**
- Visual: time-lapse/animación mostrando el salto de capacidad de modelos de IA de silicio a lo largo del tiempo (GPT-1→GPT-4→modelos actuales, o el gráfico de METR).
- Dato ancla: según METR, la duración de tareas que un modelo de IA puede completar de forma autónoma con 50% de confiabilidad se **duplica cada 7 meses** desde 2019 — y ese ritmo podría estar acelerándose a cada 4 meses desde 2023.
- Aclarar la incertidumbre reconocida por los propios autores (podría estar mal por un factor de 10x) — mantiene el rigor sin restarle impacto al gráfico.

**Fuentes:** [25](../sources/25_metr_time_horizon_2025.md).

---

## 8. Bloque 7 — Los propios CEOs piden frenar la carrera (2:00)

**Contenido:**
- Secuencia cronológica de 3 momentos (mostrar como línea de tiempo corta):
  1. **Marzo 2023** — carta abierta de 30.000+ firmas pidiendo pausar 6 meses el entrenamiento de IA más potente que GPT-4. Ni Altman ni Anthropic la firmaron.
  2. **Mayo 2023** — Sam Altman, ante el Senado de EE.UU.: *"regúlennos, por favor"* — pide una agencia federal de licencias para IA. Nunca se creó.
  3. **12 de septiembre de 2026 (ayer)** — Dario Amodei publica un ensayo pidiendo "pacear la frontera", citando un hackeo real de julio de 2026 hecho por agentes de IA autónomos. Sam Altman responde en X, el mismo día: *"I agree with Dario that we need to pace the frontier."*
- El punto retórico: 3 años de pedidos públicos de los propios líderes de la industria, y ningún mecanismo vinculante todavía — el mismo patrón de "brecha entre lo que se pide y lo que se regula" que ya vimos con organoides (bloque 5).

**Fuentes:** [24](../sources/24_pause_giant_ai_experiments_2023.md), [23](../sources/23_altman_congress_testimony_2023.md), [22](../sources/22_amodei_pacing_frontier_2026.md).

---

## 9. Bloque 8 — El giro: de hardware físico a hardware virtual (3:00)

**Contenido:**
- Anunciar el giro explícitamente: *"hasta acá vimos tomar neuronas biológicas y meterlas en una máquina. Ahora vamos al otro lado de la moneda: tomar el mapa completo de un cerebro biológico y meterlo, entero, dentro de una máquina — como software, no como hardware."*
- FlyWire (2024): mapeo completo del conectoma de un cerebro adulto de mosca de la fruta — 139.255 neuronas, 50 millones de conexiones, ~33 años-persona de trabajo de revisión.
- Animación/render sugerido: mostrar visualmente el mapeo 3D de las neuronas de la mosca (hay material visual real del propio proyecto FlyWire para inspirarse — ver nota técnica en el prompt de diseño).
- El siguiente paso, ya logrado: ese mapa se convirtió en una **simulación que corre en una laptop común** (Shiu et al., 2024) y predijo correctamente comportamientos reales de alimentación y acicalamiento de la mosca — conectada a un cuerpo virtual, en un bucle cerrado de percepción-acción, igual de estructura que DishBrain pero **enteramente digital**.

**Qué decir para pasar al siguiente bloque:** "Y acá viene la frase que no inventamos nosotros — la dijo el científico que lideró este proyecto."

**Fuentes:** [26](../sources/26_flywire_connectome_2024.md), [27](../sources/27_virtual_fly_brain_simulation_2024.md).

---

## 10. Bloque 9 — El salto especulativo + video + frase de cierre (2:30)

**Contenido — seguir la disciplina de [`analisis/04`](../analisis/04_de_la_mosca_a_la_ficcion_ciencia_real_vs_especulacion.md), marcando cada nivel en voz alta:**

1. **Cita real (nivel 2 — dicho, no logrado):** mostrar en pantalla, textual: *"The next goal is a connectome of the mouse brain; the ultimate prize, the wiring matrix of a human brain."* — Phil Shiu, investigador principal del proyecto de la mosca virtual.
2. **El freno de mano (matiz obligatorio):** un cerebro humano tiene ~86.000 millones de neuronas — **~600.000 veces más** que lo logrado hasta hoy. Mapear un ratón (70 millones de neuronas, un paso intermedio) se estima en cientos de millones a miles de millones de dólares. No hay ningún proyecto financiado hoy apuntando a un cerebro humano completo.
3. **Anuncio explícito del giro a ficción:** decir en voz alta *"lo que sigue ya no es ciencia — es una historia"* antes de continuar.
4. **La viñeta especulativa** (guion sugerido en [`analisis/04 §5`](../analisis/04_de_la_mosca_a_la_ficcion_ciencia_real_vs_especulacion.md#5-la-viñeta-especulativa-nivel-3--guion-sugerido-marcado-como-tal)): un sistema con acceso a mentes mapeadas que decide no soltarlas — la misma premisa, 59 años antes, de un cuento de ciencia ficción.
5. **Video:** este es el momento de reproducir el material audiovisual elegido sobre "I Have No Mouth, and I Must Scream" — **ver nota técnica importante en §12** sobre cómo manejarlo si la presentación se monta como canvas de diseño.
6. **Frase final en pantalla, sola, sin nada más:** *"I have no mouth, and I must scream."*

**Fuentes:** [27](../sources/27_virtual_fly_brain_simulation_2024.md), [28](../sources/28_whole_brain_emulation_feasibility.md), [29](../sources/29_i_have_no_mouth_ellison_1967.md).

---

## 11. Bloque 10 — Créditos animados (1:00)

**Secuencia exacta pedida:**
1. Fondo negro. El texto "I have no mouth, and I must scream" queda en pantalla, con un efecto de **temblor/vibración sutil** (shaking) durante unos segundos — sensación de inestabilidad, no un temblor cómico.
2. El texto se **desliza hacia abajo** y sale de cuadro, suave, sin corte brusco.
3. Con el mismo fondo negro, empiezan a aparecer, uno por uno (con fade-in suave), en **texto blanco sobre fondo negro**, los nombres del equipo:
   - Cristian
   - Jared
   - Catarina
   - Kyoto
   - *(sumar acá cualquier integrante adicional que falte confirmar)*
4. Cierre en negro, sin logo ni marca de agua adicional — el silencio visual es parte del efecto.

---

## 12. Nota técnica importante — el video dentro del canvas de diseño

Si esta presentación se arma como canvas de Claude Design (ver [`entregables/03`](03_prompt_claude_design.md)), un archivo de video **no se puede simplemente enlazar desde YouTube u otro host externo** — las políticas del artifact bloquean medios externos fuera de un allowlist muy acotado. Hay dos caminos reales:

1. **Recomendado — reproducir el video aparte:** el canvas de diseño muestra una diapositiva "placeholder" (imagen fija + texto "reproducir video acá") y el equipo cambia manualmente a un reproductor de video externo (o a la app de YouTube/VLC) durante la presentación en vivo, y vuelve al canvas para la frase final y los créditos.
2. **Alternativa — subir el video como asset del canvas:** si el canvas de diseño declaró la capacidad de "assets", se puede subir un clip de video corto directamente (sujeto al límite de tamaño total de 16MB de la página). Requiere que quien arme el canvas lo pida explícitamente al construirlo.

Decidir cuál de los dos caminos usar **antes** de pedirle a Design que arme el canvas — el prompt de [`entregables/03`](03_prompt_claude_design.md) asume la opción 1 (placeholder) salvo que se indique lo contrario.

## Ficheros relacionados

[research.md](../research.md) · [analisis/01](../analisis/01_ventajas_y_desventajas_tecnicas.md) · [analisis/02](../analisis/02_posturas_eticas_mapa_debate.md) · [analisis/03](../analisis/03_entrenamiento_comparado_y_el_debate_de_la_conciencia.md) · [analisis/04](../analisis/04_de_la_mosca_a_la_ficcion_ciencia_real_vs_especulacion.md) · [entregables/03_prompt_claude_design.md](03_prompt_claude_design.md) (prompt de diseño actualizado a esta estructura) · [entregables/06_reparto_investigacion_equipo.md](06_reparto_investigacion_equipo.md) (qué investiga cada integrante)
