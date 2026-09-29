# CLASSY-Breast
Computational workflow for breast MRI processing and quadrant-based volumetric analysis.

## Overview
CLASSY-Breast is a Python-based computational workflow for processing breast magnetic resonance imaging (MRI), generating
breast segmentations, integrating anatomical landmarks, and dividing each breast into four quadrants using alternative geometric
definitions.

## Workflow
• MRI input, preprocessing, orientation handling, and eligibility checks;
• Automated breast segmentation using the pretrained 3D Breast U-Net described by Lew et al. (2024);
• Segmentation and geometry quality-control procedures;
• Assessment of breast deformation;
• Integration of manually annotated nipple landmarks using 3D Slicer;
• Computation of breast centroids and anatomical reference geometry;
• Division of each breast into four quadrants using three alternative geometric methods;
• Calculation of absolute and relative quadrant volumes;
• Interactive quality-control visualization;
• Structured export of measurements and workflow status.

## External Segmentation Model
Breast segmentation uses the publicly available pretrained 3D Breast U-Net described by Lew et al., developed using breast MRI
from the Duke Breast Cancer MRI dataset. The model, model weights, and associated external implementation are not distributed
as part of CLASSY-Breast and remain subject to their original licensing terms.
Lew, C. O., Harouni, M., Kirksey, E. R., Kang, E. J., Dong, H., Gu, H., Grimm, L. J., Walsh, R., Lowell, D. A., & Mazurowski, M. A. (2024). A
publicly available deep learning model and dataset for segmentation of breast, fibroglandular tissue, and vessels in breast MRI. Scientific Reports,
14, 5383. DOI: 10.1038/s41598-024-54048-2

## Repository Scope
This repository contains the computational notebook implementing the CLASSY-Breast workflow. Imaging data, manual
annotations, generated masks, intermediate files, visual outputs, quantitative results, third-party model code, and pretrained model
weights are not included.

## Development and Supervision
Developed by Jade Ferreira Carvalheiro Achiam with the assistance of large language models (LLMs), under the supervision of
António Sampaio Soares, in the context of the Computational Surgery Lab. LLMs were used as development tools during iterative
coding, debugging, documentation, and workflow refinement.

## License
The original CLASSY-Breast software is jointly copyrighted by Jade Ferreira Carvalheiro Achiam and António Sampaio Soares
and is licensed under the PolyForm Noncommercial License 1.0.0. This license permits use, modification, and redistribution for
noncommercial purposes, subject to its terms. Third-party software, pretrained models, model weights, and other external
resources are not covered by the CLASSY-Breast license and remain subject to their respective licenses and terms. In particular,
the external breast-segmentation model and associated implementation described by Lew et al. (2024) are not licensed or
distributed as part of CLASSY-Breast.
