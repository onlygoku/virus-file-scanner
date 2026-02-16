
# Educational Virus File Scanner

A modular **educational antivirus scanner** built using Python that demonstrates core malware detection techniques including signature-based scanning, heuristic analysis, multithreaded file inspection, quarantine handling, and automated PDF report generation.

This project is designed for cybersecurity learning, experimentation, and portfolio demonstration.

---

## Features

### Malware Detection Engines

* Signature-based detection using SHA256 hash comparison
* Heuristic analysis for suspicious file behavior
* Multi-engine detection pipeline

### Scanning Capabilities

* Folder (bulk) scanning
* Single file upload scanning
* Recursive directory inspection
* Multithreaded fast scanning

### Security Actions

* Automatic quarantine of detected threats
* Safe file isolation workflow
* Detection logging system

### Reporting System

* JSON scan reports
* Professional PDF scan report export
* Timestamped scan history

### Graphical Interface

* Interactive desktop GUI
* Live scan activity log
* Files scanned counter
* Threat alerts
* One-click PDF report viewer

---

## Project Structure

```
virus-file-scanner/
│
├── app/
│   ├── gui.py
│   ├── scanner_engine.py
│   ├── hashing.py
│   ├── signature_scan.py
│   ├── heuristic_scan.py
│   ├── quarantine.py
│   ├── report_manager.py
│   └── pdf_exporter.py
│
├── data/
│   └── signatures/
│       └── virus_signatures.txt
│
├── reports/
│   ├── scan_reports.json
│   └── scan_report.pdf
│
├── quarantine/
│
├── main.py
└── README.md
```

---

## How It Works

1. User selects a folder or uploads a file to scan.
2. Each file is analyzed using multiple detection engines:

   * Hash signature matching
   * Heuristic inspection
3. Suspicious files are automatically moved to quarantine.
4. Scan results are saved as structured reports.
5. A professional PDF report is generated automatically.

---

## Installation

### Clone Repository

```
git clone https://github.com/onlygoku/virus-file-scanner.git
cd virus-file-scanner
```

### Install Dependencies

```
pip install -r requirements.txt
```

---

## Usage

Run the application:

```
python main.py
```

### Scan Options

* **Select Folder & Scan** → scans all files recursively
* **Select File & Scan** → scans a single uploaded file
* **Open PDF Report** → opens latest generated report

---

## Generated Output

After each scan:

```
reports/
 ├── scan_reports.json
 └── scan_report.pdf

quarantine/
 └── infected_files
```

---

## Detection Techniques Demonstrated

| Technique           | Purpose                                              |
| ------------------- | ---------------------------------------------------- |
| Signature Detection | Matches file hashes against known malware signatures |
| Heuristic Analysis  | Detects suspicious file characteristics              |
| Multithreading      | Improves scanning performance                        |
| Quarantine System   | Prevents execution of malicious files                |
| Automated Reporting | Generates security documentation                     |

---

## Educational Purpose

This project simulates the architecture of a simplified antivirus engine and demonstrates real cybersecurity concepts such as:

* Static malware analysis
* File hashing
* Detection pipelines
* Incident reporting workflows

This is **not a production antivirus** and should be used only for educational purposes.

---

## Future Improvements

* Real-time file monitoring
* Threat severity scoring
* Dark-mode security dashboard
* Cloud signature updates
* Behavioral sandbox simulation

---

## Technologies Used

* Python 3
* Tkinter (GUI)
* ReportLab (PDF generation)
* Concurrent Futures (multithreading)
* SHA256 hashing

---

## Author

Developed by **onlygoku**

GitHub: https://github.com/onlygoku

---

## License

This project is released for educational and research purposes.


