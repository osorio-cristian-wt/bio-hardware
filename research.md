# Research — Neuronas humanas como hardware de IA (Organoid Intelligence / Wetware Computing)

> Síntesis maestra de 16 fuentes documentadas en [`sources/`](sources/). Pensado para leerse de corrido y dar contexto completo sin abrir cada fuente — pero cada afirmación remite a una ficha rastreable.
>
> **Fecha de cierre de esta síntesis:** 2026-09-13

---

## 1. Qué es el campo y cómo se llama

No hay un solo nombre consolidado — conviven tres etiquetas que se solapan pero no son idénticas:

| Término | Quién lo usa | Énfasis |
|---|---|---|
| **Organoid Intelligence (OI)** | Johns Hopkins (Smirnova, Hartung) — [01](sources/01_smirnova_2023_organoid_intelligence.md), [06](sources/06_oi_workshop_baltimore_declaration_2022.md) | Agenda científica de una década; combina cómputo Y neurociencia/medicina |
| **Synthetic Biological Intelligence (SBI)** | Cortical Labs (DishBrain/CL1) — [02](sources/02_kagan_2022_dishbrain_neuron.md), [03](sources/03_cortical_labs_cl1.md), [16](sources/16_starting_sbi_lab_patterns_2025.md) | El sistema híbrido neurona-silicio como producto/plataforma |
| **Wetware computing** | FinalSpark — [05](sources/05_finalspark_neuroplatform_2024.md) | El organoide como "hardware" alquilable, análogo a un servidor cloud |

Los tres describen la misma arquitectura base: **neuronas vivas (de ratón o derivadas de células madre humanas/iPSC) cultivadas sobre un array de microelectrodos (MEA), integradas en un circuito cerrado con estimulación/registro eléctrico, que aprenden o computan a partir de feedback.**

---

## 2. Línea de tiempo (hitos verificados)

| Año | Hito | Fuente |
|---|---|---|
| 2019 | Fundación de Cortical Labs (Melbourne) | [03](sources/03_cortical_labs_cl1.md) |
| feb. 2022 | Workshop fundacional de OI en Johns Hopkins → "Baltimore Declaration" | [06](sources/06_oi_workshop_baltimore_declaration_2022.md) |
| oct. 2022 | Publicación de DishBrain en *Neuron* (Kagan et al.) — neuronas aprenden Pong en 5 min | [02](sources/02_kagan_2022_dishbrain_neuron.md) |
| feb. 2023 | Paper fundacional "Organoid Intelligence" en *Frontiers in Science* (Smirnova et al.) | [01](sources/01_smirnova_2023_organoid_intelligence.md) |
| mar. 2023 | Primera crítica filosófica pública fuerte ("Just Say No", Hanna) | [13](sources/13_critica_filosofica_hanna_2023.md) |
| dic. 2023 | Publicación de "Brainoware" en *Nature Electronics* (reconocimiento de voz) | [04](sources/04_brainoware_2023.md) |
| 2024 | FinalSpark abre la Neuroplatform a acceso académico remoto (USD 500/mes) | [05](sources/05_finalspark_neuroplatform_2024.md) |
| mar. 2025 | Cortical Labs lanza el CL1, primera computadora biológica comercial (USD 35.000) | [03](sources/03_cortical_labs_cl1.md) |
| nov. 2025 | Pioneros del campo advierten públicamente contra el hype ("podría causar backlash regulatorio") | [12](sources/12_stat_news_2025_hype_backlash.md) |
| 2026 | Primer estudio de opinión pública representativo sobre biocomputadoras (EE.UU.) | [11](sources/11_percepcion_publica_2026.md) |

**Lectura del patrón:** en menos de 4 años el campo pasó de un paper de laboratorio (DishBrain, 2022) a un producto comercial con precio de lista (CL1, 2025) — mucho más rápido que la maduración típica de la gobernanza bioética, que recién en 2025-2026 empieza a producir advertencias internas y estudios de percepción pública.

---

## 3. Cómo funciona técnicamente (denominador común)

```
┌──────────────────────────────────────────────────────────────┐
│  DONANTE HUMANO (piel/sangre) → células madre (iPSC)         │
└───────────────────────────┬────────────────────────────────────┘
                            ▼
              Reprogramación → neuronas / organoide 3D
                    (~50.000–800.000 células según sistema)
                            │
                            ▼
        ┌───────────────────────────────────────┐
        │   Array de microelectrodos (MEA)       │  ← interfaz física
        │   + soporte vital (microfluídica,      │
        │   incubadora, control CO2/O2/temp)     │
        └───────────────┬─────────────────────────┘
                        ▼
   Estimulación eléctrica  ⇄  Registro de actividad neuronal
   (input codificado)         (spikes → output decodificado)
                        │
                        ▼
        Feedback en circuito cerrado (closed-loop)
        → el sistema "aprende" minimizando error/sorpresa
          (principio de energía libre de Friston, o
           reservoir computing con regresión lineal/logística)
```

Esto es válido tanto para DishBrain/CL1 (Cortical Labs, [02](sources/02_kagan_2022_dishbrain_neuron.md)/[03](sources/03_cortical_labs_cl1.md)) como para Brainoware ([04](sources/04_brainoware_2023.md)) y la Neuroplatform ([05](sources/05_finalspark_neuroplatform_2024.md)) — cambian la escala, el protocolo de diferenciación celular y el algoritmo de decodificación, pero no el principio.

**Dos paradigmas de cómputo distintos conviven bajo el mismo nombre:**
- **Aprendizaje por refuerzo/predicción activa** (DishBrain/CL1): el organoide "actúa" y recibe consecuencias — se apoya en el principio de energía libre.
- **Reservoir computing** (Brainoware): el organoide no se entrena internamente; se usa su dinámica no lineal *tal cual* como "caja" de transformación, y solo se entrena una capa de lectura externa (regresión). Es un enfoque más simple y más fácil de justificar sin invocar aprendizaje "propio" del tejido.

---

## 4. Actores comerciales (comparación)

| | Cortical Labs (CL1) | FinalSpark (Neuroplatform) |
|---|---|---|
| País | Australia | Suiza |
| Modelo de negocio | Venta de hardware (USD 35.000/unidad) + Wetware-as-a-Service cloud (USD 300/semana) | Suscripción académica compartida (USD 500/usuario/mes) |
| Escala | 800.000 neuronas/unidad | ~10.000 neuronas/organoide, 4 organoides/MEA |
| Consumo declarado | 850–1.000 W (rack de 30 unidades) | "un millón de veces menos" que un chip digital (cifra del organoide aislado, no del sistema completo) |
| Financiamiento notable | In-Q-Tel (fondo vinculado a la CIA), Horizons Ventures | Académico/investigación |
| Vida útil | ~6 meses (hasta ~1 año) | 100+ días |

Fuentes: [03](sources/03_cortical_labs_cl1.md), [05](sources/05_finalspark_neuroplatform_2024.md).

---

## 5. Datos duros consolidados

| Métrica | Valor | Fuente |
|---|---|---|
| Cerebro humano completo | ~1 exaFLOPS a 10-20 W | [01](sources/01_smirnova_2023_organoid_intelligence.md) |
| Supercomputadora Frontier (referencia) | 1,102 exaFLOPS a 21 MW | [01](sources/01_smirnova_2023_organoid_intelligence.md) |
| Ventaja de eficiencia (cerebro completo vs. supercomputadora) | ~10⁶ | [01](sources/01_smirnova_2023_organoid_intelligence.md) |
| Organoide típico de investigación | <500 μm, <100.000 células | [01](sources/01_smirnova_2023_organoid_intelligence.md) |
| Meta de escalado (roadmap OI) | 10 millones de células/organoide | [01](sources/01_smirnova_2023_organoid_intelligence.md) |
| Precisión Brainoware (reconocimiento de voz, 8 hablantes) | 51% → 78% tras entrenamiento | [04](sources/04_brainoware_2023.md) |
| Aprendizaje DishBrain | detectable en 5 minutos de juego | [02](sources/02_kagan_2022_dishbrain_neuron.md) |
| Entrenamiento AlphaGo (comparación) | 160.000 partidas | [14](sources/14_orf_overview_ventajas_desafios.md) |
| CL1: precio / consumo / neuronas | USD 35.000 / 850-1.000 W (rack 30u) / 800.000 | [03](sources/03_cortical_labs_cl1.md) |
| Costo de montar un laboratorio SBI | USD 50.000 (básico) a +250.000 (alta densidad) | [16](sources/16_starting_sbi_lab_patterns_2025.md) |
| Datos generados por FinalSpark en 4 años | 18 TB, >20.000 millones de potenciales de acción | [05](sources/05_finalspark_neuroplatform_2024.md) |

---

## 6. Ventajas evidenciadas (con matiz de fortaleza de evidencia)

| Ventaja | Evidencia | Fortaleza |
|---|---|---|
| Eficiencia energética teórica del tejido biológico | Cerebro completo: 10⁶x vs. supercomputadora | **Fuerte pero mal aplicada** — compara cerebro completo (86.000M neuronas) contra organoides de <1M células; nadie midió esa proporción a escala de organoide real |
| Eficiencia de datos de entrenamiento | DishBrain aprende en 5 min; Brainoware llega a 78% con 240 clips | **Moderada** — tareas muy acotadas (Pong, clasificación de 8 hablantes), no comparable a tareas de IA de producción |
| Procesamiento de información "compleja"/ambigua | Argumento cualitativo (ORF) | **Débil como evidencia cuantificada** — no hay benchmark directo comparable |
| Ya existe interés comercial/inversión real | CL1 lanzado y a la venta; ronda de USD 10M | **Fuerte como hecho de mercado** — no implica que la tecnología sea superior, solo que hay apuesta financiera |

Fuentes: [01](sources/01_smirnova_2023_organoid_intelligence.md), [02](sources/02_kagan_2022_dishbrain_neuron.md), [04](sources/04_brainoware_2023.md), [14](sources/14_orf_overview_ventajas_desafios.md).

**Patrón transversal detectado:** *en las cuatro fuentes técnicas ([01], [04], [05], [16]) el mismo matiz se repite* — la eficiencia energética real se mide en el tejido biológico aislado, no en el sistema completo (soporte vital, electrónica, refrigeración, almacenamiento de datos). Es el punto más citable para cuestionar el argumento "a favor" más repetido en prensa.

---

## 7. Desventajas / limitaciones técnicas

1. **Límite físico de tamaño**: organoides avasculares, dependientes de difusión pasiva → núcleo necrótico a partir de ~300 μm. Es la barrera dura que explica por qué no existen organoides grandes y estables hoy. [01](sources/01_smirnova_2023_organoid_intelligence.md)
2. **Degradación con el tiempo**: la corriente mínima para generar respuesta aumenta con la edad del organoide (encapsulación glial); vida útil limitada a semanas/meses. [05](sources/05_finalspark_neuroplatform_2024.md), [03](sources/03_cortical_labs_cl1.md)
3. **Mismatch mecánico de interfaz**: organoides 3D esféricos sobre arrays de electrodos 2D rígidos — contacto limitado, resolución de señal comprometida. [04](sources/04_brainoware_2023.md), [14](sources/14_orf_overview_ventajas_desafios.md)
4. **Escalabilidad de infraestructura, no solo de biología**: FinalSpark solo pudo atender 7 de 32 grupos solicitantes; los algoritmos de plasticidad en paralelo (32 organoides a la vez) seguían "en desarrollo" a 2024. [05](sources/05_finalspark_neuroplatform_2024.md)
5. **Objeción de fondo (no solo de escala)**: según Tony Zador, "todavía no sabemos qué neuronas son importantes" para producir el comportamiento deseado — cuestiona si el enfoque es controlable/reproducible en principio, no solo si falta escalar. [12](sources/12_stat_news_2025_hype_backlash.md)
6. **Costo real de montaje**: USD 50.000–250.000+ de infraestructura, sin contar el costo del propio hardware comercial (CL1: USD 35.000). No es una tecnología "barata" hoy pese al argumento de eficiencia. [16](sources/16_starting_sbi_lab_patterns_2025.md)

---

## 8. Marco ético-legal-social: vigente vs. propuesto

**Lo que existe hoy (regulación real, no aspiracional):**
- EE.UU.: marco de supervisión de tres niveles (verde/amarillo/rojo) para quimeras y trasplantes neuronales, aplicado vía IRB/IACUC/ESCRO. [10](sources/10_national_academies_neural_organoids_chimeras.md)
- Comparación internacional: Reino Unido (revisión nacional para función "human-like"), Alemania (prohíbe trasplante a cerebro de grandes simios), Canadá (doble aprobación postnatal), Japón (flexibilizó en 2019 con comité nacional). [10](sources/10_national_academies_neural_organoids_chimeras.md)
- **Vacío regulatorio específico**: toda la regulación existente protege al *donante humano*; ninguna regula directamente al *organoide en sí* una vez creado, ni siquiera bajo el supuesto de que pudiera tener algún grado de sentiencia. Una propuesta del NIH en 2016 para supervisión reforzada de quimeras neuronales **nunca se finalizó**. [10](sources/10_national_academies_neural_organoids_chimeras.md)

**Lo que se propone pero no existe todavía:**
- Consenso internacional de supervisión vía OMS/ONU. [07](sources/07_johns_hopkins_elsi_2023.md)
- "Consentimiento dinámico" que permita a donantes gestionar permisos de forma continua. [07](sources/07_johns_hopkins_elsi_2023.md), [09](sources/09_consentimiento_donacion_organoides_2024.md)
- Marco de precaución inspirado en las 3R de bienestar animal (Reemplazo, Reducción, Refinamiento) aplicado a organoides. [09](sources/09_consentimiento_donacion_organoides_2024.md)

---

## 9. Mapa de posturas éticas para el debate

| Postura | Quién la sostiene | Argumento central | Fuente |
|---|---|---|---|
| **A favor con gobernanza** | Johns Hopkins (Smirnova, Hartung) | El potencial científico y médico justifica avanzar si se construye gobernanza en paralelo, no después | [01](sources/01_smirnova_2023_organoid_intelligence.md), [07](sources/07_johns_hopkins_elsi_2023.md) |
| **Cautela técnica desde adentro** | Pasca (Stanford), Zador (Cold Spring Harbor), Lancaster (Cambridge) | No es un rechazo ético sino una advertencia: el hype infundado puede generar un backlash regulatorio que dañe también la investigación médica legítima | [12](sources/12_stat_news_2025_hype_backlash.md) |
| **Precaución centrada en el organoide** | Bioética del consentimiento (varios autores) | El problema no es solo el donante humano — hay incertidumbre moral y epistemológica sobre el propio organoide que ningún consentimiento puede resolver del todo | [09](sources/09_consentimiento_donacion_organoides_2024.md), [08](sources/08_playing_brains_dishbrain_ethics_2023.md) |
| **Rechazo categórico** | Robert Hanna (filósofo) | Aunque el organoide nunca sea consciente, el uso mismo de la tecnología erosiona la autonomía y dignidad humanas ("neo-ludismo dignitario") | [13](sources/13_critica_filosofica_hanna_2023.md) |
| **Empírica / centrada en percepción pública** | Estudio Scientific Reports 2026 | Lo que mueve el apoyo público no es la evidencia técnica sino el encuadre (framing) de la pregunta — dato útil para cualquier bando, y para el propio formato del debate | [11](sources/11_percepcion_publica_2026.md) |

---

## 10. Inconsistencias / datos a verificar

- ⚠️ La cifra de "10⁶ veces más eficiente" se repite en casi todas las fuentes de marketing/divulgación ([01], [05], [14]) pero **siempre compara el cerebro completo, nunca un organoide real, contra una supercomputadora**. Ninguna fuente del corpus mide la eficiencia energética de un organoide de 100.000 células *incluyendo* su sistema de soporte vital completo contra un chip de tamaño equivalente.
- ⚠️ El texto completo de tres fuentes clave no pudo verificarse en esta sesión por paywall/bloqueo de bot: Kagan et al. 2022 ([02](sources/02_kagan_2022_dishbrain_neuron.md)), Milford/Shaw/Starke 2023 ([08](sources/08_playing_brains_dishbrain_ethics_2023.md)), Kataoka et al. 2024 ([15](sources/15_beyond_consciousness_elsi_2024.md)) y "Starting a SBI lab" ([16](sources/16_starting_sbi_lab_patterns_2025.md)). Las fichas se reconstruyeron con fuentes secundarias de alta fiabilidad, pero cualquier cita textual debería verificarse contra el PDF original antes de usarla como cita literal en el debate.
- ⚠️ No hay evidencia en el corpus de estudios de percepción pública fuera de EE.UU. — el hallazgo de [11](sources/11_percepcion_publica_2026.md) no debería generalizarse sin matiz a un público argentino/latinoamericano.

---

## 11. Preguntas abiertas / roadmap de investigación pendiente

1. ¿Existe cobertura o debate específico en medios/academia argentina o latinoamericana sobre este tema? (no investigado en esta sesión — oportunidad para dar un ángulo local al debate)
2. ¿Qué dice la CONEAU/CONICET o el marco de bioética argentino (Ley 26.529, comités de bioética de universidades) sobre investigación con organoides? (fuera de alcance de esta sesión, requiere investigación dedicada)
3. Verificar cita textual exacta del argumento de Milford/Shaw/Starke sobre sufrimiento vía principio de energía libre contra el PDF original.
4. Profundizar en la postura intermedia (ninguna fuente del corpus la desarrolla del todo): ¿es posible un marco de "estatus moral incierto pero no nulo", análogo al de animales de investigación, aplicado específicamente a organoides usados para IA?

---

## 12. Índice de fuentes

Ver [`sources/`](sources/) — 21 fuentes documentadas, numeradas 01-21. Índice temático:

- **Técnico/fundacional (biocomputación):** [01](sources/01_smirnova_2023_organoid_intelligence.md), [02](sources/02_kagan_2022_dishbrain_neuron.md), [03](sources/03_cortical_labs_cl1.md), [04](sources/04_brainoware_2023.md), [05](sources/05_finalspark_neuroplatform_2024.md), [06](sources/06_oi_workshop_baltimore_declaration_2022.md), [16](sources/16_starting_sbi_lab_patterns_2025.md)
- **Ético/legal/social:** [07](sources/07_johns_hopkins_elsi_2023.md), [08](sources/08_playing_brains_dishbrain_ethics_2023.md), [09](sources/09_consentimiento_donacion_organoides_2024.md), [10](sources/10_national_academies_neural_organoids_chimeras.md), [13](sources/13_critica_filosofica_hanna_2023.md), [15](sources/15_beyond_consciousness_elsi_2024.md)
- **Percepción pública / crítica interna:** [11](sources/11_percepcion_publica_2026.md), [12](sources/12_stat_news_2025_hype_backlash.md)
- **Síntesis/divulgación:** [14](sources/14_orf_overview_ventajas_desafios.md)
- **Paradigmas de entrenamiento y consciencia (eje pedagógico, ver [analisis/03](analisis/03_entrenamiento_comparado_y_el_debate_de_la_conciencia.md)):** [17](sources/17_reinforcement_learning_basics.md) (RL), [18](sources/18_operant_conditioning_skinner.md) (condicionamiento operante), [19](sources/19_reward_is_enough_2021.md) / [20](sources/20_scalar_reward_not_enough_2022.md) (¿alcanza la recompensa para explicar toda la inteligencia?), [21](sources/21_hard_problem_consciousness_chalmers.md) (el problema difícil de la consciencia)
- **Carrera de la IA de silicio y su gobernanza (bloques 6-7 de [entregables/05](entregables/05_guia_presentacion_grupal.md)):** [22](sources/22_amodei_pacing_frontier_2026.md) (Amodei, "pacear la frontera", 2026), [23](sources/23_altman_congress_testimony_2023.md) (Altman ante el Congreso, 2023), [24](sources/24_pause_giant_ai_experiments_2023.md) (carta de pausa de FLI, 2023, incumplida), [25](sources/25_metr_time_horizon_2025.md) (aceleración de capacidades medida por METR)
- **De la mosca a la ficción (bloques 8-9 de [entregables/05](entregables/05_guia_presentacion_grupal.md), ver [analisis/04](analisis/04_de_la_mosca_a_la_ficcion_ciencia_real_vs_especulacion.md)):** [26](sources/26_flywire_connectome_2024.md) (conectoma completo de la mosca), [27](sources/27_virtual_fly_brain_simulation_2024.md) (simulación virtual del cerebro de la mosca), [28](sources/28_whole_brain_emulation_feasibility.md) (escala real: mosca vs. ratón vs. humano), [29](sources/29_i_have_no_mouth_ellison_1967.md) (referencia literaria — ficción, no ciencia)

## 13. Glosario

Ver [`GLOSARIO.md`](GLOSARIO.md).
