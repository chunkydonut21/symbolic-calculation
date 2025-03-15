# Symbolic Calculation Project

This repository contains code for generating symbolic functions and their Taylor expansions (up to fourth order), and training sequence-to-sequence models (LSTM and Transformer) to learn these expansions.

---

## Overview

1. **Data Generation**  
   - Uses Sympy to generate a diverse set of functions with random coefficients and terms.  
   - Computes the Taylor expansion (up to \(x^4\)) for each function.  
   - Saves the resulting dataset in a tokenized format (e.g., CSV).

2. **LSTM Model**  
   - An LSTM-based sequence-to-sequence model is trained to map each function’s tokenized representation to its corresponding Taylor expansion.  
   - The model is trained via teacher forcing, minimizing the difference between predicted expansions and the ground truth.

3. **Transformer Model (Optional)**  
   - A Transformer-based encoder-decoder architecture (with positional encoding, multi-head attention, and feed-forward layers) is used for the same mapping task.

*Note: This project is for evaluating symbolic calculation tasks. The LSTM and Transformer models showcase different seq2seq approaches to learning Taylor expansions.*  
