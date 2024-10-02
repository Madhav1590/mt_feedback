# Bilingual Training with SMOL-LM 135M

This project implements a simplified version of the bilingual training methodology presented in the paper [Insert Paper Title Here] using the SMOL-LM 135M model. The aim is to explore bilingual training on a small dataset while addressing challenges related to data preprocessing and model training.

## Table of Contents
- [Project Overview](#project-overview)
- [Requirements](#requirements)
- [Installation](#installation)
- [Dataset](#dataset)
- [Data Preparation](#data-preparation)
- [Model Setup](#model-setup)
- [Training](#training)
- [Reproducing Results](#reproducing-results)
- [Challenges and Solutions](#challenges-and-solutions)
- [Conclusion](#conclusion)
- [License](#license)

## Project Overview
This project uses the SMOL-LM 135M model for bilingual training tasks. The dataset used in this implementation is sourced from [zoeyki/mt_feedback_dataset](https://huggingface.co/datasets/zoeyki/mt_feedback_dataset), focusing on English-German, English-Chinese, and English-Russian pairs. The model is fine-tuned using the `SFTTrainer` from the `trl` library.

## Requirements
To run this project, the following libraries and dependencies are required:
- Python >= 3.8
- torch
- transformers
- datasets
- peft
- trl
- huggingface_hub


