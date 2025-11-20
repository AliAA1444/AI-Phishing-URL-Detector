# 🛡️ Enterprise AI Phishing URL Detector

## 📌 Overview
A hybrid cybersecurity tool designed to detect malicious and phishing URLs with high precision. Unlike traditional blacklists, this system combines a **Trusted Whitelist Engine** with a **Random Forest Machine Learning Model** to analyze URL patterns, typosquatting, and entropy.

## 🧠 Key Capabilities
1.  **Hybrid Protection:** Uses a "Whitelist First" approach for guaranteed safety on trusted sites (e.g., GitHub, Google), followed by AI analysis for unknown links.
2.  **Smart Typosquatting Detection:** Detects sophisticated impersonation attacks like `gilhub.com` vs `github.com` or `amazan.com`.
3.  **Generalization Power (Zero-Shot Detection):**
    * The model successfully identified legitimate educational domains (e.g., `ksu.edu.sa`, `imamu.edu.sa`, `ncc.gov.sa`) as **Safe** without explicitly seeing them in the training data or whitelist.
    * This proves the AI understands the "pattern" of legitimate governmental and educational infrastructures.

## 🛠️ Technologies Used
- **Python** (Core Logic)
- **Scikit-Learn** (Random Forest Classifier)
- **Feature Engineering** (Levenshtein Distance, Shannon Entropy, Domain Parsing)

## 🚀 How It Works
The system extracts 9 key features from any URL, including:
- **Brand Imitation Score:** Checks if the URL looks like a famous brand (e.g., `absber.sa` vs `absher.sa`).
- **Entropy:** Detects random generated domains (e.g., `xkqz.xyz`).
- **Structure Analysis:** Differentiates between safe paths (`jarir.com/products/laptop`) and malicious subdomains (`amazon-security.com`).

## 📊 Demo Results
- `https://github.com` 🟢 **Safe** (Whitelist Verified)
- `http://gilhub.com` 🔴 **Phishing** (Detected Typosquatting)
- `https://ksu.edu.sa` 🟢 **Safe** (AI Verified Pattern)
- `http://ww38.gilhub.com` 🔴 **Phishing** (Deep Subdomain Scan)

---
*Developed by Ali Alkhamees - Computer Science Student at Majmaah University.*
