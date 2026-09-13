# Reinforcement Learning: cómo aprende una IA por prueba y error

- **URL:** https://aws.amazon.com/what-is/reinforcement-learning/
- **URL secundaria:** https://wandb.ai/site/articles/reinforcement-learning-a-guide-to-ais-interactive-learning-paradigm/
- **Fecha de consulta:** 2026-09-13
- **Tipo:** técnico (divulgación consolidada de múltiples fuentes de referencia — AWS, Weights & Biases)

## Resumen del contenido

Explica el paradigma de **aprendizaje por refuerzo (RL)**, la forma de entrenar IA más parecida estructuralmente al condicionamiento operante humano ([18](18_operant_conditioning_skinner.md)) y al mecanismo de DishBrain ([02](02_kagan_2022_dishbrain_neuron.md)): un agente aprende por prueba y error a partir de una **señal de recompensa**, no por ejemplos etiquetados (como el aprendizaje supervisado clásico).

## Información clave

**El ciclo de RL (4 pasos, se repite):**
1. El agente observa el estado actual del entorno.
2. Elige una acción.
3. Recibe una **señal de recompensa** que cuantifica qué tan buena fue esa acción (positiva o negativa).
4. Usa esa señal para ajustar su política de decisión, y el ciclo se repite.

**Objetivo del agente:** maximizar la recompensa acumulada esperada a lo largo del tiempo — no la recompensa inmediata. Esto genera el problema clásico de **exploración vs. explotación**: probar acciones nuevas (exploración) vs. usar lo que ya sabe que funciona (explotación).

**Diferencia clave con el aprendizaje supervisado:** en RL nadie le dice al agente "la respuesta correcta era X" — solo recibe una señal de qué tan bien o mal le fue, igual que un organismo biológico no recibe un manual de instrucciones, solo consecuencias.

## Relevancia para el debate

Es el eslabón que permite comparar, en el mismo lenguaje formal, tres sistemas muy distintos: una IA convencional entrenada por RL, un humano aprendiendo por condicionamiento operante, y un organoide (DishBrain) aprendiendo por el principio de energía libre. **Los tres comparten la misma estructura abstracta: acción → consecuencia → ajuste de comportamiento** — solo cambia el sustrato físico que hace el ajuste (pesos numéricos, sinapsis humanas, o conexiones de un cultivo de neuronas).

## Implicancias tecnológicas

La "recompensa" en RL es, en la práctica, un número que un ingeniero diseña de antemano (la "función de recompensa") — es una elección de diseño humana, no algo que el agente descubre por sí mismo. Este matiz importa para el debate: la analogía con el aprendizaje humano/biológico no es perfecta, porque nadie "programa" la función de recompensa de un bebé o de un organoide de la misma manera explícita.

## Citas relevantes

> "RL agents are trained by iteratively acting in their environment under the guidance of a reward signal: after observing the current state, agents choose an action, receive feedback that quantifies the quality of their course of action, then use this feedback to tune their current policy, and the cycle repeats."

## Observaciones

Fuente de divulgación técnica consolidada (no un único paper), elegida porque el objetivo de esta ficha es fijar el vocabulario básico de RL para la comparación pedagógica del análisis 03, no aportar un dato de investigación original.
