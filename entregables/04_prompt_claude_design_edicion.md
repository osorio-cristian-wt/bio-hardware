# Prompt para Claude Design — edición del canvas (v2: eje de entrenamiento y consciencia)

> Este prompt **edita** el canvas construido a partir de [`03_prompt_claude_design.md`](03_prompt_claude_design.md) (11 diapositivas, eje "ventajas/desventajas técnicas"). La presentación cambió de eje: ahora el centro es la comparación de cómo se entrena una IA, cómo aprendemos nosotros y cómo "aprende" un organoide, para abrir la pregunta de la consciencia (ver [`02_guia_presentacion_15min.md`](02_guia_presentacion_15min.md) v2). El prompt es autocontenido — funciona tanto para editar el canvas ya publicado como para generarlo de cero si todavía no existe.

---

## Prompt

```
Estoy editando un canvas de presentación de 15 minutos que ya generaste antes
a partir de un prompt anterior (11 diapositivas, formato 16:9, tema
"Neuronas humanas como hardware de inteligencia artificial"). SI ese canvas
ya existe: mantené el lenguaje visual ya establecido (paleta, tipografía,
tratamiento de los "blobs" orgánicos para representar organoides, numeración
de diapositivas) y aplicá los cambios de abajo. SI es la primera vez que
genera este canvas: construilo directo con la estructura de 12 diapositivas
completa que sigue, usando la misma guía de estilo del prompt original
(editorial/científico-serio, nada de cerebros brillantes ni clip-art de
ciencia ficción, paleta neutra + un acento).

QUÉ CAMBIÓ: la charla ya no gira en torno a "ventajas vs. desventajas
técnicas" — ahora gira en torno a una comparación pedagógica de tres formas
de aprender (una IA de silicio, un humano, un organoide) para abrir la
pregunta filosófica de qué es la consciencia, SIN responderla. El tono pasa
de "informativo" a "informativo + deliberadamente abierto" en el tramo
central — la presentación debe dejar al público con una pregunta, no con
una conclusión.

ESTRUCTURA NUEVA: 12 artboards (antes 11). Las diapositivas 1 y 2 se
mantienen casi iguales (ajustar solo el copy del título según se indica);
de la 3 en adelante la secuencia es enteramente nueva.

--- DIAPOSITIVA 1 (ajustar, no rehacer desde cero) ---
Título nuevo: "¿Aprender es lo mismo que ser consciente?"
Subtítulo (igual que antes): "Neuronas humanas como hardware de
inteligencia artificial"
Mantener el mismo tratamiento visual de blobs orgánicos sobre grilla de
circuito ya usado.

--- DIAPOSITIVA 2 (mantener, ajuste menor) ---
Sin cambios de contenido: "no es un mini-cerebro, es un cultivo de
neuronas conectado a electrodos" + las 3 tarjetas de nombres (Organoid
Intelligence / Synthetic Biological Intelligence / wetware computing).

--- DIAPOSITIVA 3 (NUEVA) ---
Título: "Cómo aprende una IA: premio y castigo"
Diagrama circular/cíclico de 4 pasos con iconos simples: Observar → Actuar
→ Recibir señal de recompensa (+/-) → Ajustar → (vuelve a Observar).
Nota al pie: "la recompensa es un número que un ingeniero define de
antemano."

--- DIAPOSITIVA 4 (NUEVA) ---
Título: "Cómo aprendemos nosotros: el bebé y el caramelo"
Contenido: mismo diagrama cíclico que la diapositiva 3 pero relabeled con
términos de condicionamiento operante: Conducta → Consecuencia (refuerzo o
castigo) → Cambio de probabilidad de repetirla → (vuelve a Conducta).
Ilustración simple y no infantilizada de un caramelo como ícono de
"refuerzo positivo" — evitar clip-art tierno, mantener el mismo lenguaje
geométrico/abstracto del resto de la deck.
Nota al pie: "B.F. Skinner — la conducta se moldea por sus consecuencias."

--- DIAPOSITIVA 5 (NUEVA) ---
Título: "Cómo 'aprende' un organoide: mismo esquema, otra sustancia"
Mismo diagrama cíclico otra vez, ahora relabeled: Acción del organoide →
Estímulo predecible (premio) / impredecible (castigo) → Reorganización de
conexiones → (vuelve a Acción).
IMPORTANTE: usar el MISMO diagrama visual (misma forma, mismo layout) que
las diapositivas 3 y 4, solo cambiando las etiquetas — la repetición visual
exacta es intencional, refuerza el argumento de que es la misma estructura.

--- DIAPOSITIVA 6 (NUEVA — diapositiva de pausa) ---
Título: "¿Son la misma cosa?"
Contenido visual: los tres diagramas cíclicos de las diapositivas 3, 4 y 5,
ahora lado a lado, en miniatura, idénticos en forma — sin texto adicional,
sin bullets. Mucho espacio en blanco. Esta diapositiva tiene que sentirse
deliberadamente vacía/pausada comparada con el resto — es el momento de
silencio de la charla, no agregues contenido de relleno.

--- DIAPOSITIVA 7 (NUEVA — tratamiento visual distinto: NEUTRAL, sin
jerarquía de color) ---
Título: "El problema difícil de la consciencia"
Subtítulo pequeño: explicar en una línea la distinción entre "problemas
fáciles" (qué hace un sistema) y "el problema difícil" (por qué eso se
siente desde adentro).
Contenido principal: TRES COLUMNAS DEL MISMO ANCHO, MISMO PESO VISUAL, SIN
NINGUNA DESTACADA (nada de "la opción del medio en grande" ni un color de
acento en una sola columna — las tres deben verse deliberadamente
equivalentes):
- Columna 1: "Fisicalismo / funcionalismo" — la consciencia es 100%
  física; en principio replicable en cualquier sustrato correcto.
- Columna 2: "Dualismo" — la consciencia es de otra naturaleza, no
  reducible a lo físico (aquí entran muchas tradiciones religiosas y
  filosóficas — la idea del alma).
- Columna 3: "Panpsiquismo" — la experiencia es una propiedad fundamental
  de la materia, presente en distinto grado en todo.
Esta es la diapositiva más importante para acertar visualmente: el diseño
debe comunicar neutralidad absoluta entre las tres posturas.

--- DIAPOSITIVA 8 (NUEVA) ---
Título: "¿Alcanza el premio y el castigo para producir consciencia?"
Contenido: dos tarjetas enfrentadas (formato "versus" sutil, no
confrontativo):
- Izquierda: "Reward is Enough" (DeepMind, 2021) — maximizar una señal de
  recompensa alcanzaría para producir toda capacidad asociada a la
  inteligencia.
- Derecha: "Scalar reward is not enough" (respuesta académica, 2022) — una
  recompensa de un solo número no alcanza para explicar la complejidad de
  la inteligencia biológica ni artificial.
Nota al pie: "ninguna de las dos partes afirma haber resuelto la pregunta
de la consciencia."

--- DIAPOSITIVA 9 (equivalente a la antigua diapositiva 4, condensada) ---
Título: "De laboratorio a producto en 4 años"
Timeline horizontal con 5 hitos (2019 Cortical Labs · 2022 DishBrain ·
2023 paper fundacional + Brainoware · 2025 CL1 comercial USD 35.000 ·
2025-26 advertencias internas del propio campo).

--- DIAPOSITIVA 10 (equivalente a las antiguas 6+7, fusionadas y
condensadas) ---
Título: "La promesa y su matiz"
Dos columnas simples: "Se promete" (eficiencia ~10⁶x, cita el cerebro
completo vs. supercomputadora) vs. "En el producto real" (CL1: 850-1.000W
por rack, comparable a un servidor GPU).

--- DIAPOSITIVA 11 (equivalente a la antigua 9, condensada) ---
Título: "¿Está regulado?"
Semáforo de 3 niveles (verde/amarillo/rojo) + texto destacado: "ninguna
norma regula al organoide EN SÍ una vez creado."

--- DIAPOSITIVA 12 (reemplaza a las antiguas 10 y 11, cierre único) ---
Título: "La pregunta que abre el debate"
Cita centrada, tipografía grande, dos oraciones:
"Si una IA de silicio, un bebé humano y un organoide aprenden con el mismo
esquema de premio y castigo — ¿qué distingue a uno de ser 'solo código' y
a otro de ser 'alguien'?"
Debajo, más chico: la moción del debate ("¿Debería el desarrollo de
'organoid intelligence' continuar sin restricciones adicionales a las ya
existentes?")

INSTRUCCIONES ADICIONALES:
- Los tres diagramas cíclicos (diapositivas 3, 4, 5) tienen que ser
  visualmente IDÉNTICOS en forma — es la pieza central del argumento de
  toda la charla. Si el layout de alguno de los tres queda distinto al
  resto, corregilo antes que cualquier otra cosa.
- La diapositiva 7 (las tres posturas filosóficas) no debe usar el color
  de acento de ninguna otra diapositiva para destacar una opción sobre
  las otras — usar un tratamiento neutro (ej. las tres en el mismo gris o
  el mismo azul base, sin acento).
- Mantené la numeración discreta de diapositiva (ahora "X/12" en vez de
  "X/11") en todos los artboards.
- Si el canvas anterior tenía elementos de las diapositivas viejas 6, 7,
  10 y 11 (jugadores comerciales, ventajas argumentadas por separado, el
  cierre viejo con moción sola) que ya no tienen equivalente uno-a-uno,
  fusionalos o eliminalos según el mapeo de arriba — no dejes artboards
  huérfanos del prompt anterior.
```

## Notas de uso

- Si el canvas de la v1 (prompt 03) todavía no se publicó, este prompt también sirve como generación desde cero — ya trae contenido completo para las 12 diapositivas, no depende de que exista nada previo.
- El texto para decir en voz alta en cada diapositiva sigue viviendo en [`02_guia_presentacion_15min.md`](02_guia_presentacion_15min.md) — no se repite acá a propósito, para no duplicar mantenimiento entre los dos archivos.
- Si después de esta edición hace falta un ajuste puntual, referenciar el artboard por su número nuevo (ej. "la diapositiva 6, la de pausa, necesita aún más espacio en blanco").
