---
title: Improving Spatial Resolution in Functional Ultrasound Through ULM-Guided Generative Learning
authors:
- Hana Sebia
- Thomas Guyet
- Hugues Berry
- Seunghoi Kim
- Daniel C. Alexander
- Benjamin Vidal
date: '2026-03-10'
publishDate: '2026-01-01T00:00:00.000000Z'
publication_types:
- paper-conference
publication: '*Intelligence Artificielle en Imagerie Biomédicale (IABM), Lyon, France*'

url_pdf: https://iabm2026.sciencesconf.org/resource/page/id/21
url_poster: Poster-IABM2025.pdf

tags:
- Image Generation
- Super Resolution
- Functional Ultrasound

abstract: Functional ultrasound (fUS) provides high-sensitivity hemodynamic imaging at the mesoscopic scale and is increasingly used for functional brain studies, but its spatial resolution remains limited. Ultrasound Localization Microscopy (ULM), acquired with the same probe, overcomes this limitation by localizing individual microbubbles to achieve microvascular super-resolution. However, ULM requires long acquisitions, contrast agent injections, and heavy post-processing, limiting its applicability in routine or dynamic functional imaging. In this work, we investigate whether generative AI models can enhance the spatial resolution of fUS to enable high-resolution functional imaging without the constraints of ULM. This task is particularly challenging due to the significant resolution gap between modalities and the extremely limited number of paired acquisitions (35 fUS/ULM image pairs). Rather than aiming to fully reproduce ULM resolution, our objective is to achieve moderate super-resolution. We evaluate three families of generative models; a conditional GAN (Pix2Pix), a multimodal hierarchical variational autoencoder (MHVAE), and a conditional diffusion model specifically adapted to data scarcity through patch-based training, positional embeddings, and an edge-preservation loss. Models are trained on grayscale paired data and assessed using quantitative metrics (MSE, PSNR, SSIM, LPIPS) as well as expert visual evaluation. Results highlight clear trade-offs between approaches. MHVAE achieves the lowest pixel-wise error but produces overly smooth images lacking microvascular details. Pix2Pix reconstructs the main vascular structure but misses finer features. The diffusion model provides the best perceptual and structural fidelity, generating sharper and more coherent vasculature, and is judged by experts as the most anatomically plausible, although it may hallucinate structures and struggle with the smallest vessels. Beyond model comparison, this study emphasizes key methodological insights for learning under extreme data scarcity. Patch-based training and edge-aware regularization are critical for diffusion models, while full-image training fails. Additionally, standard data augmentation strategies can degrade anatomical consistency due to spatial misalignment.Overall, our findings demonstrate that moderate super-resolution of fUS is achievable using generative models, with diffusion-based approaches emerging as the most promising direction under current data limitations.
---