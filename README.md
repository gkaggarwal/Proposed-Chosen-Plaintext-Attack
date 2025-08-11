# Chosen-Plaintext Attack on Template-Based TMS Encryption in IJTAG
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)
![Software-Level: Python](https://img.shields.io/badge/Software--Level-Python-3776AB.svg)

This repository contains Python implementations of our experimental setup and analysis presented in our paper on vulnerability assessment of template-based encryption in IJTAG architectures. The scripts demonstrate how an untrusted tester can exploit deterministic structures in the encryption process to compromise scan access through a chosen-plaintext attack.

## 📁 Repository Structure

- `1 Existing_Scheme.ipynb`: Implements the original template-based TMS encryption scheme using a fixed binary pattern and SHAKE-256-generated bitstream.
- `2 Proposed_Attack.ipynb`: Demonstrates the proposed offline attack that recovers the embedding templates used in the encrypted TMS bitstream using only two known plaintext inputs.
- `3 Template_Coverage_Analysis.ipynb`: Statistically analyzes the probability of finding template patterns of varying lengths (1–20 bits) in a 128-bit SHAKE-256-generated random stream.

## 🚀 Getting Started

### Requirements
- Python 3.8+
- No external dependencies beyond the Python standard library

### Running the Code

To run the encryption scheme:

```bash
python 1_encryption_scheme.py
