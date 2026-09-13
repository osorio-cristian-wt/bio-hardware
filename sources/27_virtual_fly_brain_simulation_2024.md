# De la mosca real a la mosca virtual: la simulación del cerebro completo corre en una laptop (Shiu et al., Nature, oct. 2024)

- **URL:** https://news.berkeley.edu/2024/10/02/researchers-simulate-an-entire-fly-brain-on-a-laptop-is-a-human-brain-next/
- **Fecha de consulta:** 2026-09-13
- **Tipo:** académico (*Nature*, 2/10/2024, equipo liderado por Phil Shiu, UC Berkeley) — ficha basada en cobertura institucional de la propia universidad

## Resumen del contenido

Usando el conectoma completo de FlyWire ([26](26_flywire_connectome_2024.md)), un equipo liderado por Phil Shiu (entonces postdoc en UC Berkeley, hoy en la startup Eon AI) construyó un **modelo computacional del cerebro completo de la mosca** que corre en una laptop común, y predijo correctamente cómo respondería el cerebro real ante distintos estímulos.

## Información clave

**Cómo se construyó:** las 139.255 neuronas y 50 millones de conexiones del conectoma se tradujeron a un modelo de simulación neuronal (tipo "leaky integrate-and-fire"), asignando a cada neurona una identidad de neurotransmisor (excitatoria/colinérgica, inhibitoria/GABAérgica o glutamatérgica, más dopaminérgica, octopaminérgica y serotoninérgica) a partir de predicciones previas a gran escala.

**Comportamientos que reprodujo correctamente:**
- **Alimentación:** al estimular neuronas de sabor dulce, el modelo predijo correctamente la activación de neuronas motoras para extender la probóscide (la "trompa" de la mosca) y comer.
- **Acicalamiento (grooming):** al estimular sensores de las antenas, predijo la activación de neuronas motoras de las patas para acicalarse.
- **Discriminación de sabor:** mostró cómo neuronas inhibitorias del sabor amargo pueden bloquear la respuesta de comer azúcar.

**Extensión embebida:** más allá del paper original, el mismo modelo se conectó a una simulación de física para controlar un **cuerpo virtual** — la mosca simulada "ve" su entorno, sus circuitos neuronales procesan la señal, las neuronas motoras se activan, y el cuerpo virtual se mueve, generando nuevo input sensorial en un bucle cerrado (igual estructura de circuito cerrado que DishBrain, [02](02_kagan_2022_dishbrain_neuron.md) — pero acá todo el "cerebro" es digital, no biológico).

**La frase que abre la puerta al siguiente paso (cita textual del propio investigador):** "The next goal is a connectome of the mouse brain; the ultimate prize, the wiring matrix of a human brain."

**Limitación reconocida explícitamente por el propio Shiu:** "We essentially ignore all of the different morphologies of individual neurons and assume all excitatory or inhibitory neurons work the same, which we know isn't the case." — el modelo es una simplificación deliberada, no una réplica perfecta.

## Relevancia para la presentación

Es la pieza central del giro narrativo hacia la ficción: **el propio científico que lideró el proyecto dice, en una entrevista real, que el "premio final" es mapear un cerebro humano.** No hace falta que la presentación invente esa aspiración — ya está dicha, en público, por quien hizo el trabajo. A partir de esta cita es donde la presentación puede pasar legítimamente del terreno científico al terreno especulativo/ficcional (ver [analisis/04](../analisis/04_de_la_mosca_a_la_ficcion_ciencia_real_vs_especulacion.md)).

## Implicancias tecnológicas

El modelo demuestra que **la sola estructura del conectoma, sin necesitar simular cada detalle biofísico de cada neurona, alcanza para predecir comportamiento real** con sorprendente precisión — un dato fuerte a favor de que la información relevante de "cómo piensa" un cerebro podría estar mayormente en su cableado, no solo en los detalles bioquímicos de cada célula. Es, con las diferencias de escala obvias, el mismo argumento de fondo que hace plausible (a nivel de discusión, no de demostración) la idea de "subir una mente" en ciencia ficción.

## Citas relevantes

> "The next goal is a connectome of the mouse brain; the ultimate prize, the wiring matrix of a human brain." — Phil Shiu

> "We essentially ignore all of the different morphologies of individual neurons and assume all excitatory or inhibitory neurons work the same, which we know isn't the case." — Phil Shiu

## Observaciones

Ficha reconstruida a partir de la cobertura institucional de UC Berkeley (fuente secundaria de alta fiabilidad, con cita directa del investigador), dado que el acceso directo a *Nature* no se verificó en esta sesión. Verificar el DOI exacto del paper antes de citarlo en un contexto formal/académico (no solo de presentación).
