# The Gradient-Causal Gap

Preprint under review (ICLR 2026 LIT Workshop)

Code for analyzing the mismatch between **gradient-based importance** and **causal importance** in Transformers.

## Overview

This repository studies the **Gradient-Causal Gap**: cases where components with large gradients are not causally important for **out-of-distribution (OOD) generalization**, and vice versa.

We identify:
- **Hidden Heroes**: low-gradient, causally essential components  
- **Gradient Bloats**: high-gradient, causally irrelevant or harmful components  

## Tasks

- Sequence Reversal  
- Sequence Sorting  

## Methods

- Gradient magnitude (Frobenius norm)
- Mean ablation for causal importance
- Spearman correlation (gradient vs. causal)
- Targeted component pruning

## Key Findings

- Gradient–causal alignment degrades with task complexity
- Pruning Hidden Heroes destroys generalization
- Pruning Gradient Bloats is unpredictable and sometimes improves OOD accuracy
