# Guía de debate — ¿Deberíamos usar neuronas humanas como hardware de inteligencia artificial?

> Documento de uso directo para preparar y moderar el debate. Se apoya en [`research.md`](../research.md) y en los análisis de [`analisis/`](../analisis/). Cada argumento cita su fuente en `sources/` para poder defenderlo si lo cuestionan en vivo.
>
> **Fecha:** 2026-09-13

---

## 1. Moción sugerida

> **"Este foro considera que el desarrollo de 'organoid intelligence' / biocomputación con neuronas humanas debería continuar sin restricciones adicionales a las ya existentes."**

Alternativa más acotada si se quiere un debate más técnico:
> **"El argumento de eficiencia energética es suficiente para justificar la inversión actual en biocomputación con neuronas humanas."**

## 2. Definiciones a acordar antes de empezar (evita discutir con definiciones distintas)

Leer en voz alta al inicio — están desarrolladas en [`GLOSARIO.md`](../GLOSARIO.md):

- **Organoid Intelligence / Synthetic Biological Intelligence / wetware computing** → mismo fenómeno base, tres nombres de tres actores distintos (academia, Cortical Labs, FinalSpark).
- **Organoide cerebral**: cultivo 3D de neuronas derivadas de células madre, del tamaño de la punta de una aguja (no un "mini-cerebro" con anatomía completa).
- **Sentiencia / estatus moral**: distinguir explícitamente "¿procesa información?" (sí, demostrado) de "¿tiene experiencia subjetiva?" (no resuelto científicamente).

## 3. Resumen ejecutivo (1 minuto)

Desde 2022 existe evidencia real de que cultivos de neuronas humanas pueden aprender tareas simples (DishBrain, *Neuron* 2022) y funcionar como sustrato de cómputo (Brainoware, *Nature Electronics* 2023). En 2025 esto pasó de laboratorio a producto comercial: Cortical Labs vende el CL1 (USD 35.000) y FinalSpark alquila acceso remoto a organoides vivos. El argumento de venta central es la eficiencia energética (hasta un millón de veces menos consumo que el cómputo digital), pero esa cifra compara el cerebro humano *completo* contra una supercomputadora — no un organoide real contra un chip equivalente — y no existe hoy ninguna medición pública que incluya el sistema de soporte completo. En paralelo, la propia comunidad científica (Stanford, Cold Spring Harbor, Cambridge) advirtió en 2025 que el exceso de promesas podría generar un backlash regulatorio dañino. El marco ético-legal actual protege al donante humano pero no regula directamente al organoide, y coexisten al menos cinco posturas éticas distintas —no un simple "sí o no"— sobre si esto debería continuar y bajo qué condiciones.

---

## 4. Argumentos A FAVOR (con evidencia citable)

| # | Argumento | Evidencia | Fuente | Fuerza |
|---|---|---|---|---|
| 1 | Ya hay evidencia experimental de aprendizaje biológico goal-directed en tiempo real | DishBrain aprende Pong en 5 min | [02](../sources/02_kagan_2022_dishbrain_neuron.md) | Fuerte (hecho verificado) |
| 2 | Un organoide puede funcionar como sustrato de cómputo real, no solo teórico | Brainoware: 51%→78% en clasificación de voz | [04](../sources/04_brainoware_2023.md) | Fuerte (hecho verificado) |
| 3 | El potencial de eficiencia energética del cerebro biológico es real y medible en principio | Cerebro completo: ~1 exaFLOPS a 10-20W vs. 21MW de una supercomputadora | [01](../sources/01_smirnova_2023_organoid_intelligence.md) | Moderada — válida como *potencial*, no como logro actual (ver réplica) |
| 4 | La comunidad científica construyó gobernanza ética desde el inicio, no como reacción tardía | Baltimore Declaration (2022) incluyó ejes éticos desde el primer workshop | [06](../sources/06_oi_workshop_baltimore_declaration_2022.md), [07](../sources/07_johns_hopkins_elsi_2023.md) | Moderada |
| 5 | Hay valor médico independiente del uso computacional (modelado de enfermedades, toxicología) que se perdería con una moratoria total | Lancaster defiende explícitamente separar ambos usos | [12](../sources/12_stat_news_2025_hype_backlash.md) | Fuerte para argumentar en contra de una prohibición total, no para defender el uso computacional en sí |

## 5. Argumentos EN CONTRA (con evidencia citable)

| # | Argumento | Evidencia | Fuente | Fuerza |
|---|---|---|---|---|
| 1 | El argumento de eficiencia energética no está demostrado a la escala real del producto | CL1 (rack 30 unidades): 850-1.000 W — comparable a un servidor GPU convencional | [03](../sources/03_cortical_labs_cl1.md) | Fuerte (contradicción numérica directa) |
| 2 | El consentimiento del donante no puede ser plenamente informado por incertidumbre científica y moral genuina | "Doble incertidumbre" epistemológica + moral | [09](../sources/09_consentimiento_donacion_organoides_2024.md) | Fuerte |
| 3 | Existe un vacío regulatorio real: nada regula al organoide en sí, solo al donante | Propuesta NIH 2016 nunca finalizada | [10](../sources/10_national_academies_neural_organoids_chimeras.md) | Fuerte (hecho verificado) |
| 4 | El propio diseño experimental podría generar sufrimiento como efecto colateral no buscado | Argumento vía principio de energía libre | [08](../sources/08_playing_brains_dishbrain_ethics_2023.md) | Moderada (teórica, no verificada empíricamente) |
| 5 | Aunque el organoide no sufra, el uso de la tecnología puede erosionar la autonomía humana | Argumento de "neo-ludismo dignitario" (Hanna) | [13](../sources/13_critica_filosofica_hanna_2023.md) | Filosófica — fuerte como postura, débil como evidencia empírica |
| 6 | Incluso científicos del propio campo dudan de la viabilidad técnica del enfoque | "Todavía no sabemos qué neuronas son importantes" (Zador) | [12](../sources/12_stat_news_2025_hype_backlash.md) | Fuerte — viene de un experto interno, no de un crítico externo |

---

## 6. Réplicas cruzadas anticipadas

**Si A FAVOR usa el argumento de eficiencia energética (arg. 3):**
→ EN CONTRA responde con arg. 1 (cifra real del CL1) y señala que en [research.md §6](../research.md#6-ventajas-evidenciadas-con-matiz-de-fortaleza-de-evidencia) el propio corpus documenta que esa comparación mide el cerebro completo, no el producto real.

**Si EN CONTRA usa el argumento de sufrimiento (arg. 4):**
→ A FAVOR puede responder que el principio de energía libre es un marco funcional/matemático de cómputo, no una prueba de experiencia subjetiva, y que ningún paper del corpus afirma consenso científico sobre sentiencia en organoides — ver matiz en [07](../sources/07_johns_hopkins_elsi_2023.md) ("estatus moral incierto", no afirmado ni descartado).

**Si A FAVOR usa "ya hay gobernanza construida" (arg. 4):**
→ EN CONTRA responde con arg. 3: la gobernanza propuesta (consenso OMS/ONU, consentimiento dinámico) **no existe todavía como norma vigente** — es una recomendación académica, no regulación real ([07](../sources/07_johns_hopkins_elsi_2023.md) vs. [10](../sources/10_national_academies_neural_organoids_chimeras.md)).

**Si EN CONTRA pide prohibición total:**
→ A FAVOR responde con arg. 5: eso frenaría también investigación médica no-computacional (modelado de enfermedades, toxicología) que no depende de las objeciones específicas al uso como hardware de IA — cita a Lancaster, [12](../sources/12_stat_news_2025_hype_backlash.md).

---

## 7. Preguntas difíciles para el moderador (una por eje, ver [analisis/02](../analisis/02_posturas_eticas_mapa_debate.md))

1. *A favor:* "Si mañana se publicara evidencia de que un organoide tiene alguna forma de experiencia displacentera, ¿seguirían defendiendo la investigación computacional con el mismo entusiasmo?"
2. *En contra:* "¿Su objeción es al bienestar del organoide, a la validez del consentimiento del donante, o a lo que le hace esto a la sociedad humana que lo usa? Son tres objeciones distintas — ¿cuál sostienen?"
3. *A ambos:* "¿Separarían la investigación médica con organoides (modelado de enfermedades) de su uso específico como hardware de cómputo? ¿Por qué sí o por qué no?"
4. *A ambos:* "Si la única barrera fuera el consentimiento del donante y se resolviera con un protocolo perfecto de consentimiento específico e informado, ¿cambiaría su postura?"

---

## 8. Citas listas para usar en vivo

> "The human brain, with its complex three-dimensional network of cells and synapses, inspires the development of AI hardware due to its energy efficiency." — paper de Brainoware, [04](../sources/04_brainoware_2023.md)

> "we still don't understand which neurons are important" — Tony Zador (Cold Spring Harbor), [12](../sources/12_stat_news_2025_hype_backlash.md)

> "Consent should not be used as an 'ethics-wash' for deeply controversial research." — [09](../sources/09_consentimiento_donacion_organoides_2024.md)

> "an all-out existential attack on our human dignity" — Robert Hanna, [13](../sources/13_critica_filosofica_hanna_2023.md)

> "More transparency and assurances could be warranted. Donors might wish to deny the use of their stem cells for the creation of, say, human–animal chimaeras." — National Academies, [10](../sources/10_national_academies_neural_organoids_chimeras.md)

---

## 9. Qué NO decir en el debate (errores frecuentes en cobertura mediática, ya detectados en el corpus)

- ❌ No afirmar que "los organoides ya reconocen voz como Alexa/Siri" — Brainoware distingue 8 hablantes en un set cerrado de 240 clips, no reconocimiento de voz abierto. [04](../sources/04_brainoware_2023.md)
- ❌ No repetir "un millón de veces más eficiente" sin aclarar que es una comparación del cerebro completo, no de un organoide de laboratorio. [01](../sources/01_smirnova_2023_organoid_intelligence.md)
- ❌ No decir "esto no está regulado" en términos absolutos — sí hay un marco de tres niveles vigente en EE.UU. para quimeras y trasplantes; lo que falta es regulación específica del organoide-como-tal, no ausencia total de regulación. [10](../sources/10_national_academies_neural_organoids_chimeras.md)
- ❌ No asumir que el hallazgo de percepción pública ([11](../sources/11_percepcion_publica_2026.md)) aplica igual fuera de EE.UU. — es el único estudio empírico del corpus y es local a un país.

## 10. Ficheros relacionados

[research.md](../research.md) (síntesis completa) · [analisis/01](../analisis/01_ventajas_y_desventajas_tecnicas.md) (ventajas/desventajas técnicas) · [analisis/02](../analisis/02_posturas_eticas_mapa_debate.md) (mapa ético detallado) · [GLOSARIO.md](../GLOSARIO.md)
