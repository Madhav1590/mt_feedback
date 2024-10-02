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


@inproceedings{ki-carpuat-2024-guiding,
    title = "Guiding Large Language Models to Post-Edit Machine Translation with Error Annotations",
    author = "Ki, Dayeon  and
      Carpuat, Marine",
    editor = "Duh, Kevin  and
      Gomez, Helena  and
      Bethard, Steven",
    booktitle = "Findings of the Association for Computational Linguistics: NAACL 2024",
    month = jun,
    year = "2024",
    address = "Mexico City, Mexico",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2024.findings-naacl.265",
    pages = "4253--4273",
    abstract = "Machine Translation (MT) remains one of the last NLP tasks where large language models (LLMs) have not yet replaced dedicated supervised systems. This work exploits the complementary strengths of LLMs and supervised MT by guiding LLMs to automatically post-edit MT with external feedback on its quality, derived from Multidimensional Quality Metric (MQM) annotations. Working with LLaMA-2 models, we consider prompting strategies varying the nature of feedback provided and then fine-tune the LLM to improve its ability to exploit the provided guidance. Through experiments on Chinese-English, English-German, and English-Russian MQM data, we demonstrate that prompting LLMs to post-edit MT improves TER, BLEU and COMET scores, although the benefits of fine-grained feedback are not clear. Fine-tuning helps integrate fine-grained feedback more effectively and further improves translation quality based on both automatic and human evaluation.",
}

