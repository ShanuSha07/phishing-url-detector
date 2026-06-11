# Phishing URL Detector

A simple rule-based cybersecurity project developed using Python to identify potentially malicious URLs. The tool analyzes URLs based on common phishing indicators and classifies them as Safe, Suspicious, or Phishing.

## Features

* Detects suspicious keywords commonly used in phishing attacks
* Checks whether HTTPS is used
* Identifies URLs containing IP addresses instead of domain names
* Detects the use of the '@' symbol trick
* Analyzes URL length
* Detects possible typosquatting attempts
* Identifies excessive subdomains
* Generates a phishing risk score
* Provides reasons for the classification

## Technologies Used

* Python
* Regular Expressions (re)

## Project Structure

```text
Phishing-URL-Detector/
│
├── phishing_detector.py
├── README.md
├── requirements.txt
└── screenshots/
    ├── safe_url.png
    ├── suspicious_url.png
    └── phishing_url.png
```

## How It Works

The detector evaluates a URL against multiple phishing indicators:

1. Suspicious keywords
2. Long URL detection
3. Presence of '@' symbol
4. IP address usage
5. HTTPS validation
6. Misspelling and typosquatting patterns
7. Excessive subdomains

Based on the calculated score:

| Score | Result         |
| ----- | -------------- |
| 0 - 1 | SAFE URL       |
| 2 - 4 | SUSPICIOUS URL |
| 5+    | PHISHING URL   |

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/phishing-url-detector.git
```

Navigate to the project folder:

```bash
cd phishing-url-detector
```

## Run the Project

```bash
python phishing_detector.py
```

## Example

### Input

```text
http://secure-login-update.example.com
```

### Output

```text
🔍 Analysis Result

⚠️ SUSPICIOUS URL

Reasons:
- Contains suspicious keyword
- Does not use HTTPS
```

## Screenshots

### Safe URL Detection

![Safe URL](screenshots/safe_url.png)

### Suspicious URL Detection

![Suspicious URL](screenshots/suspicious_url.png)

### Phishing URL Detection

![Phishing URL](screenshots/phishing_url.png)

## Future Enhancements

* Machine Learning based phishing detection
* Domain reputation analysis
* WHOIS lookup integration
* Blacklist verification
* URL shortening service detection
* Real-time threat intelligence integration
* GUI version using Tkinter

## Learning Outcomes

Through this project, I gained hands-on experience in:

* Cybersecurity fundamentals
* Phishing attack indicators
* Python programming
* Regular Expressions
* Rule-based threat detection
* Risk scoring systems

## Author

Shalini S

Aspiring Cybersecurity Analyst | Data Analyst | Python Enthusiast
