# Sentiment Analysis Optimization for Arm Architecture

## Project Overview
This project takes a pre-trained sentiment analysis model (DistilBERT) 
from Hugging Face and optimizes it using ONNX Runtime to run more 
efficiently on Arm-based architecture. The goal is to demonstrate how 
existing AI models can be migrated and optimized for better performance 
on Arm-powered devices.

## Functionality / Output
The model takes text input and classifies it as POSITIVE or NEGATIVE 
sentiment. The final output is an optimized ONNX version of the model 
that runs significantly faster than the original PyTorch model, while 
maintaining the same accuracy.

### Benchmark Results
- Original model: ~0.07-0.20 seconds per inference
- Optimized model (ONNX): ~0.03-0.13 seconds per inference
- Performance improvement: 36-57% faster

## Setup Instructions
1. Open the sentiment_analysis_onnx_arm_optimization.ipynb file in 
   Google Colab
2. Run all cells sequentially (Runtime → Run all)
3. The notebook will automatically:
   - Install required libraries (transformers, torch, optimum)
   - Download the pre-trained DistilBERT model
   - Test the original model's performance
   - Convert the model to ONNX format
   - Benchmark and compare both versions

## Tools Used
- Hugging Face Transformers
- PyTorch
- Optimum (ONNX Runtime)
- Google Colab

## Track
Track 2 - Migration/Adoption Value
