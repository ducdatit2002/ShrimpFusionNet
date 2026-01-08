# ShrimpFusionNet for Real-Time Shrimp Disease Detection Using Trust-Aware Multimodal Fusion

MMSD25 is a real-world multimodal shrimp disease dataset introduced in this paper. 
This repository provides a public sanitized reference subset of MMSD25 together with the benchmark protocol to support reproducibility and further research.

## 1. Dataset Overview

MMSD25 is designed for shrimp disease detection under real aquaculture conditions, where data are noisy, heterogeneous, asynchronous, and partially missing.

The dataset integrates three modalities:

- RGB shrimp images captured directly in ponds
- Farmer-written textual reports describing shrimp health and pond observations
- Environmental sensor streams, including:
  - Temperature
  - pH
  - Dissolved oxygen
  - Turbidity
  - Salinity

Data were collected from 8 shrimp ponds in the Mekong Delta, Vietnam, under diverse environmental and operational conditions.

## 2. Public Release Scope

### What is publicly released

This repository and the associated Hugging Face page provide:

- A **sanitized reference subset** of MMSD25  
- The **full benchmark protocol**, including:
  - Data preprocessing procedures
  - Train, validation, and test split definitions
  - Evaluation scripts and metrics

The public subset is intended to demonstrate data structure, modality alignment, and evaluation methodology.

### What is NOT publicly released

- The **full MMSD25 dataset is NOT publicly available**
- Full raw data are restricted due to data governance and farm partner agreements

Access to the full dataset may be considered for **non-commercial academic research only**, subject to a controlled-access agreement.

## 3. Dataset Composition (Full Dataset Description)

The full MMSD25 dataset (described in the paper) consists of:
- 3, 625 RGB shrimp images
- 12,404 farmer-generated text descriptions
- Synchronized multi-channel sensor time series
- 5 disease classes:
  - Healthy
  - WSSV
  - AHPND
  - EHP
  - Bacterial necrosis
Each sample is verified by aquaculture experts, with inter-annotator agreement reaching Cohen’s κ = 0.86.

## 4. Train / Validation / Test Split

The benchmark uses a **region-based (pond-level) split** to evaluate generalization:

- Training set: 70% of ponds
- Validation set: 10% of ponds
- Test set: 20% of ponds (unseen ponds)

This setup supports zero-shot domain evaluation under real deployment conditions.

## 5. Hugging Face Repository

The public reference subset is hosted on Hugging Face:

https://huggingface.co/ducdatit2002/ShrimpFusionNet

## 6. Intended Use

MMSD25 is intended for research on:

- Multimodal learning (image + text + sensor)
- Trust-aware and uncertainty-aware fusion
- Robust learning under noisy and missing modalities
- Edge AI and IoT-based aquaculture systems

The dataset is **not intended for commercial use**.

## 7. Limitations

- The public subset is not statistically representative of the full dataset
- Some environmental and operational variability present in the full dataset is not exposed
- Results obtained on the public subset should not be interpreted as full benchmark performance

## 8. Citation

If you use MMSD25 or the benchmark protocol, please cite:

```bibtex
@article{shrimpfusionnet2025,
  title={ShrimpFusionNet for Real-Time Shrimp Disease Detection Using Trust-Aware Multimodal Fusion},
  author={Le, Tan Duy and Huynh, Kha Tu and Pham, Duc Dat and Nguyen, Hong Quan and Nguyen, Minh Tu},
  year={2025}
}
````

## 9. License

The public subset of MMSD25 is released for **non-commercial research use only**.

## 11. Contact

For questions or controlled access requests to the full dataset:

* Duc Dat Pham
* Email: [ducdatit2002@gmail.com](mailto:ducdatit2002@gmail.com)

```
