# Starting a synthetic biological intelligence lab from scratch

- **URL:** https://www.cell.com/patterns/fulltext/S2666-3899(25)00080-7
- **URL secundaria:** https://www.researchgate.net/publication/391065182_Starting_a_synthetic_biological_intelligence_lab_from_scratch
- **Fecha de consulta:** 2026-09-13
- **Tipo:** académico (*Patterns*/Cell Press, 2025) — texto completo con paywall, ficha basada en metadatos y resumen de búsqueda

## Resumen del contenido

Guía práctica ("tutorial") dirigida a laboratorios que quieran empezar a trabajar en Synthetic Biological Intelligence (SBI): cultivo neuronal, interfaz electrofisiológica, costos de montaje y estrategias de mitigación de riesgo. Es la fuente más orientada a "qué hace falta en la práctica para hacer esto", en vez de resultados o promesas.

## Información clave

**Costos de equipamiento (rango de mercado):**
| Tipo de sistema | Costo estimado |
|---|---|
| Sistema in vitro básico | desde USD 50.000 |
| Sistema in vivo de alta densidad o inalámbrico | más de USD 250.000 |
| Arrays de electrodos de reemplazo | USD 500–2.000 c/u |

**Arquitectura de interfaz típica:** array de microelectrodos (MEA) para embeber neuronas vivas en tareas virtuales, con FPGA como puente entre la placa del MEA y la computadora host, a menudo con chips ASIC dedicados para manejar la electrofisiología.

**Costos operativos recurrentes:** reemplazo de arrays y almacenamiento de datos (los volúmenes generados son sustanciales — coherente con los 18 TB reportados por FinalSpark en 4 años, ver [05](05_finalspark_neuroplatform_2024.md)).

## Relevancia para el debate

Aporta el dato que falta en la mayoría de la cobertura mediática: **cuánto cuesta realmente montar esto**, más allá del precio de venta del producto terminado (CL1: USD 35.000, [03](03_cortical_labs_cl1.md)). Es útil para el argumento de "esto no es accesible ni barato hoy, pese al discurso de eficiencia".

## Implicancias tecnológicas

Confirma que el ecosistema (FPGA + MEA + ASIC + almacenamiento de datos) es la parte cara y compleja del sistema — el "reservorio" biológico en sí puede ser barato de mantener, pero la infraestructura de interfaz no lo es. Mismo patrón señalado en [01](01_smirnova_2023_organoid_intelligence.md), [04](04_brainoware_2023.md) y [05](05_finalspark_neuroplatform_2024.md): la eficiencia energética del organoide no equivale a eficiencia de costo total del sistema.

## Citas relevantes

*(Texto completo bloqueado por paywall en esta sesión — no se pudieron extraer citas textuales verificadas.)*

## Observaciones

⚠️ Ficha basada en resumen de búsqueda, no en el PDF completo (403 en cell.com). Los números de costo son consistentes entre dos fuentes independientes de búsqueda, lo que da confianza razonable, pero deberían verificarse contra el PDF si se citan como cifra exacta en el debate.
