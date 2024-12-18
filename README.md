# SemCoder Test Case Generation

This repository contains our Colab notebook implementation for evaluating semantic-aware test case and oracle generation, comparing SemCoder with DeepSeek Coder variants.

## Overview

We evaluate the effectiveness of semantic-aware language models in generating high-quality test cases, specifically comparing SemCoder and DeepSeek Coder (6.7B and 7B variants). Our evaluation framework implements comprehensive pipelines to assess test case generation capabilities across multiple dimensions, focusing on syntax validity and execution accuracy.

## Getting Started

### Requirements
The notebook will automatically install required packages:
- transformers
- torch
- timeout-decorator
- datasets
- pytest
- pytest-cov
- coverage

### Running the Experiments

To reproduce our results:

1. **Core Behavior Analysis**
   - Run all sections from 'Imports & Setup' through 'Final Results: DeepSeek v. SemCoder'
   - This provides initial behavior results comparing DeepSeek 7B and SemCoder

2. **Ablative Analysis**
   - Run the "Code Coverage Assessment" section
   - Run the "Measuring Novelty and Diversity > Measuring with Patterns" section
   - These sections provide detailed analysis of test coverage and diversity metrics

## Notebook Structure

The notebook is organized into the following sections:

1. **Setup and Imports**
   - Environment configuration
   - Memory management utilities
   - Package installation

2. **Model Initialization**
   - Loading DeepSeek and SemCoder models
   - Memory optimization implementation

3. **Test Generation Pipeline**
   - HumanEval dataset processing
   - Test case generation functions
   - Output cleaning and validation

4. **Evaluation Framework**
   - Syntax validation
   - Execution testing
   - Coverage analysis
   - Pattern analysis

5. **Results Analysis**
   - Performance metrics
   - Comparative analysis
   - Error analysis

## Results

Our current implementation demonstrates:
- Syntax validity: >90%
- Execution accuracy: >70%
- Significant improvement with semantic awareness

## Citation

If you use this implementation in your research, please cite:
```bibtex
@article{semcoder2024,
  title={SemCoder: Training Code Language Models with Comprehensive Semantics},
  author={Ding, Yangruibo and Peng, Jinjun and Min, Marcus J. and Kaiser, Gail and Yang, Junfeng and Ray, Baishakhi},
  journal={arXiv preprint arXiv:2406.01006},
  year={2024}
}
Contributors

Maria Gancayco (mig2131@columbia.edu)
Stephen Wright (svw2112@columbia.edu)
