# Análisis — Ventajas y desventajas técnicas de usar neuronas humanas como hardware de IA

> Evalúa críticamente las afirmaciones de [`research.md` §6-7](../research.md#6-ventajas-evidenciadas-con-matiz-de-fortaleza-de-evidencia) contrastando el argumento de marketing contra la evidencia real.
>
> **Fecha:** 2026-09-13

---

## 0. TL;DR

El campo tiene **evidencia técnica real pero acotada** (DishBrain, Brainoware) de que un cultivo de neuronas puede aprender o computar tareas simples con menos datos de entrenamiento que un modelo de IA convencional. El argumento de **eficiencia energética masiva (10⁶x) es retóricamente poderoso pero está mal aplicado**: compara el cerebro humano completo contra una supercomputadora, no un organoide real de laboratorio contra un chip equivalente — y cuando se mide el sistema completo (organoide + soporte vital + electrónica), la ventaja se reduce drásticamente o desaparece. La tecnología hoy es **cara de montar** (USD 50.000-250.000+ de infraestructura), **frágil** (vida útil de semanas a meses, degradación progresiva) y **no reproducible a gran escala** (ningún grupo logró aún operar decenas de organoides en paralelo de forma rutinaria). Para un debate: es legítimo argumentar que existe potencial real, pero no es legítimo argumentar que ya es una alternativa viable y probada a la IA de silicio.

## 1. Encuadre del problema

La pregunta técnica que importa para el debate no es "¿puede una neurona computar?" (sí, evidenciado) sino **"¿es esto una alternativa de hardware de IA viable hoy, o una promesa de investigación básica vendida como producto?"**. Separar ambas preguntas evita que el debate colapse en una sola dirección por confundir "demostrado en laboratorio" con "escalable y desplegable".

## 2. Qué sí está demostrado

| Afirmación | Evidencia | Fuente |
|---|---|---|
| Un cultivo de neuronas puede aprender una tarea goal-directed en tiempo real | DishBrain aprende Pong en 5 min, con condición control que no aprende | [02](../sources/02_kagan_2022_dishbrain_neuron.md) |
| Un organoide puede usarse como reservorio de cómputo para clasificación | Brainoware: 51%→78% en reconocimiento de vocales japonesas tras entrenamiento; el control sin organoide da puntaje nulo | [04](../sources/04_brainoware_2023.md) |
| Existe un mercado dispuesto a pagar por esto | CL1 a la venta (USD 35.000); Neuroplatform con suscriptores académicos pagos | [03](../sources/03_cortical_labs_cl1.md), [05](../sources/05_finalspark_neuroplatform_2024.md) |

## 3. Qué NO está demostrado (y se presenta como si lo estuviera)

1. **Eficiencia energética del sistema completo.** Ninguna fuente del corpus mide vatios/tarea de un organoide *con* su infraestructura de soporte (incubadora, control ambiental, electrónica de registro, microfluídica) contra un chip digital haciendo la misma tarea. El propio dato de Cortical Labs (rack de 30 unidades CL1: 850-1.000 W) ya es comparable al consumo de un servidor GPU de gama media — la ventaja "millón de veces" no sobrevive a esa comparación real. Ver [03](../sources/03_cortical_labs_cl1.md), [05](../sources/05_finalspark_neuroplatform_2024.md).
2. **Escalabilidad reproducible.** FinalSpark solo pudo atender 7 de 32 grupos solicitantes; el cómputo paralelo en sus 32 organoides seguía "en desarrollo" en 2024. [05](../sources/05_finalspark_neuroplatform_2024.md)
3. **Control mecanístico del sistema.** Según Tony Zador (Cold Spring Harbor), "todavía no sabemos qué neuronas son importantes" para producir el comportamiento deseado — una objeción a la *previsibilidad* del enfoque, no solo a su escala actual. [12](../sources/12_stat_news_2025_hype_backlash.md)
4. **Superioridad frente a tareas de IA reales.** Las demostraciones (Pong, clasificación de 8 hablantes) son juguetes de laboratorio (*toy problems*), órdenes de magnitud más simples que cualquier tarea de producción (visión por computadora a escala, LLMs, etc.). No existe ningún benchmark del corpus que compare directamente un organoide contra un modelo de IA de producción en la misma tarea.

## 4. Capacidades / restricciones físicas duras

- **Límite de tamaño por difusión pasiva:** organoides sin vascularización necrosan el núcleo a partir de ~300 μm — es una barrera de biología básica, no de ingeniería, y no tiene solución conocida a corto plazo. [01](../sources/01_smirnova_2023_organoid_intelligence.md)
- **Degradación temporal:** la impedancia y la corriente mínima necesaria para generar respuesta aumentan con la edad del organoide (encapsulación glial) — el sistema *envejece* y pierde sensibilidad, algo que un chip de silicio no hace. [05](../sources/05_finalspark_neuroplatform_2024.md)
- **Interfaz mecánica imperfecta:** contacto limitado entre estructuras 3D esféricas y arrays de electrodos rígidos 2D — pérdida de señal estructural. [04](../sources/04_brainoware_2023.md)

## 5. Comparación de costos (dato poco citado en la cobertura mediática)

| Ítem | Costo |
|---|---|
| Infraestructura básica de laboratorio SBI | USD 50.000+ |
| Infraestructura de alta densidad / inalámbrica | USD 250.000+ |
| Arrays de electrodos de reemplazo | USD 500–2.000 c/u |
| Unidad CL1 comercial | USD 35.000 |
| Suscripción Neuroplatform | USD 500/usuario/mes |

Fuente: [16](../sources/16_starting_sbi_lab_patterns_2025.md), [03](../sources/03_cortical_labs_cl1.md), [05](../sources/05_finalspark_neuroplatform_2024.md).

**Conclusión de costos:** contradice el argumento implícito de "esto va a ser más barato" — hoy es una tecnología de nicho, cara de operar, con costos recurrentes (reemplazo de arrays, mantenimiento de cultivo) que un chip de silicio no tiene una vez fabricado.

## 6. Riesgos técnicos de proyecto (no éticos)

| Riesgo | Probabilidad | Impacto | Nota |
|---|---|---|---|
| Contaminación/pérdida del cultivo | Alta (biología viva) | Medio — hay que reponer el organoide | Costo recurrente, no solo riesgo puntual |
| Sobre-promesa dañando credibilidad del campo | Media-alta (ya en curso) | Alto — puede frenar también investigación médica legítima con organoides | Ver [12](../sources/12_stat_news_2025_hype_backlash.md) |
| Imposibilidad de escalar el enfoque más allá de tareas de juguete | Desconocida — es la objeción de Zador | Alto si se confirma | No hay forma de descartarla con la evidencia actual |

## 7. Métricas que un debate riguroso debería exigir (y hoy no existen publicadas)

- Vatios por inferencia/tarea del **sistema completo** (no solo el tejido).
- Tasa de fallo/reemplazo de organoides por semana de operación continua.
- Comparación directa organoide-vs-red-neuronal-artificial en la *misma* tarea, mismo dataset, mismas condiciones de evaluación.

## 8. Ficheros relacionados

[research.md §6-7](../research.md), [03](../sources/03_cortical_labs_cl1.md), [04](../sources/04_brainoware_2023.md), [05](../sources/05_finalspark_neuroplatform_2024.md), [12](../sources/12_stat_news_2025_hype_backlash.md), [16](../sources/16_starting_sbi_lab_patterns_2025.md).
