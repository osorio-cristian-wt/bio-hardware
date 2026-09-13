# Prompt para Claude Design — "paseo rápido" (~15 min: 10 min de contenido + 5 min de video)

> **Reemplaza la versión anterior de este archivo** (era la de ~30 minutos con 10 bloques largos — quedó en el historial de git). Esta es la versión condensada pedida: un recorrido rápido de 7 beats cortos, video de 5 minutos, y el mismo cierre. Autocontenido, trae el contenido de [`05_guia_presentacion_grupal.md` §0.bis](05_guia_presentacion_grupal.md#0bis--versión-condensada-paseo-rápido-15-min-total).

---

## Antes de pegar el prompt — la misma decisión de siempre

El video no se puede reproducir desde un host externo dentro del canvas por política de contenido. Este prompt asume **placeholder** (el equipo cambia a un reproductor externo en vivo, ver [`05` §12](05_guia_presentacion_grupal.md#12-nota-técnica-importante--el-video-dentro-del-canvas-de-diseño)). Si en cambio lo quieren embebido como asset, avisen antes de generar el canvas.

---

## Prompt

```
Necesito un canvas de diseño para un "paseo rápido" de ~15 minutos en total:
~10 minutos de contenido en 7 beats cortos y muy directos, seguidos de un
placeholder de video de 5 minutos, y un cierre animado. Formato 16:9.

TEMA: "Neuronas humanas como hardware de inteligencia artificial". Es un
recorrido veloz, NO una charla exhaustiva — cada beat tiene que leerse en
segundos, con una sola idea fuerte por artboard. Menos texto que en una
presentación normal, no más. El arco narrativo completo: arranca como
divulgación científica rigurosa y termina como un cierre cinematográfico
inspirado en "I Have No Mouth, and I Must Scream" (Harlan Ellison, 1967) —
marcado EXPLÍCITAMENTE como ficción, nunca como pronóstico real.

ARCO DE ESTILO VISUAL (lo más importante del prompt): la paleta pasa de
editorial/científica y luminosa (beats A-D: blancos, grises, un azul/teal
de acento, estilo Nature/Wired) a progresivamente más fría y oscura (beats
E-F) hasta terminar 100% en negro con tipografía blanca (beat G en
adelante, video y créditos). Con solo 7 beats de contenido, la transición
de paleta tiene que sentirse más comprimida que en una versión larga —
arrancá a enfriar el tono ya desde el beat E, no esperes al F.

DISCIPLINA DE HONESTIDAD VISUAL: en los beats E, F y G, cada afirmación
fuerte lleva una badge chica indicando su nivel de certeza:
- "DEMOSTRADO" (azul/verde apagado) — publicado y logrado.
- "DECLARADO, NO LOGRADO" (ámbar apagado) — dicho en público por alguien
  real, sin haberse cumplido.
- "FICCIÓN" (tono oscuro, igual al del cierre) — especulación explícita.
No es decorativo: es lo que sostiene la seriedad del recorrido incluso
cuando el contenido se vuelve especulativo hacia el final.

CITAS AL PIE: cada beat con un dato (no los puramente de transición) lleva
una cita corta (autor/organización + año) en el pie — chica, pero visible.

AUDIENCIA: estudiantes universitarios sin conocimiento previo.

---

ESTRUCTURA: 7 beats de contenido + 1 placeholder de video + 1 cierre
animado. Dale a cada beat UN SOLO artboard salvo que se indique lo
contrario — el objetivo es que se pueda pasar de uno a otro cada 60-90
segundos reales de exposición.

--- BEAT A (1:30) — Apertura relámpago ---
Título: "¿Y si la computadora que entrena tu IA... estuviera viva?"
Diagrama cíclico simple de 4 pasos (Observar → Actuar → Recompensa +/- →
Ajustar) para explicar aprendizaje por refuerzo en una sola imagen. Nota
al pie chica: "así aprendemos nosotros también — más adelante volvemos a
esto." Blobs orgánicos simples sobre grilla de circuito, nada literal.

--- BEAT B (1:30) — La startup + cómo entrena neuronas reales ---
Un solo artboard fusionando: DishBrain (2022, 800.000 neuronas aprenden
Pong en 5 min) → CL1 (2025, USD 35.000, 850-1.000W por rack). El mismo
diagrama de circuito cerrado del beat A, ahora relabeled con "estímulo
predecible / impredecible" en vez de "recompensa +/-" — la repetición
visual exacta es intencional.

--- BEAT C (1:00) — El bebé en la sala blanca ---
Tono deliberadamente más incómodo, sin llegar todavía al negro total —
podés anticipar acá un poco de temperatura fría de color.
Pregunta grande y centrada, mucho espacio en blanco: "¿Qué pasaría si
entrenáramos a un bebé humano con los mismos castigos y estímulos que
acaban de ver aplicados a un organoide?"

--- BEAT D (1:30) — Ventajas, el matiz y la regulación ---
Volver al tono neutro. Un artboard con 3 elementos rápidos en columnas:
"Se promete" (eficiencia ~10⁶x) · "En el producto real" (CL1: 850-1.000W,
comparable a un servidor GPU) · semáforo de 3 niveles con el texto
"ninguna norma regula al organoide EN SÍ una vez creado."

--- BEAT E (1:30) — La carrera que nadie frena ---
Empezar a enfriar la paleta acá. Un dato de aceleración (METR: "la
capacidad de la IA se duplica cada 7 meses desde 2019") + la cita más
fuerte y más reciente: "I agree with Dario that we need to pace the
frontier." — Sam Altman, respondiendo el mismo día al ensayo de Dario
Amodei (Anthropic) pidiendo "pacear la frontera" (12 sept. 2026). Badge
"DEMOSTRADO" en el dato de METR (con nota chica: los propios autores
reconocen hasta 10x de margen de error).

--- BEAT F (1:30) — El giro: la mosca mapeada y simulada ---
Anuncio explícito: "Ahora vamos al otro lado de la moneda: de neuronas
biológicas en una máquina, a un cerebro biológico entero DENTRO de una
máquina." FlyWire (2024): 139.255 neuronas, 50 millones de conexiones,
conectoma completo de un cerebro adulto de mosca — corriendo después como
simulación en una laptop, prediciendo comportamiento real (Shiu et al.,
2024). Si es posible, una animación simple de nodos/líneas rotando
lentamente (CSS/canvas, geometría abstracta, no una imagen médica real)
sugiriendo el mapeo neuronal. Paleta ya notablemente fría acá.

--- BEAT G (1:00) — El salto especulativo + "esto ya es ficción" ---
Un solo artboard, casi negro ya: cita grande con badge "DECLARADO, NO
LOGRADO": "The next goal is a connectome of the mouse brain; the ultimate
prize, the wiring matrix of a human brain." — Phil Shiu. Debajo, más
chico, con badge "DEMOSTRADO": "~600.000 veces más neuronas que lo
logrado hasta hoy — ningún proyecto financiado apunta ahí." Y como última
línea de este mismo artboard, ya en texto grande sobre negro puro, badge
"FICCIÓN": "Lo que sigue ya no es ciencia. Es una historia."

--- VIDEO (5:00) — placeholder ---
Artboard aparte, fondo 100% negro, ícono de play simple centrado, texto
chico abajo: "reproducir video aquí" — señal para el orador, no reproduce
nada dentro del canvas.

--- CIERRE ANIMADO (~0:30-1:00) ---
Artboard final, fondo negro. Secuencia en CSS (keyframes, sin librerías
externas):
1. Aparece centrada la frase "I have no mouth, and I must scream." con un
   efecto de vibración/temblor sutil (shake de 1-3px en X, rápido, baja
   amplitud — inestable, no cómico) durante unos segundos.
2. El texto se desliza hacia abajo (translateY) y sale de cuadro,
   transición suave (ease-out, ~1-1.5s).
3. Sobre el mismo fondo negro, aparecen uno por uno con fade-in
   escalonado (~0.4-0.6s de delay entre cada uno), en blanco sobre negro:
   Cristian · Jared · Catarina · Kyoto
   (dejar la lista fácil de editar por si se suma gente).
4. Termina en negro sólido, sin logo.
Si el motor no soporta control manual del avance, que la secuencia se
reproduzca sola al entrar al artboard, con opción de reiniciarla con un
click/tap en cualquier parte.

---

INSTRUCCIONES ADICIONALES:
- Nunca fotos de stock de cerebros ni ilustraciones médicas realistas —
  mismo lenguaje geométrico/abstracto (blobs, nodos, líneas) del beat A
  al F; que el color y la tipografía, no la iconografía, marquen el
  cambio de tono hacia el cierre.
- Los diagramas cíclicos de los beats A y B tienen que ser visualmente
  IDÉNTICOS en forma (mismo layout, solo cambian las etiquetas).
- Numerar los artboards de forma discreta y continua (ej. "4/9").
- Con solo 7 beats de contenido, priorizá que CADA UNO se lea en menos de
  10 segundos por sobre agregar más información — si algo no entra
  cómodo en un artboard, es señal de recortarlo más, no de agregar un
  artboard extra.
```

## Notas de uso

- El guion completo (qué dice cada orador, con más detalle del que entra en un beat de 60-90 segundos) vive en [`05_guia_presentacion_grupal.md` §0.bis](05_guia_presentacion_grupal.md#0bis--versión-condensada-paseo-rápido-15-min-total) — cada orador debería leer igual el contenido completo de su bloque original (§2-§11 de esa guía) para poder responder preguntas, aunque en el recorrido solo diga la versión corta.
- Si después hace falta recuperar algo del recorrido largo (la línea de tiempo completa de CEOs, el desglose técnico de Jared, etc.), está todo documentado en la misma guía — no se perdió, solo se resumió para esta versión.
- La versión anterior de este prompt (~30 min, 10 bloques) quedó en el historial de git de este archivo.
