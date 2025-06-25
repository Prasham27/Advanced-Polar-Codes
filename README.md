# Polar Codes in MATLAB: Advanced Simulation Framework

A fully modular MATLAB toolkit for polar coding—spanning sub‐channel reliability analysis, encoding, channel modeling, and cutting‐edge decoding. Ideal for both classroom demonstrations and research explorations, it lets you benchmark error‐correction performance under a variety of noise conditions.

---

## 🔍 Features Overview

### 1. Sub‐Channel Reliability  
- Computes Bhattacharyya parameters to rank and select which bit‐channels carry information versus which remain frozen.

### 2. Encoder  
- Transforms a message vector (information + frozen bits) into a polar‐encoded codeword ready for transmission.

### 3. Channel Models  
- **BPSK + AWGN**  
  Simulates binary phase‐shift keying transmission over an Additive White Gaussian Noise channel.  
- **Composite Noise**  
  Introduces a blend of Gaussian, Laplace, and Uniform noise distributions to test decoder robustness in realistic interference scenarios.

### 4. Decoding Algorithms  
- **Successive Cancellation (SC)**  
  Implements the baseline SC decoder for polar codes.  
- **CRC-Aided Successive Cancellation List (SCL)**  
  Maintains multiple candidate codewords and employs a CRC check to select the correct one—dramatically boosting error‐correction performance.

### 5. Performance Analytics  
- **BER & BLER Simulations**  
  Scripts to generate bit‐error and block‐error curves across different SNRs, code rates, and block sizes.  
- **Algorithm Comparisons**  
  Side‐by‐side plots contrasting SC vs. CRC-SCL performance gains.  
- **Shannon Limit Benchmarking**  
  Overlays theoretical capacity bounds to gauge coding efficiency.  
- **AWGN vs. Mixed Noise**  
  Visual comparisons highlighting decoder resilience under non‐Gaussian disturbances.

---

## 🚀 Key Advantages

- **Clean, Modular Codebase**  
  Each component (reliability, encoding, channel, decoding) lives in its own well‐documented function—simplifying customization and extension.
- **Enhanced CRC-SCL Decoder**  
  Bridges the gap with state‐of‐the‐art codes (Turbo, LDPC) at finite block lengths by integrating CRC checks into list decoding.
- **Unique Mixed-Noise Channel**  
  The `bpsk_mixed_channel` module enables evaluation of polar codes under composite noise profiles—an uncommon feature in most public implementations.
- **Comprehensive Visualization**  
  Built‐in plotting routines for BER/BLER curves, decoder comparisons, and channel benchmarks make performance insights immediate and clear.

---
