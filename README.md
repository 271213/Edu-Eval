# Edu-Eval: A Large-Scale Multimodal Benchmark for MLLMs in Authentic Educational Scenarios

[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)
[![Paper](https://img.shields.io/badge/Paper-KDD%202026-blue)](#)
[![Dataset](https://img.shields.io/badge/Dataset-HuggingFace-yellow)](#)

> This is the official repository for the KDD 2026 paper: **Edu-Eval: A Large-Scale Multimodal Benchmark for MLLMs in Authentic Educational Scenarios**.

## 📖 Introduction
The modern classroom is an inherently multimodal environment, rich with the teacher's speech, student expressions, and interactive instructional resources. However, existing benchmarks primarily test Multimodal Large Language Models (MLLMs) as *students* rather than as *assistants*. 

To fill this critical gap, we introduce **Edu-Eval**, the first large-scale benchmark focused on **educational scenario-centric evaluation**. Constructed from over 3,000 real-world scenarios, Edu-Eval comprises 75,900 annotated samples designed to comprehensively assess the entire pedagogical process.

## 🎯 The Teacher-Student-Resource Framework
Inspired by educational theories, we computationally operationalize abstract pedagogical concepts into nine concrete evaluation tasks across three core pillars:

### 🧑‍🏫 Teacher Dimension
* **Teacher Behavior Understanding (TBU):** Evaluates spatial modeling and recognition of 10 in-class behaviors across 7,000 video samples.
* **Teacher Emotion Recognition (TER):** Assesses perception of nuanced emotional states across 8 categories from 15,000 audio samples.
* **Lesson Plan Generation (LPG):** Evaluates the generation of structured lesson plans using 2,000 carefully curated samples.

### 🙋 Student Dimension
* **Student Gaze Point Prediction (SGPP):** Identifies student attention across 5 gaze direction categories from 2,000 image samples.
* **Student Action Recognition (SAR):** Recognizes 8 fundamental classroom behaviors (e.g., raising hands, reading aloud) from 2,000 image samples.
* **Student Ability Modeling (SAM):** Predicts knowledge mastery and future performance from historical learning behaviors using 10,500 samples.

### 📚 Resource Dimension
* **Essay Scoring (ES):** Evaluates MLLMs' ability to assign scores and generate multi-dimensional feedback from 2,000 essay images.
* **Problem Solving (PS):** Tests robust mathematical reasoning using 30,000 questions transformed via semantic rewriting and reverse reasoning.
* **Question Generation (QG):** Evaluates the generation of pedagogically-aligned questions based on difficulty, knowledge points, and Bloom's cognitive levels across 5,400 samples.

## 📊 Key Findings
Our comprehensive evaluation of 8 mainstream MLLM series (including Claude 3.7, Gemini 2.5 Pro, and GPT-4o) reveals critical capability boundaries:
1.  **Multimodal Reasoning is the Bottleneck:** Models struggle with fine-grained temporal logic (TBU), acoustic emotion (TER), and non-salient visual targets (SGPP).
2.  **Conservative Behavior in Higher-Order Tasks:** MLLMs excel at surface-level, memorization-based tasks but consistently fail at true reasoning and generating high-level ("Create") cognitive questions.
3.  **Domain-Specific Advantages:** Smaller parameter education-specific models (e.g., Spark) perform on par with or surpass general-purpose models in specialized educational tasks.

## 🚀 Quick Start

