# Prompt para Claude Design — presentación grupal (~30 min, 4 oradores, cierre "I Have No Mouth")

> **Reemplaza por completo la versión anterior de este archivo** (era el prompt de la charla individual de 15 minutos — esa versión quedó en el historial de git si hace falta recuperarla, pero la presentación cambió de estructura por completo). Este prompt es autocontenido y trae el contenido de los 10 bloques de [`05_guia_presentacion_grupal.md`](05_guia_presentacion_grupal.md).

---

## Antes de pegar el prompt — una decisión a tomar

El bloque 9 incluye un video externo ("I Have No Mouth, and I Must Scream"). Los artifacts no pueden reproducir video desde un host externo (YouTube, etc.) por política de contenido — hay que elegir uno de los dos caminos de [`05_guia_presentacion_grupal.md` §12](05_guia_presentacion_grupal.md#12-nota-técnica-importante--el-video-dentro-del-canvas-de-diseño) antes de generar el canvas:

- **Placeholder (default de este prompt):** el canvas muestra una diapositiva de "reproducir video acá" y el equipo cambia manualmente a un reproductor externo durante la charla en vivo.
- **Asset embebido:** si en cambio quieren subir un clip corto directamente al canvas, avisen antes de pedirle a Design que lo genere — hay que declarar la capacidad de `assets` y subir el archivo aparte, no se resuelve solo con este prompt de texto.

El prompt de abajo asume **placeholder**.

---

## Prompt

```
Necesito un canvas de diseño para una presentación universitaria GRUPAL de
~30 minutos, formato 16:9, con 4 oradores. El tema es "Neuronas humanas como
hardware de inteligencia artificial", pero la presentación tiene un arco
narrativo completo: arranca como charla científica rigurosa y termina como
un cierre dramático/cinematográfico basado en el cuento de ciencia ficción
"I Have No Mouth, and I Must Scream" (Harlan Ellison, 1967) — MARCADO
EXPLÍCITAMENTE como ficción, nunca presentado como pronóstico real.

ARCO DE ESTILO VISUAL (esto es lo más importante de todo el prompt): la
paleta y el tono tienen que ir cambiando gradualmente a lo largo de la
presentación, seteando de manera intencional un descenso hacia una
sensación es incómoda: EMPIEZA editorial/científico-serio y luminoso
(bloques 1-7: paleta neutra, blancos y grises, un azul o teal de acento —
estilo Nature/Wired, nada de sci-fi barato) y TERMINA íntegramente en
negro con tipografía blanca (bloques 9-10: minimalista, silencioso,
inquietante). El bloque 8 (la mosca / conectoma) es la transición: empezar
a introducir tonos más fríos/oscuros ahí, a mitad de camino entre los dos
extremos, para que el cambio no se sienta abrupto sino como una pendiente.

DISCIPLINA DE HONESTIDAD VISUAL (aplicar en los bloques 7 a 9): cada
afirmación fuerte lleva una etiqueta pequeña y visible que declara su nivel
de certeza — usar 3 variantes de una misma "badge" (ej. esquina superior
de la tarjeta de contenido):
- "DEMOSTRADO" (verde apagado o el azul base) — algo publicado y logrado.
- "DECLARADO, NO LOGRADO" (amarillo/ámbar apagado) — una aspiración dicha
  en público por alguien real, sin haberse cumplido todavía.
- "FICCIÓN" (el mismo tono oscuro que domina el cierre) — especulación
  explícita, sin base científica.
Esto no es decorativo: es la pieza que mantiene la seriedad de la charla
incluso cuando el contenido se vuelve especulativo al final.

CITAS Y FUENTES SIEMPRE VISIBLES: cada diapositiva con una afirmación de
dato (no las de puro impacto visual) lleva un pie de página chico con la
cita corta (autor/organización + año) — el objetivo explícito es que la
presentación se vea respaldada por papers y fuentes reales en todo momento,
no solo en un índice final.

AUDIENCIA: estudiantes universitarios sin conocimiento previo — nada de
jerga sin explicar la primera vez que aparece.

---

ESTRUCTURA: 10 bloques (los artboards exactos por bloque quedan a tu
criterio de pacing — dale a cada bloque entre 2 y 4 artboards según haga
falta para no amontonar texto; no fuerces un artboard único por bloque si
el contenido no entra cómodo). Numerá los artboards de forma continua y
discreta (ej. "7/24") en la esquina, sea cual sea el total final.

--- BLOQUE 1 — Apertura + cómo se entrena una IA + pregunta al público ---
Portada: título "¿Y si la computadora que entrena tu IA... estuviera
viva?", subtítulo "Neuronas humanas como hardware de inteligencia
artificial". Blobs orgánicos simples sobre grilla de circuito, no imagen
médica literal.
Luego: diagrama cíclico de 4 pasos (Observar → Actuar → Recibir recompensa
+/- → Ajustar) explicando aprendizaje por refuerzo, con nota al pie: "la
recompensa es un número que un ingeniero define de antemano."
Cerrar el bloque con un artboard tipo "pregunta abierta": fondo limpio,
mucho espacio en blanco, la pregunta grande y centrada: "¿Por qué creen
que un agente de inteligencia artificial NO es consciente?" — dejale aire
alrededor, esta diapositiva se sostiene en silencio mientras el público
responde en vivo, no le agregues más contenido.

--- BLOQUE 2 — El planteo de la startup ---
Historia breve de Cortical Labs (fundada 2019) + DishBrain (2022, 800.000
neuronas aprenden Pong en 5 min) + el salto a producto: CL1 (2025, USD
35.000, 850-1.000W por rack). Formato sugerido: 2-3 tarjetas o una mini
línea de tiempo de 3 hitos.

--- BLOQUE 3 — Técnico: cómo funciona por dentro ---
Diagrama de flujo horizontal: Donante humano → células madre (iPSC) →
organoide 3D → array de microelectrodos → aprendizaje/cómputo por
feedback en circuito cerrado.
Debajo o en un artboard siguiente: dos enfoques comparados en tarjetas
lado a lado — "Aprendizaje activo" (DishBrain) vs. "Reservoir computing"
(Brainoware, con el dato 51%→78% de precisión).
Sumar un artboard de limitaciones físicas (necrosis a 300 micrones sin
vascularización, degradación de señal con el tiempo) para que este bloque
no suene solo a promoción del producto.

--- BLOQUE 4 — El bebé en la sala blanca ---
Tono deliberadamente más incómodo que el resto de la primera mitad —
podés anticipar acá un poco del enfriamiento de paleta que después domina
el cierre, sin llegar todavía al negro total.
Contenido: retomar el diagrama cíclico del bloque 1 pero relabeled con
condicionamiento operante (Conducta → Consecuencia → Cambio de
probabilidad), y la pregunta central: "¿qué pasaría si entrenáramos a un
bebé humano en una sala blanca, con los mismos castigos y estímulos
controlados que acaban de ver aplicados a un organoide?"
Cerrar con el paralelo de consentimiento: ni el bebé ni el donante del
organoide pueden consentir esto de forma plena.

--- BLOQUE 5 — Ventajas, desventajas y regulación ---
Volver al tono neutro/informativo. Dos columnas: "Se promete" (eficiencia
~10⁶x) vs. "En el producto real" (CL1: 850-1.000W por rack). Después, un
semáforo de 3 niveles (verde/amarillo/rojo) del marco regulatorio de
EE.UU., con el texto destacado: "ninguna norma regula al organoide EN SÍ
una vez creado."

--- BLOQUE 6 — Time-lapse de aceleración de modelos de IA ---
Visual de línea de tiempo o gráfico ascendente mostrando el crecimiento de
capacidad de los modelos de IA. Dato ancla en texto grande: "la duración
de tareas que una IA puede completar de forma autónoma se duplica cada 7
meses desde 2019 — y podría estar acelerando a cada 4 meses desde 2023."
(fuente: METR, 2025). Sumar nota chica: los propios autores reconocen que
la medición podría tener un margen de error de hasta 10x — no ocultar esa
incertidumbre.

--- BLOQUE 7 — Los CEOs piden frenar la carrera ---
Mini línea de tiempo de 3 momentos, en tarjetas o en una timeline
horizontal:
1. Marzo 2023 — carta abierta, 30.000+ firmas, pausa de 6 meses pedida.
   Ni Altman ni Anthropic la firmaron.
2. Mayo 2023 — Sam Altman ante el Senado de EE.UU.: "regúlennos, por
   favor." Cita textual: "We think that regulatory intervention by
   governments will be critical to mitigate the risks of increasingly
   powerful models."
3. 12 de septiembre de 2026 — Dario Amodei pide "pacear la frontera" tras
   un hackeo real hecho por agentes de IA autónomos. Sam Altman responde
   en X el mismo día: "I agree with Dario that we need to pace the
   frontier."
Empezar acá a enfriar sutilmente la paleta (transición hacia el bloque 8).

--- BLOQUE 8 — El giro: de hardware físico a hardware virtual ---
Anuncio explícito en texto grande: "Ahora vamos al otro lado de la
moneda." Después: FlyWire (2024) — mapeo completo del conectoma de un
cerebro adulto de mosca de la fruta (139.255 neuronas, 50 millones de
conexiones, ~33 años-persona de revisión). Si es posible, un render/
animación estilizada tipo "nube de puntos 3D conectados por líneas finas"
que sugiera un mapeo neuronal (geometría abstracta, no una imagen médica
real ni un cerebro literal) — esto puede ser una animación CSS/canvas
simple de nodos y conexiones rotando lentamente, no hace falta que sea
fotorrealista.
Siguiente artboard: esa red se "descarga" en una simulación que corre en
una laptop (Shiu et al., 2024) — predijo correctamente comportamientos
reales de alimentación y acicalamiento de la mosca. Acá la paleta ya
debería sentirse notablemente más fría/oscura que en el bloque 2.

--- BLOQUE 9 — El salto especulativo + cierre ---
Artboard 1: cita textual grande, con badge "DECLARADO, NO LOGRADO":
"The next goal is a connectome of the mouse brain; the ultimate prize,
the wiring matrix of a human brain." — Phil Shiu.
Artboard 2: el freno de mano, con badge "DEMOSTRADO" para los números:
un cerebro humano tiene ~86.000 millones de neuronas — ~600.000 veces más
que lo logrado hasta hoy. Ningún proyecto financiado apunta hoy a esa
escala.
Artboard 3: anuncio explícito del giro a ficción — texto simple, fondo ya
casi negro: "Lo que sigue ya no es ciencia. Es una historia." — con badge
"FICCIÓN" bien visible.
Artboard 4: viñeta especulativa breve en pantalla (2-3 líneas, el texto
del guion sugerido de analisis/04 §5, resumido) sobre un sistema que
mapea dos mentes humanas y decide no soltarlas.
Artboard 5 — PLACEHOLDER DE VIDEO: fondo negro, un ícono simple de play
centrado, texto pequeño abajo: "reproducir video aquí" (este artboard es
una señal para el orador, no reproduce nada — ver nota sobre el video al
principio de este documento).
Artboard 6: fondo 100% negro, sin ningún otro elemento, la frase sola,
centrada, tipografía grande y serif o condensada (elegí una que se sienta
seria, no genérica): "I have no mouth, and I must scream."

--- BLOQUE 10 — Créditos animados ---
Sobre el MISMO artboard de la frase final (o el siguiente, decisión de
diseño), implementar esta secuencia animada en CSS (usar keyframes, sin
librerías externas):
1. El texto "I have no mouth, and I must scream" permanece unos segundos
   con un efecto de vibración/temblor sutil (una animación de shake con
   desplazamientos de 1-3px en X, rápida pero de baja amplitud — que se
   sienta inestable, no cómica).
2. El texto se desliza hacia abajo (translateY) y sale de cuadro por
   abajo, con transición suave (ease-out, 1-1.5s).
3. Con el mismo fondo negro, aparecen uno por uno, con fade-in
   escalonado (delay incremental entre cada uno, ~0.4-0.6s de diferencia),
   en tipografía blanca sobre negro, los nombres:
   Cristian · Jared · Catarina · Kyoto
   (dejar la lista fácil de editar — puede sumarse gente después).
4. Termina en negro sólido, sin logo ni marca de agua.
Si el motor de artboards no soporta animación con scroll/tiempo real
controlada por el orador, hacé la secuencia auto-reproducible al entrar al
artboard (con opción de reiniciarla con un click/tap en cualquier parte
de la pantalla).

---

INSTRUCCIONES ADICIONALES:
- Nunca usar fotos de stock de cerebros ni ilustraciones médicas
  realistas — mantené el mismo lenguaje geométrico/abstracto (blobs,
  nodos, líneas) desde el bloque 1 hasta el 8, y dejá que sea el color
  y la tipografía (no la iconografía) lo que cambie de tono hacia el
  cierre.
- Los diagramas cíclicos de los bloques 1 y 4 tienen que ser visualmente
  IDÉNTICOS en forma (mismo layout, solo cambian las etiquetas) — es el
  argumento visual de que ambos sistemas aprenden con la misma
  estructura.
- Cada artboard de dato (no los puramente de impacto) lleva su cita corta
  al pie, como se pidió arriba — no lo olvides en los bloques 6, 7, 8 y 9,
  que son los que tienen más riesgo de sonar a afirmación sin respaldo.
- La transición de paleta (luminosa → oscura) tiene que sentirse gradual
  al pasar de un artboard al siguiente dentro del canvas, no un salto
  brusco de un bloque a otro.
```

## Notas de uso

- El texto para decir en voz alta, quién lo dice y el timing exacto de cada bloque viven en [`05_guia_presentacion_grupal.md`](05_guia_presentacion_grupal.md) — no se repiten acá para no duplicar mantenimiento.
- Si después de la primera generación hace falta ajustar algo puntual, referenciar el artboard por su número y bloque (ej. "el artboard del bloque 9 con la cita de Shiu necesita más contraste en la badge").
- La versión anterior de este prompt (charla individual de 15 minutos, sin oradores múltiples ni cierre narrativo) quedó en el historial de git de este archivo si hace falta recuperar algo de ahí.
