# Overview / 项目概述

OPMMDoctor targets **opportunistic osteoporosis screening** by combining routinely-archived
whole-body multi-joint radiographs with structured clinical indicators.

## Task

Three-class ordinal classification following the WHO DXA T-score standard:

| Class | T-score |
|---|---|
| Normal BMD | T ≥ −1.0 |
| Osteopenia | −2.5 < T < −1.0 |
| Osteoporosis (OP) | T ≤ −2.5 |

## Modules

1. **Image branch** — Swin Transformer V2, hierarchical multi-scale features.
2. **Clinical branch** — sinusoidal encoding of scalar clinical values into tokens.
3. **CVFM (Clinical-Visual Fusion Module)** — region-adaptive cross-modal modulation that
   routes each clinical variable to relevant skeletal regions, plus a reliability-aware gate
   that down-weights clinical information when it is missing or unreliable.
4. **EGOLM (Expert-Guided Ordinal Loss Module)** — ordinal loss with expert-annotated
   salient-feature weighting to constrain mis-classifications to adjacent grades.

## Status

Documentation and code will be completed and released upon manuscript acceptance.
