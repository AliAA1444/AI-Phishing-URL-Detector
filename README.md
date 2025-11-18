# 🛡️ AI Phishing URL Detector

## 📌 Overview
This project is a Machine Learning solution designed to detect **Phishing URLs** and protect users from cyber threats. It uses a **Random Forest Classifier** to analyze URL features (such as length, special characters, and domain patterns) to distinguish between legitimate and malicious websites.

## 🚀 Features
- **Smart Feature Extraction:** Analyzes URL length, IP presence, and suspicious characters (`@`, `-`).
- **Typosquatting Detection:** Detects fake domains like `amazan-security.com` or `g00gle.com`.
- **Social Engineering Detection:** Identifies sensitive keywords typically used by attackers (e.g., `verify`, `login`, `bonus`).
- **Synthetic Data Generation:** The model is trained on a generated dataset of **10,000+ URLs** to ensure high accuracy and diversity.

## 🛠️ Technologies Used
- **Python** 🐍
- **Scikit-Learn** (Machine Learning)
- **Pandas & NumPy** (Data Processing)

## 💻 How to Run
1. Open the file `Phishing_URL_Detector.ipynb`.
2. Run the cells sequentially.
3. In the final cell, enter any URL to test the detection system in real-time.

## 📊 Sample Result
When testing a malicious link like `http://www.paypal-update-secure.com`:
> **🚨 RESULT: PHISHING / DANGEROUS WEBSITE!**

---
*Developed by Ali Alkhamees - Computer Science Student at Majmaah University.*
