# bio-hardware — Neuronas humanas como hardware de inteligencia artificial

> Repositorio de investigación para preparar un **debate** sobre "organoid intelligence" / biocomputación: usar neuronas humanas vivas como sustrato de cómputo para entrenar/ejecutar IA.
>
> Metodología replicada de [`casaJustina`](../casaJustina) (ver [WORKFLOW.md](WORKFLOW.md)).

---

## ¿Qué es este repositorio?

Desde 2022 existe una línea de investigación real —no ciencia ficción— que usa cultivos 3D de neuronas humanas (**organoides cerebrales**, derivados de células madre) conectados a electrodos para que aprendan tareas o funcionen como sustrato de cómputo. En 2025 esto pasó de laboratorio a producto comercial (Cortical Labs vende el CL1 por USD 35.000; FinalSpark alquila acceso remoto a organoides vivos).

Este repositorio documenta **qué se hizo, qué ventajas y desventajas técnicas tiene, y qué posturas éticas existen**, con el objetivo de armar un debate universitario riguroso, no un intercambio de titulares de prensa.

## Estado del repositorio

| Bloque | Estado | Archivos |
|---|---|---|
| 📚 Investigación de fuentes primarias | **Completa** | 21 fuentes en `sources/` |
| 📘 Glosario de términos | Completo | `GLOSARIO.md` |
| 🧬 Síntesis del campo (línea de tiempo, cómo funciona, actores comerciales, datos duros) | **Completa** | `research.md` |
| 🔬 Análisis: ventajas y desventajas técnicas | **Completo** | `analisis/01` |
| ⚖️ Análisis: mapa de posturas éticas (5 ejes, con réplicas) | **Completo** | `analisis/02` |
| 🧠 Análisis: entrenamiento comparado (IA / humano / organoide) y el debate de la consciencia | **Completo — eje central de la presentación actual** | `analisis/03` |
| 🎤 Guía lista para el debate (argumentos, réplicas, citas, preguntas de moderador) | **Completa** | `entregables/01` |
| 🖥️ Guía de presentación de 15 min (timing + contenido por diapositiva) | **v2 — eje reorientado a entrenamiento/consciencia** | `entregables/02` |
| 🎨 Prompt para Claude Design (canvas visual v1, 11 diapositivas) | **Completo** | `entregables/03` |
| 🎨 Prompt para Claude Design — edición a v2 (12 diapositivas) | **Completo** | `entregables/04` |

## Estructura del repositorio

```
bio-hardware/
├── README.md              ← este archivo
├── WORKFLOW.md             ← metodología para seguir investigando
├── GLOSARIO.md              ← términos y siglas del campo
├── research.md              ← síntesis maestra (13 secciones)
│
├── sources/                 ← 21 fuentes documentadas, 1 archivo c/u
│   ├── 01-06  ← técnico/fundacional (DishBrain, Brainoware, FinalSpark, Cortical Labs, workshop OI)
│   ├── 07-10, 13, 15  ← ético/legal/social (consentimiento, gobernanza, crítica filosófica)
│   ├── 11-12  ← percepción pública y crítica interna del propio campo científico
│   ├── 14, 16  ← síntesis de divulgación y guía práctica de costos
│   └── 17-21  ← paradigmas de entrenamiento y consciencia (RL, condicionamiento operante,
│               "Reward is Enough" y su réplica, el problema difícil de la consciencia)
│
├── analisis/                ← evaluación crítica, no solo resumen
│   ├── 01_ventajas_y_desventajas_tecnicas.md
│   ├── 02_posturas_eticas_mapa_debate.md
│   └── 03_entrenamiento_comparado_y_el_debate_de_la_conciencia.md   ← eje central actual
│
└── entregables/
    ├── 01_guia_debate.md                    ← el documento para usar en el debate mismo
    ├── 02_guia_presentacion_15min.md        ← v2: timing + contenido, eje entrenamiento/consciencia
    ├── 03_prompt_claude_design.md           ← prompt v1 (11 diapositivas, ya usado)
    └── 04_prompt_claude_design_edicion.md   ← prompt v2: edita el canvas a la nueva estructura (12)
```

## Cómo navegar

- **Si vas a preparar o moderar el debate ya mismo** → andá directo a [`entregables/01_guia_debate.md`](entregables/01_guia_debate.md): moción, definiciones, argumentos de ambos lados con fuente, réplicas anticipadas, citas listas para usar y errores frecuentes a evitar.
- **Si querés entender el panorama completo antes de armar tu posición** → leé [`research.md`](research.md): línea de tiempo, cómo funciona técnicamente, comparación de los dos actores comerciales (Cortical Labs vs. FinalSpark), datos duros consolidados y el mapa de 5 posturas éticas.
- **Si querés el análisis crítico de un ángulo específico** → `analisis/01` (¿es cierto el argumento de eficiencia energética?), `analisis/02` (¿cuáles son las posturas éticas reales, más allá de "a favor/en contra"?), o `analisis/03` (¿qué implica que una IA, un humano y un organoide aprendan con el mismo esquema de premio y castigo? — el eje que sostiene la presentación actual).
- **Si querés verificar una afirmación contra la fuente original** → `sources/NN_*.md`.
- **Si una sigla no la conocés** (OI, SBI, MEA, iPSC, ELSI...) → `GLOSARIO.md`.
- **Si querés seguir investigando otro ángulo** (ej. marco legal argentino, cobertura latinoamericana) → leé `WORKFLOW.md`.

## Hallazgos clave (cheat sheet)

- **No es ciencia ficción:** hay productos comerciales reales (CL1, USD 35.000; Neuroplatform, USD 500/mes) desde 2024-2025.
- **El argumento de venta central —eficiencia energética "millón de veces mejor"— está mal aplicado:** compara el cerebro humano completo contra una supercomputadora, no un organoide de laboratorio contra un chip. El propio CL1 consume 850-1.000 W por rack, comparable a un servidor GPU convencional.
- **Las demostraciones técnicas son reales pero acotadas:** DishBrain aprende Pong en 5 minutos; Brainoware clasifica vocales japonesas con 78% de precisión sobre un set cerrado de 8 hablantes — lejos de cualquier tarea de IA de producción.
- **Hay un vacío regulatorio específico:** la regulación vigente (EE.UU., marco de 3 niveles) protege al donante humano, pero ninguna norma regula directamente al organoide una vez creado.
- **Se entrena con el mismo esquema formal en los tres casos:** una IA de silicio (aprendizaje por refuerzo), un humano (condicionamiento operante — el bebé y el caramelo) y un organoide (DishBrain, principio de energía libre) ajustan su comportamiento con la misma estructura conducta→consecuencia→ajuste. Eso no resuelve si los tres tienen experiencia subjetiva — es justamente la pregunta que dispara, sin cerrarla. Ver [analisis/03](analisis/03_entrenamiento_comparado_y_el_debate_de_la_conciencia.md).
- **No hay un solo "bando ético"** — hay al menos 5 posturas que responden preguntas distintas: ¿puede sufrir?, ¿es válido el consentimiento?, ¿daña la dignidad humana aunque no sufra?, ¿es un problema de marketing más que de ética?, ¿está mal encuadrado el debate público mismo? Ver [analisis/02](analisis/02_posturas_eticas_mapa_debate.md).
- **La propia comunidad científica está dividida:** Stanford, Cold Spring Harbor y Cambridge advirtieron en 2025 que el exceso de promesas podría generar un backlash regulatorio que dañe también la investigación médica legítima con organoides.

## Pendiente / próximos pasos sugeridos

- Investigar marco legal y cobertura académica **argentina/latinoamericana** específica (no cubierto en esta ronda de investigación).
- Verificar citas textuales de las 4 fuentes cuyo texto completo estuvo bloqueado por paywall en esta sesión (ver "Observaciones" en `sources/02`, `08`, `15`, `16`).
- Si el formato de debate lo permite, considerar el "formato por ejes" sugerido en [analisis/02 §6](analisis/02_posturas_eticas_mapa_debate.md#6-tabla-resumen-para-armar-equipos-de-debate) en vez del clásico a favor/en contra.
