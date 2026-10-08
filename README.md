# ReconX — Web Reconnaissance & Security Intelligence Platform

ReconX is a web-based cybersecurity reconnaissance tool that automates DNS enumeration, subdomain discovery, HTTP reconnaissance, technology detection, security-header analysis, TLS inspection, endpoint discovery, and basic port scanning.

## Features

- DNS Reconnaissance
- Subdomain Discovery
- HTTP/HTTPS Reconnaissance
- Technology Detection
- Security Header Analysis
- TLS/SSL Analysis
- Endpoint Discovery
- TCP Port Scanning
- JSON, PDF & TXT Reports
- Web-based Dashboard

## Tech Stack

- **Backend:** Python, Flask
- **Frontend:** HTML, CSS, JavaScript
- **Libraries:** Requests, dnspython, BeautifulSoup4, ReportLab

## Project Structure

```text
ReconX/
├── Backend/
│   ├── app.py
│   ├── recon_engine.py
│   ├── dns_recon.py
│   ├── subdomain_recon.py
│   ├── http_recon.py
│   ├── technology.py
│   ├── headers.py
│   ├── tls_recon.py
│   ├── endpoint_recon.py
│   ├── port_scanner.py
│   ├── reporter.py
│   ├── report_export.py
│   ├── requirements.txt
│   └── reports/
│
├── Frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
│
└── README.md
```

# How to Run on Any PC

## 1. Install Python

Install **Python 3.10 or newer**.

Check the installation:

```bash
python --version
```

If required:

```bash
python3 --version
```

## 2. Download the Project

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/ReconX.git
cd ReconX
```

Or download the ZIP from GitHub and extract it.

## 3. Go to Backend

```bash
cd Backend
```

## 4. Create Virtual Environment

### Windows

```bash
python -m venv .venv
.venv\Scripts\activate
```

### Linux/macOS

```bash
python3 -m venv .venv
source .venv/bin/activate
```

## 5. Install Dependencies

```bash
pip install -r requirements.txt
```

## 6. Start the Backend

```bash
python app.py
```

The backend will run at:

```text
http://127.0.0.1:5000
```

Check the API:

```text
http://127.0.0.1:5000/api/health
```

## 7. Open the Frontend

Open the following file in your browser:

```text
Frontend/index.html
```

Make sure the backend is running before starting a scan.

# Scan Modes

### Passive

Performs reconnaissance without port scanning.

### Active

Performs reconnaissance with TCP port scanning.

### Full

Runs the complete reconnaissance workflow.

# Reports

Reports are stored in:

```text
Backend/reports/
```

Supported formats:

- JSON
- PDF
- TXT

# Quick Setup

### Windows

```bash
git clone https://github.com/YOUR_USERNAME/ReconX.git
cd ReconX/Backend
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

Then open:

```text
Frontend/index.html
```

### Linux/macOS

```bash
git clone https://github.com/YOUR_USERNAME/ReconX.git
cd ReconX/Backend
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python app.py
```

Then open:

```text
Frontend/index.html
```

# Requirements

Python packages required:

```text
Flask
Flask-Cors
requests
dnspython
beautifulsoup4
reportlab
```
