---
title: Vascular Segmentation of fUS Images using Deep Learning
authors:
- admin
- Thomas Guyet
- Hugues Berry
- Benjamin Vidal
date: '2025-01-01'
publishDate: '2025-07-10T16:16:52.540076Z'
publication_types:
- paper-conference
publication: '*Intelligence Artificielle en Imagerie Biomédicale (IABM), Nice, France*'

url_pdf: https://inria.hal.science/hal-04964498v1
url_poster: Poster-IABM2025.pdf

abstract:  Segmentation of medical images is a fundamental task with numerous applications. While MRI, CT, and PET modalities have significantly benefited from deep learning segmentation techniques, more recent modalities, like functional ultrasound (fUS), have seen limited progress. fUS is a non invasive imaging method that measures changes in cerebral blood volume (CBV) with high spatio-temporal resolution. However, distinguishing arterioles from venules in fUS is challenging due to opposing blood flow directions within the same pixel. Ultrasound localization microscopy (ULM) can enhance resolution by tracking microbubble contrast agents but is invasive, and lacks dynamic CBV quantification. In this paper, we introduce the first deep learning-based application for fUS image segmentation, capable of differentiating signals based on vertical flow direction (upward vs. downward), using ULM-based automatic annotation, and enabling dynamic CBV quantification. In the cortical vasculature, this distinction in flow direction provides a proxy for differentiating arteries from veins. We evaluate various UNet architectures on fUS images of rat brains, achieving competitive segmentation performance, with 90% accuracy, a 71% F1 score, and an IoU of 0.59, using only 100 temporal frames from a fUS stack. These results are comparable to those from tubular structure segmentation in other imaging modalities. Additionally, models trained on resting-state data generalize well to images captured during visual stimulation, highlighting robustness. Although it does not reach the full granularity of ULM, the proposed method provides a practical, non-invasive and cost-effective solution for inferring flow direction—particularly valuable in scenarios where ULM is not available or feasible. Our pipeline shows high linear correlation coefficients between signals from predicted and actual compartments, showcasing its ability to accurately capture blood flow dynamics.
---
