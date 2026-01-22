# Chosen-Plaintext Attack on Template-Based TMS Encryption in IJTAG
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)
![Software-Level: Python](https://img.shields.io/badge/Software--Level-Python-3776AB.svg)

This repository contains Python implementations of our experimental setup and analysis presented in our paper on vulnerability assessment of template-based encryption in IJTAG architectures. The scripts demonstrate how an untrusted tester can exploit deterministic structures in the encryption process to compromise scan access through a chosen-plaintext attack.

## 📌 Citation (If you use this code)
If you use this repository (code, scripts, or experimental methodology) in your research, please cite our paper:

**Gaurav Kumar, Pardeep Kumar, Anuj Kumar, Raj Kumar Choudhary, and Satyadev Ahlawat.**  
“On Evaluating the Security of Complete Access Protocol of IJTAG Architecture”.  
*In 59th International Symposium on Circuits and Systems Conference (ISCAS 2026), Shanghai, China, May 24–27, 2026.*

## BibTeX
<pre>
@inproceedings{KumarISCAS2026IJTAG,
  author    = {Gaurav Kumar and Pardeep Kumar and Anuj Kumar and Raj Kumar Choudhary and Satyadev Ahlawat},
  title     = {On Evaluating the Security of Complete Access Protocol of IJTAG Architecture},
  booktitle = {Proceedings of the 59th International Symposium on Circuits and Systems (ISCAS 2026)},
  address   = {Shanghai, China},
  month     = may,
  year      = {2026},
  note      = {Just Accepted}
}
</pre>

## 📁 Repository Structure

- `1 Existing_Scheme.ipynb`: Implements the original template-based TMS encryption scheme using a fixed binary pattern and SHAKE-256-generated bitstream.
- `2 Proposed_Attack.ipynb`: Demonstrates the proposed offline attack that recovers the embedding templates used in the encrypted TMS bitstream using only two known plaintext inputs.
- `3 Template_Coverage_Analysis.ipynb`: Statistically analyzes the probability of finding template patterns of varying lengths (1–20 bits) in a 128-bit SHAKE-256-generated random stream.
- `4 Proposed_Scheme.ipynb`: The session depended LFSR based template generation and SHAKE‑driven sequential embedding countermeasure (LSB‑first embedding)


## 🚀 Getting Started

### Requirements
- Python 3.8+
- No external dependencies beyond the Python standard library

### Running the Code

To run the encryption scheme:

```bash
python 1_encryption_scheme.py

## 🛠️ License

This project is licensed under the [MIT License](LICENSE).

