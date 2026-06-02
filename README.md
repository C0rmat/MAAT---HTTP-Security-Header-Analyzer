# MAAT---HTTP-Security-Header-Analyzer

A lightweight HTTP security header analyzer written in Python. Named after Ma'at, the Egyptian goddess of truth, balance and justice, MAAT helps you evaluate the security posture of web servers by inspecting important HTTP response headers.

Designed for penetration testers, security researchers, students and developers.

## ⚠ Disclaimer

This tool is intended for educational purposes, security research and authorized security assessments only.

Always obtain permission before testing systems you do not own or manage.

##  Features

- Analyzes common HTTP security headers
- Displays HTTP response status codes
- Calculates a security score
- Detects missing security headers
- Handles invalid URLs and failed requests
- Simple command-line interface
- Beginner-friendly and easy to extend

##  Security Headers Checked

- Content-Security-Policy
- X-Frame-Options
- Strict-Transport-Security
- X-Content-Type-Options
- Referrer-Policy
- Permissions-Policy

## Requirements

- Python 3.x
- requests

## Installation

Clone the repository:

```bash
git clone https://github.com/C0rmat/MAAT-HTTP-Header-Analyzer.git
```

Move into the project directory:

```bash
cd MAAT-HTTP-Header-Analyzer
```

Install dependencies:

```bash
pip install requests
```

## Usage

```bash
python3 HTTP_analyzer.py
```

Enter a target URL when prompted:

```text
Please enter a valid URL:
https://example.com
```

## Example Output

```text
Status Code: 200

✅ Content-Security-Policy
✅ X-Frame-Options
✅ Strict-Transport-Security
✅ X-Content-Type-Options
✅ Referrer-Policy
❌ Permissions-Policy

Found: 5/6
Total Security Score: 83%
```

## Pairs Well With

### APEP - Subdomain Enumerator

Use APEP to discover subdomains and then analyze each discovered host with MAAT.

### SOBEK - Directory & File Fuzzer

After finding hidden directories and files with SOBEK, use MAAT to inspect their HTTP security configuration.

## Author

C0rmat
