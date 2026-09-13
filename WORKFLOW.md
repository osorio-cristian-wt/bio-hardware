# WORKFLOW — Cómo seguir investigando en este repositorio

> Metodología replicada de [`casaJustina/WORKFLOW.md`](../casaJustina/WORKFLOW.md), adaptada al dominio de biocomputación/organoid intelligence. Si vas a sumar un ángulo nuevo (vos, un compañero, o un LLM), seguí este flujo.

---

## 0. Principios

1. **Una fuente → un archivo.** Nada de mezclar varios papers/artículos en un solo archivo de `sources/`.
2. **Toda síntesis cita fuentes.** Si afirmás algo en `research.md` o `analisis/`, debe poder rastrearse a un archivo de `sources/`.
3. **Marcá lo que no pudiste verificar.** Varias fuentes de este repo tienen paywall/bloqueo de bot — están marcadas explícitamente con ⚠️ en "Observaciones". No borres esa marca sin verificar el original.
4. **Distinguí evidencia de marketing.** Este campo tiene mucho comunicado de prensa disfrazado de dato técnico (ver `analisis/01`). Cuando una cifra viene de una empresa (Cortical Labs, FinalSpark), señalalo.
5. **Tablas antes que prosa** cuando haya datos comparables.

---

## 1. Fases

```
FASE 1 — RECONNAISSANCE     → 6-8 búsquedas web amplias en paralelo, sin escribir archivos todavía
FASE 2 — DEEP DIVE           → WebFetch por fuente clave → sources/NN_*.md
FASE 3 — SYNTHESIS           → actualizar research.md con patrones transversales
FASE 4 — CRITICAL ANALYSIS   → analisis/NN_*.md sobre una pregunta concreta
FASE 5 — ENTREGABLE          → si el hallazgo cambia el debate, actualizar entregables/01_guia_debate.md
```

## 2. Plantilla para `sources/NN_nombre.md`

```markdown
# <Título descriptivo>

- **URL:** <link>
- **URL secundaria (opcional):** <link>
- **Fecha de consulta:** YYYY-MM-DD
- **Tipo:** <académico / prensa / oficial / opinión>

## Resumen del contenido
## Información clave
## Relevancia para el debate
## Implicancias tecnológicas
## Citas relevantes
## Observaciones
```

Reglas: nombre `NN_palabra_clave.md` (dos dígitos), citas textuales siempre entre `> ""`, si el texto completo estuvo bloqueado (403/paywall) decilo explícitamente en Observaciones en vez de inventar contenido.

## 3. Plantilla para `analisis/NN_tema.md`

Más libre, pero debería incluir: TL;DR con veredicto, qué está demostrado vs. qué se presenta como demostrado sin estarlo, datos duros en tabla, y "ficheros relacionados" al final.

## 4. Cuándo escribir cada archivo

| Situación | Dónde |
|---|---|
| URL nueva con info útil | `sources/NN_*.md` |
| Ya cubierto en una fuente existente | Actualizar esa fuente, no duplicar |
| Evaluando una afirmación concreta (ej. "¿es cierto el dato de eficiencia energética?") | `analisis/NN_*.md` |
| Cambia la síntesis general del campo | `research.md` (sección correspondiente) |
| Cambia algo que se va a decir en el debate | `entregables/01_guia_debate.md` |
| Sigla/término nuevo | `GLOSARIO.md` |

## 5. Vectores pendientes conocidos (ver `README.md` § Pendiente)

1. Marco legal y cobertura académica argentina/latinoamericana — **no investigado todavía**.
2. Verificación de citas textuales contra PDF original en las fuentes marcadas con ⚠️ (`02`, `08`, `15`, `16`).
3. Un eventual "eje 6" del mapa ético si aparece evidencia nueva que no encaje en los 5 ejes de `analisis/02`.

## 6. Prompt probado para continuar con un LLM

```
Necesito profundizar en <ángulo> dentro de la investigación de neuronas humanas
como hardware de IA (repositorio bio-hardware).

Hacé 4-6 búsquedas web en paralelo cubriendo:
- Evidencia técnica/académica
- Cobertura de prensa especializada
- Postura ética o regulatoria específica
- Comparación internacional si aplica

Para cada fuente relevante, hacé WebFetch y escribí un archivo en sources/
siguiendo la plantilla de WORKFLOW.md § 2. Marcá con ⚠️ cualquier fuente
cuyo texto completo no se pudo verificar (403/paywall).

Después actualizá research.md con cualquier patrón transversal nuevo,
sin duplicar lo que ya está en sources/.
```

## 7. Reglas de calidad antes de dar por cerrado un archivo

- [ ] ¿Tiene URL canónica?
- [ ] ¿Fecha de consulta?
- [ ] ¿Citas textuales separadas de paráfrasis, y marcadas si no se pudieron verificar?
- [ ] ¿Tablas en vez de prosa larga cuando aplica?
- [ ] ¿Distingue evidencia demostrada de afirmación comercial/de marketing?
- [ ] ¿Vinculado a fuentes relacionadas con `[link](path)`?
