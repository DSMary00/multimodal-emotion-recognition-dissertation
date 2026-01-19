# Multimodal Emotion Recognition (MSc Dissertation)

This repository contains the code, experiments, and documentation for my MSc Data Science dissertation at Manchester Metropolitan University. The project focuses on **multimodal emotion recognition**, exploring how combining text, audio, and visual information can improve the prediction of emotional states compared to unimodal approaches.

## Project Background and Motivation
Emotion recognition plays an important role in areas such as human–computer interaction, mental health analysis, and conversational AI. Many existing approaches rely on a single data modality, such as text or speech, which can limit performance when emotional cues are subtle or ambiguous. Human emotion is naturally multimodal, expressed through language, tone of voice, and facial expressions. This project was motivated by the question of whether integrating multiple modalities can lead to more robust and accurate emotion recognition models.

## Research Aims
The main aim of this dissertation is to evaluate the effectiveness of multimodal learning for emotion recognition. Specifically, the project seeks to:
- Compare unimodal and multimodal models for emotion prediction
- Investigate different feature-level fusion strategies
- Assess whether improved fusion architectures outperform simple baseline models
- Explore the use of large language models, specifically Emotion-LLaMA, in a zero-shot emotion recognition setting

## Dataset
This project uses the **CMU-MOSI** dataset, a widely used benchmark for multimodal sentiment and emotion analysis. The dataset includes aligned text transcripts, audio features, and visual features extracted from video recordings. The task focuses on predicting emotional or sentiment-related outcomes based on these modalities. Due to licensing restrictions, the raw dataset is not included in this repository.

## Methodology and Models
Several models were implemented and evaluated throughout the project. These include unimodal models trained separately on text, audio, and visual features, as well as multimodal fusion models that combine all three modalities. A baseline fusion approach using simple concatenation was first established, followed by an improved fusion architecture incorporating GRU-based encoders and a multi-layer perceptron classifier. In addition, Emotion-LLaMA was evaluated in a zero-shot setting to compare large language model performance against supervised multimodal approaches.

## Evaluation
Model performance was evaluated using a range of metrics to provide a balanced assessment of predictive accuracy and error. These metrics include Accuracy, F1-score, Mean Absolute Error (MAE), and Pearson correlation coefficient. This combination of metrics allows for both classification-style evaluation and regression-based performance analysis.

## Key Findings
The results show that multimodal fusion models generally outperform unimodal approaches, supporting the hypothesis that combining modalities improves emotion recognition performance. Text features contributed most strongly to overall model performance, while audio and visual features provided complementary information. Improved fusion architectures demonstrated better stability and robustness compared to baseline fusion methods. Emotion-LLaMA showed potential in zero-shot emotion recognition but did not consistently outperform supervised multimodal models trained directly on the dataset.

## Repository Structure
The repository is organised as follows:
- `data/` – Data preprocessing scripts and metadata (no raw data included)
- `models/` – Model definitions and architectures
- `experiments/` – Training and evaluation notebooks
- `results/` – Performance metrics and visualisations
- `docs/` – Dissertation report and supporting figures

## Reproducibility
Instructions and scripts are provided to support reproducibility of the experiments, excluding access to the raw dataset. Dependencies are listed in the requirements file, and training and evaluation steps are documented within the experiment notebooks.

## Limitations and Future Work
The project is limited by the size and scope of the available dataset, which may restrict generalisability to real-world applications. Future work could explore attention-based fusion methods, larger and more diverse multimodal datasets, and fine-tuning large language models for multimodal emotion recognition tasks.

## Author
**Mary Owofolaju**  
MSc Data Science, Manchester Metropolitan University  

This repository is shared for academic and portfolio purposes.
