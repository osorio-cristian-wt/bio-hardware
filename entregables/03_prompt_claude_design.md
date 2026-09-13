# Prompt para Claude Design — "paseo rápido" (~15 min), con fuentes en formato APA

> **Reemplaza la versión anterior de este archivo** (la misma estructura de 7 beats + video, pero sin fuentes citadas — quedó en el historial de git). Esta versión agrega: los pasos de cultivo del organoide en el beat B, placeholders de imágenes reales (chip físico, visualización del conectoma, laptop) en los beats B y F, los tweets citados con permalink en el beat E, la comparación GPT-3.5 → GPT-6 Astra, y una lista de referencias en formato APA al final del propio prompt — todo trazable a `sources/` por si hace falta verificar algo.

---

## Antes de pegar el prompt

- El video sigue sin poder reproducirse desde un host externo dentro del canvas — este prompt asume **placeholder** (ver [`05_guia_presentacion_grupal.md` §12](05_guia_presentacion_grupal.md#12-nota-técnica-importante--el-video-dentro-del-canvas-de-diseño)).
- Los tres placeholders de imagen real (chip físico, conectoma, laptop) **no traen la imagen en sí** — traen el lugar exacto donde buscarla (documentado en `sources/`) para no inventar una imagen genérica que después haya que reemplazar. Si van a subir esas imágenes como asset del canvas, avisen antes de generarlo.

---

## Prompt

```
Necesito un canvas de diseño para un "paseo rápido" de ~15 minutos en total:
~10 minutos de contenido en 7 beats cortos, seguidos de un placeholder de
video de 5 minutos, y un cierre animado. Formato 16:9.

TEMA: "Neuronas humanas como hardware de inteligencia artificial". Recorrido
veloz, NO una charla exhaustiva — una sola idea fuerte por artboard. Arranca
como divulgación científica rigurosa y termina como un cierre cinematográfico
inspirado en "I Have No Mouth, and I Must Scream" (Ellison, 1967) — marcado
EXPLÍCITAMENTE como ficción, nunca como pronóstico real.

CADA AFIRMACIÓN DE DATO LLEVA SU FUENTE EN PANTALLA: un pie de página chico
con cita corta (autor/organización, año) en cada beat que tenga un dato — la
lista completa en formato APA está al final de este prompt, en la sección
REFERENCIAS. Usalas tal cual están ahí, no resumas ni inventes una cita
distinta.

ARCO DE ESTILO VISUAL: paleta editorial/científica y luminosa en los beats
A-D (blancos, grises, azul/teal de acento, estilo Nature/Wired) que se
enfría progresivamente en E-F hasta terminar 100% en negro con tipografía
blanca desde el beat G en adelante (video y créditos).

DISCIPLINA DE HONESTIDAD VISUAL: en los beats E, F y G, cada afirmación
fuerte lleva una badge chica de certeza — "DEMOSTRADO" (azul/verde apagado),
"DECLARADO, NO LOGRADO" (ámbar apagado), o "FICCIÓN" (tono oscuro, el mismo
del cierre).

AUDIENCIA: estudiantes universitarios sin conocimiento previo.

PLACEHOLDERS DE IMAGEN REAL (usar los 3, no reemplazar por ilustraciones
genéricas): cada uno lleva un recuadro con borde punteado, un ícono simple
de imagen, y un texto chico abajo indicando DÓNDE conseguir la imagen real
antes de la presentación final — están marcados en los beats B y F más
abajo con la etiqueta "[PLACEHOLDER DE IMAGEN REAL]".

---

ESTRUCTURA: 7 beats de contenido + 1 placeholder de video + 1 cierre
animado. Un artboard por beat salvo que se indique lo contrario — cada uno
tiene que poder pasarse cada 60-90 segundos reales de exposición.

--- BEAT A (1:30) — Apertura relámpago ---
Título: "¿Y si la computadora que entrena tu IA... estuviera viva?"
Diagrama cíclico de 4 pasos (Observar → Actuar → Recompensa +/- → Ajustar)
para explicar aprendizaje por refuerzo. Nota al pie: "así aprendemos
nosotros también — más adelante volvemos a esto." Blobs orgánicos simples
sobre grilla de circuito, nada literal. Sin cita de dato específico en este
beat (es un encuadre conceptual, no una afirmación cuantitativa).

--- BEAT B (1:30) — La startup: cómo se cultiva y cómo entrena ---
DOS partes en este beat (podés usar 1 o 2 artboards, el que entre mejor):

Parte 1 — LOS PASOS DEL CULTIVO (secuencia horizontal de 5 pasos con
iconos simples, es la parte nueva pedida):
1. Donación: biopsia de piel o muestra de sangre de un donante voluntario.
2. Reprogramación: las células del donante se convierten en células madre
   pluripotentes inducidas (iPSC).
3. Diferenciación: las iPSC se dirigen hacia precursores neuronales.
4. Auto-organización: las células se cultivan en suspensión 3D y se
   autoorganizan en un organoide cerebral (10+ semanas de cultivo).
5. Integración: el organoide se monta sobre un array de microelectrodos
   (MEA) que lo estimula y registra su actividad — acá empieza el
   entrenamiento por premio/castigo del beat A.
Cita al pie: Smirnova et al. (2023); Kitchen et al. (2022).

Parte 2 — LA STARTUP (fusionar en el mismo artboard o en el siguiente):
DishBrain (2022, 800.000 neuronas aprenden Pong en 5 min) → CL1 (2025, USD
35.000, 850-1.000W por rack). Cita al pie: Kitchen et al. (2022);
Wikipedia contributors (2026).

[PLACEHOLDER DE IMAGEN REAL] — un recuadro de borde punteado en este beat,
texto: "Insertar foto real del chip/circuito físico (CL1 o el montaje de
DishBrain) — buscar en la cobertura de DataCenterDynamics o BioPharmaTrend
sobre el lanzamiento del CL1 (ver referencia Datacenter Dynamics, 2025, al
final de este prompt). No usar una ilustración genérica de circuito."

--- BEAT C (1:00) — El bebé en la sala blanca ---
Sin cambios respecto a la versión anterior: pregunta grande y centrada,
mucho espacio en blanco: "¿Qué pasaría si entrenáramos a un bebé humano con
los mismos castigos y estímulos que acaban de ver aplicados a un
organoide?" Tono deliberadamente más incómodo, empezar a insinuar
temperatura fría de color. Sin cita de dato específico (es una pregunta
retórica/ética, no una afirmación cuantitativa).

--- BEAT D (1:30) — Ventajas, el matiz y la regulación ---
3 elementos en columnas: "Se promete" (eficiencia ~10⁶x, cita: Smirnova et
al., 2023) · "En el producto real" (CL1: 850-1.000W, cita: Wikipedia
contributors, 2026) · semáforo de 3 niveles con "ninguna norma regula al
organoide EN SÍ una vez creado" (cita: National Academies of Sciences,
Engineering, and Medicine — ver referencia completa al final).

--- BEAT E (1:30) — La carrera que nadie frena ---
Empezar a enfriar la paleta. DOS partes:

Parte 1 — El salto de capacidad (arriba o a la izquierda del artboard):
"GPT-3.5 (2022, ~175.000 millones de parámetros) → GPT-6 Astra (4 sept.
2026, entrenado con más de 100.000 GPUs — el mayor esfuerzo de cómputo de
OpenAI hasta la fecha)." Cita al pie: OpenAI (2026); Wikipedia contributors
(2026b). Badge "DEMOSTRADO".
Sumar el dato de METR en una línea chica debajo: "la duración de tareas que
una IA completa de forma autónoma se duplica cada 7 meses desde 2019" (cita:
METR, 2025) — con nota de que los propios autores reconocen hasta 10x de
margen de error.

Parte 2 — Los tweets citados (abajo o a la derecha, en formato "captura de
tweet" simple — burbuja con el ícono de X, el nombre de usuario, y el texto
entre comillas, NO hace falta imitar el diseño real de X, alcanza con que
se lea claramente como una cita textual de una publicación):
> @DarioAmodei (12 sept. 2026): "We Must Pace the Frontier: I've written a
  new essay on why the AI industry should slow down..."
> @sama (12 sept. 2026): "I agree with Dario that we need to pace the
  frontier."
> @elonmusk (12 sept. 2026): "Dario is right."
Cita al pie de esta parte: Amodei (2026a, 2026b); Altman (2026); Musk
(2026) — ver referencias completas al final.

--- BEAT F (1:30) — El giro: la mosca mapeada y simulada ---
Anuncio explícito: "Ahora vamos al otro lado de la moneda: de neuronas
biológicas en una máquina, a un cerebro biológico entero DENTRO de una
máquina." FlyWire (2024): 139.255 neuronas, 50 millones de conexiones,
conectoma completo de un cerebro adulto de mosca — corriendo después como
simulación en una laptop, prediciendo comportamiento real. Cita al pie:
Dorkenwald et al. (2024); Shiu et al. (2024).

[PLACEHOLDER DE IMAGEN REAL #1] — recuadro de borde punteado: "Insertar
captura real de la visualización 3D del conectoma — sacarla del explorador
Codex (codex.flywire.ai) o del reportaje inmersivo de Nature (ver
referencia FlyWire/Nature al final). No generar un render genérico de
'red neuronal' — usar la visualización real del propio proyecto."

[PLACEHOLDER DE IMAGEN REAL #2] — recuadro de borde punteado, en el mismo
artboard o en uno siguiente: "Insertar foto real de la simulación corriendo
en una laptop — buscar en la cobertura de Berkeley News sobre el paper de
Shiu et al. (ver referencia al final). Es la imagen que sostiene la frase
'corre en una laptop común', tiene que ser una laptop real, no una gráfica
abstracta de código."

Paleta ya notablemente fría en este beat.

--- BEAT G (1:00) — El salto especulativo + "esto ya es ficción" ---
Un solo artboard, casi negro: cita grande con badge "DECLARADO, NO
LOGRADO": "The next goal is a connectome of the mouse brain; the ultimate
prize, the wiring matrix of a human brain." — Phil Shiu (cita: Shiu et al.,
2024, vía cobertura de Berkeley News). Debajo, con badge "DEMOSTRADO":
"~600.000 veces más neuronas que lo logrado hasta hoy — ningún proyecto
financiado apunta ahí" (cita: e11 Bio roadmap, ver referencia al final). Y
como última línea, ya en texto grande sobre negro puro, badge "FICCIÓN":
"Lo que sigue ya no es ciencia. Es una historia."

--- VIDEO (5:00) — placeholder ---
Artboard aparte, fondo 100% negro, ícono de play centrado, texto chico
abajo: "reproducir video aquí — I Have No Mouth, and I Must Scream (cita:
Ellison, 1967, ver referencia al final)."

--- CIERRE ANIMADO (~0:30-1:00) ---
Igual que antes: la frase "I have no mouth, and I must scream." tiembla
sutilmente unos segundos, se desliza hacia abajo y sale de cuadro, y sobre
fondo negro aparecen uno por uno, con fade-in escalonado, en blanco:
Cristian · Jared · Catarina · Kyoto. Termina en negro sólido.

---

INSTRUCCIONES ADICIONALES:
- Nunca fotos de stock de cerebros ni ilustraciones médicas realistas para
  las partes ilustradas — SALVO los 3 placeholders de imagen real pedidos
  arriba, que son intencionalmente reales, no estilizados.
- Los diagramas cíclicos de los beats A y B (parte del entrenamiento) deben
  ser visualmente IDÉNTICOS en forma.
- No omitir ningún pie de cita en los beats B, D, E, F y G — son los que
  tienen datos verificables; A y C son conceptuales/retóricos y no llevan
  cita.
- Numerar los artboards de forma discreta y continua.

---

REFERENCIAS (formato APA — usar estas citas tal cual, no reformular):

Altman, S. [@sama]. (2026, September 12). I agree with Dario that we need
to pace the frontier... [Post]. X. https://x.com/sama/status/2098811563415150910

Amodei, D. (2026a, September 12). We must pace the frontier.
https://darioamodei.com/post/we-must-pace-the-frontier

Amodei, D. [@DarioAmodei]. (2026b, September 12). We Must Pace the
Frontier: I've written a new essay... [Post]. X.
https://x.com/DarioAmodei/status/2098773920774074715

Dorkenwald, S., Matsliah, A., Sterling, A. R., Schlegel, P., Yu, S. C.,
McKellar, C. E., Lin, A., Costa, M., Eichler, K., Yin, Y., Silversmith, W.,
Schneider-Mizell, C., Jordan, C. S., Brittain, D., Halageri, A., Kuehner,
K., Ogedengbe, O., Morey, R., Gager, J., … Murthy, M. (2024). Neuronal
wiring diagram of an adult brain. Nature, 634(8032), 124–138.
https://doi.org/10.1038/s41586-024-07558-y

Datacenter Dynamics. (2025). Australian startup Cortical Labs unveils
"world's first" commercial biological computer.
https://www.datacenterdynamics.com/en/news/australian-startup-cortical-labs-unveils-worlds-first-commercial-biological-computer/

Ellison, H. (1967). I have no mouth, and I must scream. IF: Worlds of
Science Fiction.

e11 Bio. (n.d.). A roadmap to scale connectomics to entire mammalian
brains. Retrieved September 2026, from https://www.e11.bio/blog/roadmap

Kitchen, A. C., Kagan, B. J., Tran, N. T., Habibollahi, F., Khajehnejad,
M., Parker, B. J., Bhat, A., Rollo, B., Razi, A., & Friston, K. J. (2022).
In vitro neurons learn and exhibit sentience when embodied in a simulated
game-world. Neuron, 110(23), 3952–3969.e8.
https://doi.org/10.1016/j.neuron.2022.09.001

METR. (2025, March 19). Measuring AI ability to complete long software
tasks. https://metr.org/blog/2025-03-19-measuring-ai-ability-to-complete-long-tasks/

Musk, E. [@elonmusk]. (2026, September 12). Dario is right [Post]. X.
https://x.com/elonmusk/status/2098789109980332057

National Academies of Sciences, Engineering, and Medicine. (2021). The
emerging field of human neural organoids, transplants, and chimeras:
Science, ethics, and governance. The National Academies Press.
https://www.nationalacademies.org/read/26078

OpenAI. (2026). GPT-6 Astra: A new generation of intelligence.
https://openai.com/index/gpt-6-astra/

Shiu, P. K., Sterne, G. R., Spiller, N., Franconville, R., Sandoval, A.,
Zhou, J., Simha, N., Kang, C. H., Yu, S., Kim, J. S., Dorkenwald, S.,
Matsliah, A., Schlegel, P., Yu, S., McKellar, C. E., Sterling, A., Costa,
M., Eichler, K., Bates, A. S., … Bidaye, S. S. (2024). A Drosophila
computational brain model reveals sensorimotor processing. Nature,
634(8032), 210–219. https://doi.org/10.1038/s41586-024-07763-9

Smirnova, L., Caffo, B. S., Gracias, D. H., Huang, Q., Morales Pantoja,
I. E., Tang, B., Zack, D. J., Berlinicke, C. A., Boyd, J. L., Harris, T. D.,
Johnson, E. C., Kagan, B. J., Kahn, J., Muotri, A. R., Paulhamus, B. L.,
Schwamborn, J. C., Plotkin, J. B., Szalay, A. S., Vogelstein, J. T.,
Worley, P. F., & Hartung, T. (2023). Organoid intelligence (OI): The new
frontier in biocomputing and intelligence-in-a-dish. Frontiers in Science,
1, Article 1017235. https://doi.org/10.3389/fsci.2023.1017235

Wikipedia contributors. (2026a). Cortical Labs. Wikipedia.
https://en.wikipedia.org/wiki/Cortical_Labs

Wikipedia contributors. (2026b). GPT-6 Astra. Wikipedia.
https://en.wikipedia.org/wiki/GPT-6_Astra
```

## Notas de uso

- Todas las referencias de arriba están además documentadas, con más contexto y matices, en `sources/` — número de archivo entre paréntesis: Altman/Musk/Amodei ([22](../sources/22_amodei_pacing_frontier_2026.md)), Dorkenwald/Schlegel ([26](../sources/26_flywire_connectome_2024.md)), Datacenter Dynamics/Wikipedia CL1 ([03](../sources/03_cortical_labs_cl1.md)), Ellison ([29](../sources/29_i_have_no_mouth_ellison_1967.md)), e11 Bio ([28](../sources/28_whole_brain_emulation_feasibility.md)), Kitchen et al. ([02](../sources/02_kagan_2022_dishbrain_neuron.md)), METR ([25](../sources/25_metr_time_horizon_2025.md)), National Academies ([10](../sources/10_national_academies_neural_organoids_chimeras.md)), OpenAI/GPT-6 Astra ([30](../sources/30_gpt_model_evolution_2022_2026.md)), Shiu et al. ([27](../sources/27_virtual_fly_brain_simulation_2024.md)), Smirnova et al. ([01](../sources/01_smirnova_2023_organoid_intelligence.md)).
- El guion completo de qué dice cada orador sigue en [`05_guia_presentacion_grupal.md` §0.bis](05_guia_presentacion_grupal.md#0bis--versión-condensada-paseo-rápido-15-min-total).
- **Nota de honestidad académica:** dos referencias (Smirnova et al., 2023 y Dorkenwald et al., 2024) tienen listas de autores muy largas — se completaron con búsqueda pero no se verificaron letra por letra contra el PDF original. Si esto va a un entregable formal con nota, revisar el orden exacto de autores contra la fuente antes de entregar.
