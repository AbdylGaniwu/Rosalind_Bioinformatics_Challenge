# Rosalind Bioinformatics Challenge Solutions

Welcome to my rolling repository dedicated to solving computational biology problems from the [Rosalind](https://rosalind.info/) platform. This project serves as an active, weekly sandbox for sharpening my skills in algorithm design, scientific thinking, and Python programming applied to genomics and molecular biology.

🔄 **Status:** *Actively Updated Weekly* — New problem solutions and data-driven scripts are added every week as I progress through the challenge.

## 📌 Repository Overview

Bioinformatics bridges the gap between massive biological datasets and computational insights. The scripts in this repository focus on processing genetic sequences efficiently, implementing core algorithms for DNA/RNA manipulation, and optimizing string operations for long sequences.

## 🛠️ Tech Stack & Concepts
* **Language:** Python 3.x
* **Core Libraries Used:** `collections` (for high-performance string counting), standard built-ins (`str.translate`, list comprehensions).
* **Key Skills:** String manipulation, genomic sequence processing, optimization for single-pass data processing, and dictionary mappings.

---

## 🗓️ Weekly Progress Log

| Week | Problem Solved | Core Concept / Algorithm | Status |
| :--- | :--- | :--- | :--- |
| **Week 1** | Counting DNA Nucleotides | String counting & Performance Tuning |  Completed |
| **Week 1** | Transcribing DNA into RNA | Sequence Transcription (`.replace()`) |  Completed |
| **Week 1** | Complementing a Strand of DNA | Reverse Complements (`str.maketrans`) |  Completed |
| **Week 2** | *Upcoming Challenge* | *Dynamic Programming / Alignment* | ⏳ In Progress |

---

## 🧬 Solved Problems Detailed

### 1. Counting DNA Nucleotides
* **Problem Link:** [Rosalind - DNA](https://rosalind.info/problems/dna/)
* **Objective:** Given a DNA string, count the individual occurrences of the symbols 'A', 'C', 'G', and 'T'.
* **Approach:** Implemented both a clean generator expression using standard `.count()` and a high-performance, single-pass dictionary counter (`collections.Counter`) suited for larger chromosomal datasets.

### 2. Transcribing DNA into RNA
* **Problem Link:** [Rosalind - RNA](https://rosalind.info/problems/rna/)
* **Objective:** Transcribe a given DNA strand into its corresponding RNA strand by replacing all occurrences of Thymine (`T`) with Uracil (`U`).
* **Approach:** Handled efficiently using Python's native `.replace()` string method.

### 3. Complementing a Strand of DNA
* **Problem Link:** [Rosalind - REVC](https://rosalind.info/problems/revc/)
* **Objective:** Find the reverse complement of a DNA string, adhering to the biological standard of writing sequences in the $5'$ to $3'$ direction.
* **Approach:** Avoided chained replacements by using a simultaneous translation mapping via `str.maketrans()` combined with C-level string slicing (`[::-1]`) for an optimal, lightning-fast execution.

---

## 🚀 How to Run the Solutions

Ensure you have Python installed on your machine. You can run any of the solution scripts directly from your terminal:

```bash
python solution_name.py
