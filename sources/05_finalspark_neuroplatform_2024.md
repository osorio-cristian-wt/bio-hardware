# Open and remotely accessible Neuroplatform for research in wetware computing (FinalSpark)

- **URL:** https://pmc.ncbi.nlm.nih.gov/articles/PMC11097343/
- **URL secundaria:** https://finalspark.com/neuroplatform/
- **Fecha de consulta:** 2026-09-13
- **Tipo:** académico (*Frontiers in Artificial Intelligence*, 2024) + información comercial de la empresa

## Resumen del contenido

FinalSpark (Suiza) publica la arquitectura de su **Neuroplatform**: la primera plataforma online que da acceso remoto y pago a neuronas biológicas humanas in vitro ("wetware computing"). Ofrece suscripción académica a USD 500/usuario/mes.

## Información clave

**Arquitectura técnica:**
- 4 Multi-Electrode Arrays (MEAs), cada uno con 4 organoides y 8 electrodos por organoide (32 electrodos totales).
- Organoides de prosencéfalo (Forebrain Organoids) derivados de células madre neurales iPSC humanas, ~500 μm de diámetro.
- Sistema de microfluídica en circuito cerrado (15 μL/min), recambio automático de medio cada 24h, interfaz aire-líquido.
- Registro/estimulación: cabezales Intan RHS 32, muestreo a 30 kHz / 16-bit (precisión 0,15 μV); estimulación de 10 nA a 2,5 mA.
- Sistema de "uncaging" molecular por UV (365 nm) para liberar dopamina, glutamato, NMDA de forma controlada.

**Datos operativos (a 2024):**
- Vida útil de organoide: hasta 100+ días (inicialmente solo horas al inicio del proyecto).
- 1.000+ organoides probados en 4 años; 250+ reemplazos.
- 18 terabytes de datos acumulados; >20.000 millones de potenciales de acción individuales registrados.
- 8 de 36 grupos académicos solicitantes fueron admitidos (capacidad actual: 7 grupos).

## Relevancia para el debate

Es el caso más citado del argumento de **eficiencia energética como ventaja comercial explícita**: FinalSpark declara que sus bioprocesadores "consumen un millón de veces menos energía que los procesadores digitales tradicionales" — la cifra que replican Yahoo, Tom's Hardware y BioSpace en sus titulares.

## Implicancias tecnológicas

**Limitaciones reconocidas:**
- Un solo protocolo de diferenciación para generar organoides (poca diversidad de tipos celulares).
- Los algoritmos de circuito cerrado para plasticidad hoy corren en **un solo organoide** — la ejecución paralela en los 32 está "en desarrollo", no operativa.
- La corriente mínima necesaria para generar un spike **aumenta con la edad del organoide** (vinculado a encapsulación glial y cambios de impedancia) — el sistema se degrada con el tiempo, no es estable indefinidamente.
- Solo 7 de 32 grupos solicitantes pudieron ser atendidos por límite de infraestructura — la escalabilidad real es baja.

## Citas relevantes

> "Over the past three years, the Neuroplatform was utilized with over 1,000 brain organoids, enabling the collection of more than 18 terabytes of data."

> "Given these conditions, the prospect of replacing ANNs running on digital computers with real BNNs is enticing."

## Observaciones

El claim de "millón de veces menos energía" (repetido en la prensa comercial) mide el organoide aislado, no el sistema completo con incubadoras, control ambiental (CO₂/O₂/humedad/presión/temperatura) y electrónica de registro — el mismo matiz que en [01](01_smirnova_2023_organoid_intelligence.md) y [03](03_cortical_labs_cl1.md). Es un patrón transversal a documentar en `research.md`.
