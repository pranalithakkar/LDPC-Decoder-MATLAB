# LDPC Decoder Simulation Engine (MATLAB)

## Description
This project implements a **Low-Density Parity-Check (LDPC) decoder** in MATLAB.

When we send digital messages (like text or data) over a network, some bits can get lost or erased due to noise. **LDPC codes** are a type of **error-correcting code** that helps detect and fix these errors so the original message can be recovered.

This project focuses on decoding **12-bit messages** sent over a **Binary Erasure Channel (BEC)**, where some bits may be “erased” (unknown) during transmission. The decoder uses a **graph-based approach** with **variable nodes** (representing received bits) and **check nodes** (used to verify correctness) to iteratively reconstruct the original message.

We use **Monte Carlo simulations** (repeating the experiment many times) to measure how reliably the decoder works under different noise conditions.

## Key Features
- Supports **hard and soft decision decoding**, showing different ways to handle missing or uncertain bits.  
- Runs **over 100,000 simulations** to calculate success rates and error trends.  
- **Modular graph-based design**, making it easy to understand the interaction between variable nodes and check nodes.  
- Produces **visualizations** of decoding performance, including convergence and fraction of erased bits.  
- **Validated with analytical models** to ensure the simulation matches theory.
