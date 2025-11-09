# MAP - Charting Student Math Misunderstandings

[![Kaggle Competition](https://img.shields.io/badge/Kaggle-Competition-blue.svg)](https://www.kaggle.com/competitions/map-charting-student-misunderstandings)
[![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-green.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## 📖 Overview

This project addresses the critical educational challenge of automatically identifying mathematical misconceptions from student-written explanations. Built for the Kaggle competition "MAP - Charting Student Math Misunderstandings" in collaboration with Vanderbilt University and The Learning Agency.

## 🎯 Project Objective

Develop machine learning systems that can:
- Analyze short student-written math explanations
- Identify specific mathematical misconceptions
- Rank the top 3 most likely misconceptions using MAP@3 metric
- Provide actionable insights for educators

## 🏗️ Methodology

### Dual-Track Pipeline Architecture

1. **Baseline Model (TF-IDF + XGBoost)**
   - Efficient lexical pattern recognition
   - Math-aware text preprocessing
   - Multi-class classification with probability ranking

2. **Neural Model (DistilBERT Transformer)**
   - Fine-tuned for semantic understanding
   - Combined label space training
   - Enhanced rare class detection

3. **Optimized Ensemble**
   - Weighted combination of XGBoost and DistilBERT
   - MAP@3 score: **0.8437**
   - Top-3 Accuracy: **96.06%**

## 📊 Key Results

| Model | MAP@3 | Top-1 Accuracy | Top-3 Accuracy | Macro F1 |
|-------|-------|----------------|----------------|----------|
| XGBoost | 0.8136 | 72.1% | 94.2% | 0.46 |
| DistilBERT | 0.8393 | 74.7% | 95.7% | 0.74 |
| **Ensemble** | **0.8437** | **74.9%** | **96.06%** | **0.75** |

## 🚀 Quick Start

### Prerequisites
```bash
Python 3.8+
Jupyter Notebook
Required packages in requirements.txt
