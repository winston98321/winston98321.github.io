---
title: "Prompt-Based Vertebral Segmentation Using a Generative AI Approach in OVCF Spinal Radiographs"
collection: publications
permalink: /publication/2025-prompt-vertebral-segmentation
excerpt: 'This paper introduces a generative AI framework combining YOLO-based detection with prompt-driven segmentation (SAM-inspired) for vertebral segmentation in spinal X-rays, achieving Dice 0.9389 and IoU 0.8854 on OVCF patients including challenging post-vertebroplasty cases.'
date: 2025-10-22
venue: 'Asia Pacific Signal and Information Processing Association Annual Summit and Conference (APSIPA ASC 2025)'
paperurl: 'https://doi.org/10.1109/apsipaasc65261.2025.11249394'
citation: 'Po-Kai Su, Pei-Rong Jiang, Kai-Xuan Xu, Meng-Lei Su, Jiann-Her Lin, Hsin-Han Chiang, Hsiao-Chi Li. (2025). &quot;Prompt-Based Vertebral Segmentation Using a Generative AI Approach in OVCF Spinal Radiographs.&quot; <i>APSIPA ASC 2025</i>. DOI: 10.1109/apsipaasc65261.2025.11249394'
---



## Background

Osteoporotic vertebral compression fractures (OVCFs) are prevalent among elderly patients, with X-ray imaging serving as the primary diagnostic tool. However, challenges such as organ obstruction and poor contrast after vertebroplasty procedures complicate vertebral segmentation in spinal X-rays.

Most OVCF studies focus on classification tasks rather than segmentation. Precise postoperative vertebrae segmentation remains underexplored despite its importance for treatment monitoring and providing biomechanics and radiomics a firm foundation for further research. X-ray images after vertebroplasty (VP) surgery — with surgical implants including cages, screws, and other hardware — are hard to read, and existing methods relying on handcrafted parameter tuning lead to weak generalizability across datasets.
<img src="/images/APSIPA_flowchart.png" alt="Framework Overview" style="width:100%; border-radius:6px; margin: 16px 0;">
## Method

This research introduces an innovative generative AI framework for vertebral segmentation in spinal X-ray images, combining YOLO-based detection with prompt-driven segmentation inspired by the Segment Anything Model (SAM). The system generates bounding boxes around vertebrae as segmentation prompts and employs an interpolation strategy to address potentially missed compressed vertebrae. By incorporating domain-specific knowledge of vertebral anatomy via the interpolation strategy, the framework enables accurate delineation of vertebral structures in cases of compression fractures.

## Results

| Metric | Score |
|--------|-------|
| Dice Coefficient | 0.9389 ± 0.0026 |
| IoU | 0.8854 ± 0.0045 |
| Sensitivity | 0.9436 ± 0.0062 |

This generative AI application effectively addresses clinical challenges in vertebral segmentation for OVCF patients, potentially enhancing the accuracy of diagnoses and treatment planning.

---

<div style="display:flex; gap:12px; flex-wrap:wrap; margin: 8px 0;">
  <a href="https://doi.org/10.1109/apsipaasc65261.2025.11249394" target="_blank" style="display:inline-flex; align-items:center; gap:6px; padding:0.5em 1.2em; background:#0f4c81; color:#fff; border-radius:2em; text-decoration:none; font-size:0.9em; font-weight:600;">
    📄 View Paper (DOI)
  </a>
  <a href="/files/APSIPA_Poster.pdf" target="_blank" style="display:inline-flex; align-items:center; gap:6px; padding:0.5em 1.2em; background:#fff; color:#0f4c81; border:2px solid #0f4c81; border-radius:2em; text-decoration:none; font-size:0.9em; font-weight:600;">
    🖼️ Download Poster (PDF)
  </a>
</div>

