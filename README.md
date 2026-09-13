# bio-hardware — Neuronas humanas como hardware de inteligencia artificial

> Repositorio de investigación para una **presentación grupal + debate universitario** sobre "organoid intelligence" / biocomputación: usar neuronas humanas vivas como sustrato de cómputo para entrenar/ejecutar IA — y qué dispara eso sobre la pregunta de la consciencia.
>
> Metodología replicada de [`casaJustina`](../casaJustina) (ver [WORKFLOW.md](WORKFLOW.md)).

---

## ¿Qué es este repositorio?

Desde 2022 existe una línea de investigación real —no ciencia ficción— que usa cultivos 3D de neuronas humanas (**organoides cerebrales**, derivados de células madre) conectados a electrodos para que aprendan tareas o funcionen como sustrato de cómputo. En 2025 esto pasó de laboratorio a producto comercial (Cortical Labs vende el CL1 por USD 35.000; FinalSpark alquila acceso remoto a organoides vivos).

Este repositorio documenta **qué se hizo, qué ventajas y desventajas técnicas tiene, qué posturas éticas existen, y cómo eso se conecta con la pregunta de qué es la consciencia** — con el objetivo de armar una presentación grupal de ~30 minutos y, a partir de ahí, un debate universitario riguroso, no un intercambio de titulares de prensa.

## Estado del repositorio

| Bloque | Estado | Archivos |
|---|---|---|
| 📚 Investigación de fuentes primarias | **Completa** | 29 fuentes en `sources/` |
| 📘 Glosario de términos | Completo | `GLOSARIO.md` |
| 🧬 Síntesis del campo (línea de tiempo, cómo funciona, actores comerciales, datos duros) | **Completa** | `research.md` |
| 🔬 Análisis: ventajas y desventajas técnicas | **Completo** | `analisis/01` |
| ⚖️ Análisis: mapa de posturas éticas (5 ejes, con réplicas) | **Completo** | `analisis/02` |
| 🧠 Análisis: entrenamiento comparado (IA / humano / organoide) y el debate de la consciencia | **Completo** | `analisis/03` |
| 🎬 Análisis: de la mosca a la ficción — ciencia real vs. especulación | **Completo** | `analisis/04` |
| 🎤 Guía lista para el debate (argumentos, réplicas, citas, preguntas de moderador) | **Completa** | `entregables/01` |
| 🖥️ Guía de presentación individual de 15 min | **Histórica** — superada por la versión grupal | `entregables/02` |
| 🎨 Prompt para Claude Design (canvas visual, estructura grupal actual) | **Completo — pisa versiones anteriores** | `entregables/03` |
| 🎭 Guía de presentación **grupal** (~30 min, 4 oradores, cierre "I Have No Mouth") | **Completa — es la versión vigente** | `entregables/05` |
| 👥 Reparto de investigación por integrante | **Completo** | `entregables/06` |

## Estructura del repositorio

```
bio-hardware/
├── README.md              ← este archivo
├── WORKFLOW.md             ← metodología para seguir investigando
├── GLOSARIO.md              ← términos y siglas del campo
├── research.md              ← síntesis maestra
│
├── sources/                 ← 29 fuentes documentadas, 1 archivo c/u
│   ├── 01-06  ← técnico/fundacional (DishBrain, Brainoware, FinalSpark, Cortical Labs, workshop OI)
│   ├── 07-10, 13, 15  ← ético/legal/social (consentimiento, gobernanza, crítica filosófica)
│   ├── 11-12  ← percepción pública y crítica interna del propio campo científico
│   ├── 14, 16  ← síntesis de divulgación y guía práctica de costos
│   ├── 17-21  ← paradigmas de entrenamiento y consciencia (RL, condicionamiento operante,
│   │           "Reward is Enough" y su réplica, el problema difícil de la consciencia)
│   └── 22-29  ← carrera de la IA de silicio (Amodei, Altman, carta de pausa, METR) y
│               de la mosca a la ficción (FlyWire, simulación virtual, emulación de cerebro
│               completo, "I Have No Mouth, and I Must Scream")
│
├── analisis/                ← evaluación crítica, no solo resumen
│   ├── 01_ventajas_y_desventajas_tecnicas.md
│   ├── 02_posturas_eticas_mapa_debate.md
│   ├── 03_entrenamiento_comparado_y_el_debate_de_la_conciencia.md
│   └── 04_de_la_mosca_a_la_ficcion_ciencia_real_vs_especulacion.md
│
└── entregables/
    ├── 01_guia_debate.md                    ← el documento para usar en el debate mismo
    ├── 02_guia_presentacion_15min.md        ← histórica: versión individual de 15 min
    ├── 03_prompt_claude_design.md           ← prompt vigente del canvas (estructura grupal)
    ├── 05_guia_presentacion_grupal.md       ← VIGENTE: ~30 min, 4 oradores, timing y guion
    └── 06_reparto_investigacion_equipo.md   ← qué lee cada integrante antes de presentar
```

## Cómo navegar

- **Si vas a armar o ensayar la presentación grupal** → andá directo a [`entregables/05_guia_presentacion_grupal.md`](entregables/05_guia_presentacion_grupal.md): los 10 bloques, quién dice qué, timing exacto y el guion sugerido para el cierre.
- **Si sos parte del equipo y necesitás saber qué leer** → [`entregables/06_reparto_investigacion_equipo.md`](entregables/06_reparto_investigacion_equipo.md).
- **Si vas a generar el diseño visual** → [`entregables/03_prompt_claude_design.md`](entregables/03_prompt_claude_design.md), autocontenido para pegar en `/design`.
- **Si vas a preparar o moderar el debate posterior** → [`entregables/01_guia_debate.md`](entregables/01_guia_debate.md): moción, argumentos de ambos lados con fuente, réplicas anticipadas, citas listas para usar.
- **Si querés entender el panorama completo antes de armar tu parte** → leé [`research.md`](research.md): línea de tiempo, cómo funciona técnicamente, comparación de actores comerciales, datos duros consolidados.
- **Si querés el análisis crítico de un ángulo específico** → `analisis/01` (¿es cierto el argumento de eficiencia energética?), `analisis/02` (mapa de posturas éticas), `analisis/03` (entrenamiento comparado y consciencia), o `analisis/04` (dónde termina la ciencia y empieza la ficción en el cierre).
- **Si querés verificar una afirmación contra la fuente original** → `sources/NN_*.md`.
- **Si una sigla no la conocés** (OI, SBI, MEA, iPSC, ELSI, conectoma...) → `GLOSARIO.md`.

## Hallazgos clave (cheat sheet)

- **No es ciencia ficción, hasta que decidimos que lo sea a propósito en el cierre:** hay productos comerciales reales (CL1, USD 35.000; Neuroplatform, USD 500/mes) desde 2024-2025, y el cierre de la presentación salta deliberadamente a un escenario ficcional a partir de un logro real (ver siguiente punto).
- **El argumento de venta central —eficiencia energética "millón de veces mejor"— está mal aplicado:** compara el cerebro humano completo contra una supercomputadora, no un organoide de laboratorio contra un chip. El propio CL1 consume 850-1.000 W por rack, comparable a un servidor GPU convencional.
- **Se entrena con el mismo esquema formal en los tres casos:** una IA de silicio (aprendizaje por refuerzo), un humano (condicionamiento operante) y un organoide (DishBrain, principio de energía libre) ajustan su comportamiento con la misma estructura conducta→consecuencia→ajuste. Eso no resuelve si los tres tienen experiencia subjetiva — es la pregunta que dispara, sin cerrarla. Ver [analisis/03](analisis/03_entrenamiento_comparado_y_el_debate_de_la_conciencia.md).
- **Ya se mapeó y se corrió virtualmente un cerebro adulto completo — el de una mosca:** 139.255 neuronas, 50 millones de conexiones (FlyWire, 2024), corriendo como simulación en una laptop y prediciendo comportamiento real (Shiu et al., 2024). El propio investigador principal dijo en público que "el premio final es la matriz de cableado de un cerebro humano" — pero esa meta está ~600.000 veces más lejos en escala, sin proyecto financiado apuntando ahí hoy. Ver [analisis/04](analisis/04_de_la_mosca_a_la_ficcion_ciencia_real_vs_especulacion.md).
- **Los propios CEOs de la industria piden frenar la carrera, y la carrera no frena:** de la carta de 2023 (30.000 firmas, sin Altman ni Anthropic) a Altman pidiéndole regulación al Congreso (2023) al ensayo de Amodei pidiendo "pacear la frontera" (12/09/2026, con Altman de acuerdo el mismo día) — tres años de pedidos públicos, ningún mecanismo vinculante todavía.
- **Hay un vacío regulatorio específico también para organoides:** la regulación vigente (EE.UU., marco de 3 niveles) protege al donante humano, pero ninguna norma regula directamente al organoide una vez creado.
- **No hay un solo "bando ético"** — hay al menos 5 posturas que responden preguntas distintas: ¿puede sufrir?, ¿es válido el consentimiento?, ¿daña la dignidad humana aunque no sufra?, ¿es un problema de marketing más que de ética?, ¿está mal encuadrado el debate público mismo? Ver [analisis/02](analisis/02_posturas_eticas_mapa_debate.md).

## Pendiente / próximos pasos sugeridos

- **Asignar oradores a los bloques 6-9** de la presentación grupal (time-lapse, CEOs, la mosca, el cierre) — quedaron sin asignar en [`entregables/05`](entregables/05_guia_presentacion_grupal.md).
- **Decidir el tratamiento del video** de "I Have No Mouth" (externo vs. embebido como asset) antes de generar el canvas de diseño — ver [`entregables/05 §12`](entregables/05_guia_presentacion_grupal.md#12-nota-técnica-importante--el-video-dentro-del-canvas-de-diseño).
- **Confirmar la duración real** asignada a la presentación — esta guía asumió ~30 minutos a falta de un dato concreto.
- Investigar marco legal y cobertura académica **argentina/latinoamericana** específica (no cubierto en esta ronda de investigación).
- Verificar citas textuales de las fuentes cuyo texto completo estuvo bloqueado por paywall (ver "Observaciones" en `sources/02`, `08`, `15`, `16`, `22`, `27`).
- Si el formato de debate lo permite, considerar el "formato por ejes" sugerido en [analisis/02 §6](analisis/02_posturas_eticas_mapa_debate.md#6-tabla-resumen-para-armar-equipos-de-debate) en vez del clásico a favor/en contra.
