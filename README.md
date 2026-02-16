# Educational Virus Scanner

A modular **educational antivirus prototype** built in Python that demonstrates core malware detection techniques including signature scanning, heuristic analysis, multithreaded file inspection, quarantine handling, and automated PDF reporting.

This project is designed for cybersecurity learning and portfolio demonstration purposes.

---

## Features

### Detection Engines

* Signature-based malware detection using SHA256 hashes
* Heuristic detection for suspicious file behavior
* Multi-engine scanning pipeline

### Scanning System

* Recursive directory scanning
* Multithreaded fast scan mode
* Live scan progress logging
* Automatic infected file quarantine

### Reporting

* JSON scan report generation
* Professional PDF security report export
* Timestamped scan history

### Graphical Dashboard

* Folder selection interface
* Live scan activity log
* Files scanned counter
* Threat detection alerts
* One-click PDF report viewer

---

## Project Structure

```
virus-scanner/
│
├── app/
│   ├── hashing.py
│   ├── signature_scan.py
│   ├── heuristic_scan.py
│   ├── scanner_engine.py
│   ├── quarantine.py
│   ├── report_manager.py
│   ├── pdf_exporter.py
│   └── gui.py
│
├── data/
│   └── signatures/
│       └── virus_signatures.txt
│
├── reports/
│   └── scan_reports.json
│
├── quarantine/
│
├── main.py
└── README.md
```

---

## How It Works

1. The scanner walks through all files inside a selected directory.
2. Each file is analyzed using multiple detection engines:

   * Hash signature comparison
   * Heuristic inspection
3. Detected threats are automatically moved to quarantine.
4. Results are saved as:

   * JSON structured report
   * PDF security report
5. GUI displays live scan progress and results.

---

## Installation

### 1. Clone Repository

```
git clone https://github.com/onlygoku/virus-file-scanner.git
cd virus-file-scanner
```

### 2. Install Dependencies

```
pip install -r requirements.txt
```

---

## Usage

Run the application:

```
python main.py
```

Steps:

1. Click **Select Folder & Scan**
2. Choose a directory
3. Monitor live scanning progress
4. View results and open generated PDF report

---

## Generated Outputs

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

| Technique           | Description                                              |
| ------------------- | -------------------------------------------------------- |
| Signature Detection | Matches file hashes against known malware signatures     |
| Heuristic Analysis  | Flags suspicious extensions and abnormal file properties |
| Multithreading      | Parallel file scanning for faster analysis               |
| Quarantine System   | Safely isolates detected threats                         |
| Automated Reporting | Generates structured and printable scan reports          |

---

## Educational Purpose

This project simulates how real antivirus engines structure their scanning pipeline.
It is intended for:

* Cybersecurity learning
* Malware analysis fundamentals
* Python security tooling practice
* Portfolio demonstration

This is **not a production antivirus** and should not be used as a primary security solution.

---

## Future Improvements

* Real-time file monitoring
* Threat severity scoring
* Dark mode dashboard
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

Developed as a cybersecurity learning project.

---

## License

This project is released for educational use.



