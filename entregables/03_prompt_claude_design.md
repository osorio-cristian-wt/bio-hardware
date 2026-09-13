# Prompt para Claude Design — presentación de 15 minutos

> Prompt listo para pegar al invocar el skill `/design`. Es autocontenido (no depende de que la sesión tenga cargado el resto del repo) — trae el contenido condensado de las 11 diapositivas de [`02_guia_presentacion_15min.md`](02_guia_presentacion_15min.md).

---

## Prompt

```
Necesito un canvas de diseño para una presentación universitaria de 15 minutos,
formato 16:9, un artboard por diapositiva (11 diapositivas en total).

TEMA: "Neuronas humanas como hardware de inteligencia artificial" — organoid
intelligence / biocomputación con neuronas humanas vivas como sustrato de
cómputo. Es la introducción de contexto ANTES de un debate universitario, no
el debate en sí: tiene que informar con rigor, sin bajar línea a favor ni en
contra, y terminar lanzando una pregunta/moción.

AUDIENCIA: estudiantes universitarios sin conocimiento previo del tema —
nada de jerga sin explicar.

TONO Y ESTILO VISUAL:
- Editorial / científico-serio, NO ciencia-ficción ni clip-art de "cerebro
  brillante flotando en un frasco". Pensar más en el lenguaje visual de una
  revista como Nature/Wired que en una película de sci-fi.
- Paleta: base neutra (blancos, grises, un azul o teal oscuro como acento) +
  un segundo color de acento cálido reservado ÚNICAMENTE para señalar
  matices/advertencias (la diapositiva 7 es "la de las advertencias" y debe
  distinguirse visualmente del resto).
- Tipografía limpia, alto contraste, texto mínimo por diapositiva — esto se
  narra en voz alta, las diapositivas apoyan, no reemplazan al orador.
- Debe verse bien tanto en modo claro como oscuro.

CONTENIDO POR DIAPOSITIVA (11 artboards, en este orden):

1. PORTADA (0:45 min de exposición)
   Título: "¿Y si la computadora que entrena tu IA... estuviera viva?"
   Subtítulo: "Neuronas humanas como hardware de inteligencia artificial"
   Elemento visual: composición abstracta que sugiera "organoide sobre un
   chip" sin ser literal ni gore — pensar en formas orgánicas simples
   (círculos/blobs) sobre una grilla de circuito, no una imagen médica real.

2. QUÉ ES ESTO
   Título: "No es un mini-cerebro. Es un cultivo de neuronas conectado a
   electrodos."
   3 columnas/tarjetas, mismo concepto con tres nombres distintos:
   - "Organoid Intelligence" — academia (Johns Hopkins)
   - "Synthetic Biological Intelligence" — Cortical Labs (producto)
   - "Wetware computing" — FinalSpark (plataforma de acceso remoto)
   Nota al pie pequeña: "del tamaño de la punta de una aguja — no un cerebro
   con anatomía completa."

3. CÓMO FUNCIONA
   Título: "El circuito básico"
   Diagrama de flujo horizontal, 5 pasos con iconos simples:
   Donante humano (piel/sangre) → células madre reprogramadas (iPSC) →
   organoide 3D → array de microelectrodos (estimula y registra actividad
   eléctrica) → aprendizaje o cómputo por feedback en circuito cerrado.
   Debajo del diagrama, dos cajas comparando los dos enfoques:
   "Aprendizaje activo" (DishBrain: el organoide actúa y recibe
   consecuencias) vs. "Reservoir computing" (Brainoware: el organoide solo
   transforma señales, se entrena una capa externa).

4. LÍNEA DE TIEMPO
   Título: "De laboratorio a producto comercial en 4 años"
   Timeline horizontal con 5 hitos:
   2019 Fundación de Cortical Labs · 2022 DishBrain aprende Pong en 5 min ·
   2023 Paper fundacional "Organoid Intelligence" + Brainoware reconoce voz ·
   2025 Cortical Labs lanza el CL1, primer producto comercial (USD 35.000) ·
   2025-26 Los propios científicos del campo advierten sobre el exceso de
   promesas.

5. LOS DOS JUGADORES COMERCIALES
   Título: "Dos modelos de negocio, la misma tecnología base"
   Tabla comparativa de 2 columnas (Cortical Labs / FinalSpark) x 4 filas:
   Modelo de negocio (venta de hardware USD 35.000 / suscripción USD
   500-mes) · Escala (800.000 neuronas por unidad / ~10.000 por organoide) ·
   Consumo declarado (850-1.000W por rack de 30 unidades / "un millón de
   veces menos" — cifra del tejido aislado) · País (Australia / Suiza).

6. LA PROMESA: VENTAJAS ARGUMENTADAS
   Título: "Lo que se promete"
   3 tarjetas grandes con una cifra cada una, tono afirmativo/optimista:
   - Eficiencia energética: cerebro humano ~1 exaFLOPS a 10-20W vs. 21
     megavatios de una supercomputadora equivalente → ventaja de ~10⁶
   - Eficiencia de datos: DishBrain aprende en 5 minutos vs. AlphaGo,
     160.000 partidas de entrenamiento
   - Demanda comercial real: producto a la venta, suscriptores pagos

7. EL MATIZ: LO QUE NO SE DICE TANTO ⚠️ (diapositiva de advertencia —
   usar el color de acento cálido reservado para esta diapositiva; debe
   sentirse visualmente distinta a todas las demás)
   Título: "¿Comparado con qué, exactamente?"
   4 puntos, cada uno contrarrestando uno de la diapositiva anterior:
   - La cifra de "10⁶ veces más eficiente" compara el CEREBRO COMPLETO
     (86.000 millones de neuronas) contra una supercomputadora — nunca un
     organoide real de laboratorio (100.000-800.000 células) contra un chip
   - El CL1 real consume 850-1.000W por rack — comparable a un servidor GPU
   - Montar un laboratorio de este tipo cuesta USD 50.000 a 250.000+
   - Límite físico duro: sin vascularización, el núcleo del organoide
     necrosa a partir de ~300 micrones — sin solución conocida a corto plazo

8. LA ÉTICA NO ES UNA SOLA PREGUNTA
   Título: "Cinco preguntas distintas, no un sí/no"
   5 preguntas cortas en formato de lista numerada o diagrama radial:
   1. ¿Puede el organoide sufrir?
   2. ¿Es válido el consentimiento si ni la ciencia sabe qué autoriza?
   3. ¿Daña la dignidad humana aunque el organoide nunca sufra?
   4. ¿Es un problema de marketing, no de ética?
   5. ¿Está bien encuadrado el debate público mismo?

9. ¿ESTÁ REGULADO?
   Título: "Sí, pero con un agujero específico"
   Elemento visual simple: semáforo de 3 niveles (verde/amarillo/rojo) del
   marco regulatorio de EE.UU. para quimeras y trasplantes neuronales.
   Texto destacado debajo: "Ninguna norma regula al organoide EN SÍ una vez
   creado — toda la regulación protege al donante humano."

10. CIERRE Y MOCIÓN DEL DEBATE
    Título: "La pregunta que abre el debate"
    Cita/moción centrada, tipografía grande:
    "¿Debería el desarrollo de 'organoid intelligence' continuar sin
    restricciones adicionales a las ya existentes?"

11. PREGUNTAS
    Diapositiva simple de cierre: "Preguntas" + espacio en blanco generoso.

INSTRUCCIONES ADICIONALES:
- Cada diapositiva debe poder leerse en menos de 10 segundos — texto mínimo,
  jerarquía visual clara (título grande, 1-4 puntos de apoyo, nada más).
- No usar fotos de stock de cerebros ni ilustraciones médicas realistas —
  preferir formas geométricas/abstractas simples y consistentes entre
  diapositivas (mismo lenguaje visual para "organoide" en toda la deck).
- Numerar las diapositivas discretamente (ej. "3/11") para que el orador
  pueda ubicarse.
```

## Notas de uso

- Este prompt asume que Claude Design va a generar el **contenido visual** de las 11 diapositivas descriptas en [`02_guia_presentacion_15min.md`](02_guia_presentacion_15min.md) — el texto para decir en voz alta (timing, qué decir) queda en esa guía, no se repite en el canvas.
- Si se quiere iterar el diseño después de la primera pasada, referenciar directamente el artboard por número (ej. "la diapositiva 7, la de las advertencias, necesita más contraste en el color de acento").
