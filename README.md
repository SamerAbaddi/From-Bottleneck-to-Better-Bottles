# From Bottleneck to Better Bottles

**Artificial Intelligence supported Lean Six Sigma for plastic bottle manufacturing quality improvement**

Copyright © 2026 Samer Abaddi. All rights reserved.

## Repository description

This repository supports the study **From Bottleneck to Better Bottles**, which investigates how Lean Six Sigma and artificial intelligence can be integrated to reduce defects, improve inspection consistency, and support sustained process control in semi-automated plastic bottle manufacturing.

The study focuses on an anonymized 250-ml PET bottle production line. Company identity, plant location, equipment identifiers, operator information, supplier details, and proprietary process settings are intentionally excluded to protect industrial confidentiality.

## What this repository contains

This repository is intended to include a small anonymized sample of collected bottle images used for inspection-model development and documentation.

### Sample image summary

| Class | File prefix | Number of images | Description |
|---|---:|---:|---|
| Accepted bottles | `ACCxx` | 50 | Bottles classified as saleable with no rejectable feature |
| Minor-defect bottles | `MINxx` | 48 | Bottles with low-risk cosmetic or recoverable defects |
| Major-defect bottles | `MAJxx` | 58 | Bottles with structural, sealing, forming, or high-risk visual defects |
| **Total** | — | **156** | Sample images across the three quality classes |

## Suggested folder structure

```text
from-bottleneck-to-better-bottles/
├── README.md
├── LICENSE
├── .gitignore
├── data/
│   ├── sample_image_manifest.csv
│   └── sample_images/
│       ├── accepted/
│       │   └── ACC01 ... ACC50
│       ├── minor/
│       │   └── MIN01 ... MIN48
│       └── major/
│           └── MAJ01 ... MAJ58
├── docs/
│   └── DATASET_NOTES.md
└── src/
    └── README.md
```

## Image naming convention

Use short anonymized names only:

- Accepted bottles: `ACC01`, `ACC02`, ..., `ACC50`
- Minor-defect bottles: `MIN01`, `MIN02`, ..., `MIN48`
- Major-defect bottles: `MAJ01`, `MAJ02`, ..., `MAJ58`

Recommended file extensions are `.jpg` or `.png`. Keep the same extension consistently within each class when possible.

## Data anonymization rules

Before adding images to this repository, remove or mask:

- company logos;
- operator faces or body features;
- plant signs, labels, and location identifiers;
- machine serial numbers or supplier identifiers;
- any proprietary production settings visible in the image background.

Only bottle-region images should be included. Images should be cropped around the product when possible.

## Study context

The manuscript evaluates an integrated framework combining:

1. Lean Six Sigma DMAIC structure;
2. baseline defect and cost-of-poor-quality analysis;
3. root-cause analysis using statistical and engineering tools;
4. machine-learning image classification for accepted, minor-defect, and major-defect bottles;
5. sustained control using process indicators and inspection feedback.

The full industrial dataset is not released because it contains confidential production records and proprietary image data. The sample images are provided only for demonstration, documentation, and reproducibility of the inspection-class structure.

## Dataset classes

### Accepted

Accepted bottles are saleable bottles with no visible feature expected to affect sealing, strength, filling compatibility, downstream handling, or customer appearance.

### Minor defect

Minor-defect bottles contain visible low-risk nonconformities, typically cosmetic or recoverable, that do not compromise basic function.

Examples may include light scuffing, haze, faint flow lines, mild cosmetic dents, or small non-critical specks.

### Major defect

Major-defect bottles contain defects that may affect sealing, structural integrity, downstream processing, leakage risk, or customer acceptance.

Examples may include short blow, cracks, leak paths, severe deformation, damaged neck finish, unstable base, or severe contamination.

## Recommended use

This repository can be used to:

- document the sample image structure;
- demonstrate class naming and image organization;
- support supplementary material for the manuscript;
- provide a reproducible starting point for image-classification experiments;
- show how quality-control labels were mapped into machine-learning classes.

## Important note

This repository should not be used to disclose confidential factory information. Public sharing should be limited to anonymized sample images and non-proprietary documentation.

## Citation

If this repository supports a publication, cite the final manuscript once published.

Suggested repository citation before publication:

Abaddi S. From Bottleneck to Better Bottles: Artificial Intelligence supported Lean Six Sigma for plastic bottle manufacturing quality improvement. GitHub repository. 2026.

## Copyright

Copyright © 2026 Samer Abaddi. All rights reserved.

No part of this repository may be copied, redistributed, modified, or used for commercial purposes without prior written permission from the copyright holder.
