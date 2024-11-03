# CUDA Warp Divergence Example

This repository provides a CUDA example demonstrating **warp divergence**.

## Overview

The program includes two kernels:
- **`code_without_divergence`**: Avoids warp divergence by aligning thread execution paths within each warp.
- **`code_with_divergence`**: Introduces warp divergence as threads in the same warp take different paths based on conditions.

## Execution

The kernels are launched with a grid and block configuration, and the program synchronizes after each kernel.
