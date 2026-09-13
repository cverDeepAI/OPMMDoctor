# Architecture / 架构说明

```
                 ┌─────────────────────────┐
  X-ray (10 joints) ─▶│  Image Branch (Swin V2) │──┐
                 └─────────────────────────┘  │
                                              ▼
                 ┌─────────────────────────┐  ┌───────────────────────────┐
 Clinical vars ─▶│ Clinical Encoding (sin) │─▶│  CVFM                     │─▶ fused feature ─▶ classifier
                 └─────────────────────────┘  │  • region cross-modal      │
                                              │    modulation (α, β)       │
                                              │  • reliability-aware gate  │
                                              └───────────────────────────┘
                                                          │
                                              EGOLM (ordinal loss + EASF)
```

Full module definitions, hyper-parameters and training scripts will be provided here upon
manuscript acceptance.
