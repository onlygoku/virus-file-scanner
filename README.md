# Static Virus File Scanner

## Overview
This project is a Python-based static virus file scanner designed to analyze files safely without executing them.

The scanner detects potentially malicious files using signature matching, hash-based identification, and heuristic analysis. It is intended for learning antivirus fundamentals and blue-team security workflows.

---

## Key Features
- Static file scanning without execution
- Virus signature based detection
- Hash based malware identification
- Heuristic analysis for suspicious patterns
- JSON scan report generation
- Modular and extensible architecture
- No third-party libraries required

---

## Project Structure
virus_file_scanner/
├── scanner/
│ ├── init.py
│ ├── signature_scanner.py
│ ├── hash_scanner.py
│ └── heuristic_scanner.py
├── signatures/
│ └── virus_signatures.txt
├── samples/
│ └── test_file.bin
├── reports/
│ └── scan_report.json
├── main.py
└── README.md


---

## How It Works

### Signature Scanning
Scans files for known malicious byte patterns stored in a signature database.

### Hash Scanning
Calculates cryptographic hashes and compares them against known malicious hashes.

### Heuristic Analysis
Detects suspicious indicators such as command execution strings and network related keywords.

---

## Technologies Used
- Python
- hashlib
- json
- os

All components rely on the Python standard library only.

---

## How to Run

1. Place a file inside the `samples` directory
2. Rename it to:
3. Run the scanner:
```bash
python main.py
