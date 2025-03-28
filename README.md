# Performance Benchmarking of Cryptographic Mechanisms

## Overview
This project benchmarks the performance of different cryptographic mechanisms, specifically measuring the time required for AES, RSA, and SHA-256 operations on files of varying sizes. The goal is to analyze encryption, decryption, and hashing efficiency using Python.

## Authors
- Alexandre Furriel
- Henrique Teixeira
- João Ferreira

## Technologies Used
- **Python** (Primary language for implementation)
- **cryptography** module ([hazmat primitives](https://cryptography.io/en/latest/hazmat/primitives/))
- **timeit** (For performance measurement)
- **Matplotlib** (For data visualization)

## Benchmarking Tasks

### 1. File Generation
Random text files of the following sizes are generated:
- **AES & SHA-256**: 8B, 64B, 512B, 4KB, 32KB, 256KB, 2MB
- **RSA**: 2B, 4B, 8B, 16B, 32B, 64B, 128B

### 2. AES Encryption & Decryption
- Uses a **256-bit key** for encryption and decryption.
- Execution time measured for each file size.
- Results analyzed for statistical significance.

### 3. RSA Encryption & Decryption
- Uses a **2048-bit key** (minimum recommended for RSA).
- Execution time measured for each file size.

### 4. SHA-256 Hashing
- Hashing execution time is measured for each file size.

## Performance Analysis
The following comparisons are included:
- **AES vs. RSA encryption performance**
- **AES encryption vs. SHA-256 hashing performance**
- **RSA encryption vs. RSA decryption performance**

## Results & Visualization
- The report includes **plots** comparing performance.
- The x-axis represents **file size (bytes)**, while the y-axis represents **execution time (μs)**.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/johnpierrre/CryptoAlgs_testing/
   cd src
   ```
2. Install dependencies:
   ```bash
   pip install cryptography matplotlib
   ```
3. Open the Jupyter Notebook file.

4. View the results in the generated report.

## Submission
This project is part of **Security and Privacy** coursework. The final report, including implementation details and analysis, is submitted on Moodle.
