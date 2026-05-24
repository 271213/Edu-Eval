# Edu-Eval: A Large-Scale Multimodal Benchmark for MLLMs in Authentic Educational Scenarios

[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)
[![Paper](https://img.shields.io/badge/Paper-KDD%202026-blue)](#)
[![Dataset](https://img.shields.io/badge/Dataset-HuggingFace-yellow)](#)

> [cite_start]This is the official repository for the KDD 2026 paper: **Edu-Eval: A Large-Scale Multimodal Benchmark for MLLMs in Authentic Educational Scenarios**[cite: 22].

## 📖 Introduction
[cite_start]The modern classroom is an inherently multimodal environment, rich with the teacher's speech, student expressions, and interactive instructional resources[cite: 8]. [cite_start]However, existing benchmarks primarily test Multimodal Large Language Models (MLLMs) as *students* rather than as *assistants*[cite: 10]. 

[cite_start]To fill this critical gap, we introduce **Edu-Eval**, the first large-scale benchmark focused on **educational scenario-centric evaluation**[cite: 11]. [cite_start]Constructed from over 3,000 real-world scenarios, Edu-Eval comprises 75,900 annotated samples designed to comprehensively assess the entire pedagogical process[cite: 13, 52].

## 🎯 The Teacher-Student-Resource Framework
[cite_start]Inspired by educational theories, we computationally operationalize abstract pedagogical concepts into nine concrete evaluation tasks across three core pillars[cite: 12, 50, 51]:

### 🧑‍🏫 Teacher Dimension
* [cite_start]**Teacher Behavior Understanding (TBU):** Evaluates spatial modeling and recognition of 10 in-class behaviors across 7,000 video samples[cite: 58, 159].
* [cite_start]**Teacher Emotion Recognition (TER):** Assesses perception of nuanced emotional states across 8 categories from 15,000 audio samples[cite: 88, 169].
* [cite_start]**Lesson Plan Generation (LPG):** Evaluates the generation of structured lesson plans using 2,000 carefully curated samples[cite: 78, 181].

### 🙋 Student Dimension
* [cite_start]**Student Gaze Point Prediction (SGPP):** Identifies student attention across 5 gaze direction categories from 2,000 image samples[cite: 70, 72, 194].
* [cite_start]**Student Action Recognition (SAR):** Recognizes 8 fundamental classroom behaviors (e.g., raising hands, reading aloud) from 2,000 image samples[cite: 75, 76, 201].
* [cite_start]**Student Ability Modeling (SAM):** Predicts knowledge mastery and future performance from historical learning behaviors using 10,500 samples[cite: 63, 209].

### 📚 Resource Dimension
* [cite_start]**Essay Scoring (ES):** Evaluates MLLMs' ability to assign scores and generate multi-dimensional feedback from 2,000 essay images[cite: 106, 216].
* [cite_start]**Problem Solving (PS):** Tests robust mathematical reasoning using 30,000 questions transformed via semantic rewriting and reverse reasoning[cite: 94, 230].
* [cite_start]**Question Generation (QG):** Evaluates the generation of pedagogically-aligned questions based on difficulty, knowledge points, and Bloom's cognitive levels across 5,400 samples[cite: 98, 239].

## 📊 Key Findings
[cite_start]Our comprehensive evaluation of 8 mainstream MLLM series (including Claude 3.7, Gemini 2.5 Pro, and GPT-4o) reveals critical capability boundaries[cite: 110, 252]:
1.  [cite_start]**Multimodal Reasoning is the Bottleneck:** Models struggle with fine-grained temporal logic (TBU), acoustic emotion (TER), and non-salient visual targets (SGPP)[cite: 546, 547].
2.  [cite_start]**Conservative Behavior in Higher-Order Tasks:** MLLMs excel at surface-level, memorization-based tasks but consistently fail at true reasoning and generating high-level ("Create") cognitive questions[cite: 550, 551].
3.  [cite_start]**Domain-Specific Advantages:** Smaller parameter education-specific models (e.g., Spark) perform on par with or surpass general-purpose models in specialized educational tasks[cite: 553, 554].

## 🚀 Quick Start
### Installation
```bash
git clone [https://github.com/271213/Edu-Eval.git](https://github.com/271213/Edu-Eval.git)
cd Edu-Eval
pip install -r requirements.txt
