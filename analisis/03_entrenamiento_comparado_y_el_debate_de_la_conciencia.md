# Análisis — Cómo se entrena una IA, cómo aprendemos nosotros, y qué dispara eso sobre la pregunta de la consciencia

> Es el análisis que sostiene el nuevo eje central de la presentación (ver [`entregables/02`](../entregables/02_guia_presentacion_15min.md)): en vez de partir de "ventajas técnicas vs. desventajas técnicas", parte de una comparación pedagógica de **tres formas de aprender** para llegar a una pregunta filosófica abierta, no a un veredicto.
>
> **Fecha:** 2026-09-13

---

## 0. TL;DR

Una IA convencional entrenada por aprendizaje por refuerzo, un bebé humano aprendiendo por condicionamiento operante (el caramelo), y un organoide tipo DishBrain aprendiendo por el principio de energía libre **comparten la misma estructura formal**: una conducta, seguida de una consecuencia (favorable o desfavorable), que aumenta o disminuye la probabilidad de que esa conducta se repita. Esto no es una coincidencia retórica — está documentado en tres tradiciones científicas independientes ([17](../sources/17_reinforcement_learning_basics.md), [18](../sources/18_operant_conditioning_skinner.md), [02](../sources/02_kagan_2022_dishbrain_neuron.md)). La pregunta que esa simetría dispara —y que ninguna de las tres tradiciones puede responder por sí sola— es si compartir el mismo mecanismo de *ajuste de conducta* implica compartir también **experiencia subjetiva**. La filosofía llama a esto el "problema difícil de la consciencia" ([21](../sources/21_hard_problem_consciousness_chalmers.md)) y no tiene una respuesta de consenso — ni siquiera un laboratorio de IA de primer nivel que apostó fuerte por la hipótesis de que "la recompensa alcanza para todo" ([19](../sources/19_reward_is_enough_2021.md)) logró zanjarla, y tiene una réplica académica seria en contra ([20](../sources/20_scalar_reward_not_enough_2022.md)). Ese vacío —no una conclusión— es el punto de llegada correcto para una presentación que busca generar debate interno, no cerrarlo.

---

## 1. Encuadre del problema

La pregunta que este análisis responde: **¿es legítimo comparar el entrenamiento de una IA, el aprendizaje de un bebé y el "aprendizaje" de un organoide en los mismos términos?** Respuesta corta: sí, a nivel de *estructura formal* (conducta → consecuencia → ajuste), y no automáticamente a nivel de *lo que eso implica* sobre experiencia subjetiva — confundir ambos niveles es el error más fácil de cometer en este tema, y es precisamente el error que la presentación quiere exponer para generar debate, no el que quiere cometer sin darse cuenta.

## 2. Los tres (cuatro) paradigmas, en la misma tabla

| | IA convencional (aprendizaje supervisado) | IA convencional (aprendizaje por refuerzo) | Humano (condicionamiento operante) | Organoide (DishBrain) |
|---|---|---|---|---|
| **Qué ajusta** | Pesos numéricos de una red neuronal artificial | Política de decisión de un agente | Sinapsis / probabilidad de repetir una conducta | Conexiones funcionales de neuronas vivas |
| **Señal de aprendizaje** | Error respecto a una respuesta "correcta" etiquetada por humanos | Recompensa escalar (positiva/negativa) | Refuerzo o castigo (Skinner: 4 tipos) | Estímulo predecible (ↈ "premio") / impredecible (ↈ "castigo") — principio de energía libre |
| **¿Quién diseña la señal?** | El ingeniero que etiqueta los datos | El ingeniero que define la función de recompensa | El entorno social/familiar (a veces deliberado, a veces no) | El diseño experimental del laboratorio |
| **Evidencia de experiencia subjetiva** | Ninguna reclamada | Ninguna reclamada, salvo por la hipótesis especulativa de [19](../sources/19_reward_is_enough_2021.md) | Asumida por defecto (sabemos que los humanos son conscientes por evidencia externa a la propia teoría) | **No resuelto** — es exactamente la pregunta en disputa ([08](../sources/08_playing_brains_dishbrain_ethics_2023.md)) |
| **Fuente** | — | [17](../sources/17_reinforcement_learning_basics.md) | [18](../sources/18_operant_conditioning_skinner.md) | [02](../sources/02_kagan_2022_dishbrain_neuron.md), [08](../sources/08_playing_brains_dishbrain_ethics_2023.md) |

**Lectura de la tabla:** la columna "evidencia de experiencia subjetiva" es la única que no se puede completar con un simple sí/no para el organoide — y es, no por casualidad, la columna que le falta precisamente al caso que hoy se vende como producto comercial (CL1, [03](../sources/03_cortical_labs_cl1.md)).

## 3. La analogía del bebé y el caramelo, con cuidado

Es una analogía pedagógicamente potente y académicamente defendible (Skinner, [18](../sources/18_operant_conditioning_skinner.md)), pero conviene usarla con dos precisiones para que no se caiga en el primer contraargumento obvio:

1. **El condicionamiento operante es una teoría deliberadamente ciega a la experiencia subjetiva.** Skinner la construyó *ignorando a propósito* la pregunta de qué siente el organismo — describe conducta observable, no consciencia. Usarla para argumentar "el bebé aprende igual que la IA, luego ambos son igual de conscientes (o igual de no-conscientes)" es un salto que ni el propio Skinner habría avalado.
2. **Sabemos que el bebé es consciente por una razón que no tiene nada que ver con el mecanismo de aprendizaje** — lo sabemos porque es humano, biológicamente emparentado con nosotros, y podemos preguntarle (cuando crece) qué sintió. Ni la IA ni el organoide nos pueden dar esa misma clase de evidencia, sin importar cuánto se parezca el mecanismo formal de aprendizaje.

**Por qué la analogía sigue siendo útil pese a esto:** obliga a la audiencia a notar que *el mecanismo* no es, por sí solo, lo que nos convence de que el bebé es consciente — es otra cosa (continuidad biológica, lenguaje, comportamiento social). Entonces, ¿qué es exactamente esa "otra cosa", y la tienen o no la tienen un chip de silicio o un cultivo de neuronas? Ahí es donde entra el problema difícil de la consciencia ([21](../sources/21_hard_problem_consciousness_chalmers.md)).

## 4. Las tres posturas filosóficas, aplicadas a los tres sistemas

| Postura | ¿La IA de silicio podría ser consciente? | ¿El organoide podría ser consciente? |
|---|---|---|
| **Fisicalismo/funcionalismo** | Sí, en principio, si replica la función correcta — no importa el sustrato | Sí, en principio — y con más plausibilidad intuitiva por ser sustrato biológico, aunque el fisicalismo estricto no debería darle ninguna ventaja al carbono sobre el silicio |
| **Dualismo** | No — ningún proceso físico-funcional produce experiencia, sin importar cuán sofisticado | No tampoco — tener neuronas reales no resuelve el problema si la consciencia es, de fondo, no-física (la postura de muchas tradiciones religiosas y filosóficas, la noción de "alma") |
| **Panpsiquismo** | Posiblemente algún grado mínimo de experiencia, si la experiencia es una propiedad fundamental de la materia organizada de cierta forma | Posiblemente también, por la misma razón — sin que ser biológico le dé automáticamente "más" experiencia que al silicio |

**El punto contraintuitivo para remarcar en la presentación:** la intuición común es "un organoide de neuronas humanas está más cerca de ser consciente que un chip, porque es biológico". Esa intuición **no se sostiene igual de fuerte bajo las tres posturas filosóficas** — para un dualista estricto, ninguno de los dos lo es nunca; para un panpsiquista, ambos podrían tener algún grado. La única postura donde "ser biológico" da una ventaja real es una versión particular del fisicalismo que además sostenga que hay algo específico del tejido neuronal vivo (no solo de la función que cumple) que importa — una posición intelectualmente respetable, pero que hay que defender explícitamente, no asumir.

## 5. Riesgos argumentales a evitar en la presentación

- **Falacia genética ("es biológico, por lo tanto consciente"):** el origen del material no determina por sí solo el estatus moral o la presencia de experiencia — ver §4.
- **Falacia funcionalista ingenua ("funciona igual, por lo tanto es igual de consciente"):** el hecho de compartir el esquema premio/castigo (§2) no demuestra nada sobre experiencia subjetiva — es exactamente la distinción entre "problemas fáciles" y "problema difícil" de [21](../sources/21_hard_problem_consciousness_chalmers.md).
- **Presentar "Reward is Enough" como si fuera consenso científico:** es una hipótesis de posición con una réplica académica seria en contra ([20](../sources/20_scalar_reward_not_enough_2022.md)) — usarla para abrir la pregunta, no para cerrarla a favor de una postura.
- **Dejar afuera la dimensión religiosa/existencial por incomodidad:** el usuario pidió explícitamente poder tocarla — el dualismo (§4) es el lugar académicamente honesto donde encaja sin caricaturizarla ni convertir la charla en un sermón. Presentarla como una postura filosófica legítima entre otras, no como la conclusión correcta ni como algo a refutar.

## 6. Ficheros relacionados

[research.md](../research.md) · [analisis/02](02_posturas_eticas_mapa_debate.md) (eje 1, sufrimiento vía principio de energía libre — comparte base con este análisis) · [17](../sources/17_reinforcement_learning_basics.md) · [18](../sources/18_operant_conditioning_skinner.md) · [19](../sources/19_reward_is_enough_2021.md) · [20](../sources/20_scalar_reward_not_enough_2022.md) · [21](../sources/21_hard_problem_consciousness_chalmers.md) · [02](../sources/02_kagan_2022_dishbrain_neuron.md) · [08](../sources/08_playing_brains_dishbrain_ethics_2023.md)
