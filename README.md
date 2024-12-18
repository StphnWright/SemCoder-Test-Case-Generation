# SemCoder Test Case Generation

This repository contains our Colab notebook implementation for evaluating semantic-aware test case generation, comparing SemCoder with DeepSeek Coder variants.

## Overview

We evaluate the effectiveness of semantic-aware language models in generating high-quality test cases, specifically comparing SemCoder and DeepSeek Coder (6.7B and 7B variants). Our evaluation framework implements comprehensive pipelines to assess test case generation capabilities across multiple dimensions, focusing on syntax validity and execution accuracy.

### Requirements
The notebook will automatically install required packages:
- transformers
- torch
- timeout-decorator
- datasets
- pytest
- pytest-cov
- coverage

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
