# Source Code / 源代码

> The full training and inference code (model definitions, CVFM, EGOLM, data pipeline,
> and evaluation scripts) will be released here **upon acceptance of the manuscript**.
>
> 完整训练与推理代码将在论文接收后公开。

Planned layout:

```
src/
├── models/            # backbone, CVFM, EGOLM, classifier
├── data/              # dataset & preprocessing (patient-level split)
├── train.py           # training entry
├── evaluate.py        # 10-fold CV & leave-one-hospital-out evaluation
└── visualize.py       # Grad-CAM & clinical feature attribution
```
