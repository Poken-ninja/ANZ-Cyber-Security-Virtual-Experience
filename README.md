# ANZ Cyber Security Virtual Experience 🛡️

**Platform:** [Forage](https://www.theforage.com/)
**Author:** [Poken-ninja (Pratham M.)](https://github.com/Poken-ninja)
**Repo:** [View on GitHub](https://github.com/Poken-ninja/ANZ-Cyber-Security-Virtual-Experience)

---

## 📌 Overview

This project showcases my participation in the **ANZ Cyber Security Virtual Experience**. I simulated the role of a SOC (Security Operations Center) analyst, where I:

* Investigated network traffic (PCAP files)
* Extracted hidden files (PDFs, ZIPs, JPEGs, Base64)
* Performed forensic analysis on suspicious downloads
* Analyzed phishing emails
* Documented findings in a professional format

---

## 🧠 Skills Gained

* Packet capture analysis using **Wireshark**
* File signature recognition and **hex editing with HxD**
* **Base64 decoding**, ZIP carving, and PDF recovery
* Steganographic clue identification
* Real-world **email phishing detection**
* Secure browsing & password hygiene tips

---

## 🧪 Technical Task Breakdown

### 🔍 Sub-task 1: Extract `anz-logo.jpg` and `bank-card.jpg`

* Used Wireshark → Export HTTP Objects
* Valid JPEG signatures (FFD8)
* Successfully saved and analyzed images

### 🖼️ Sub-task 2: Hidden content in `ANZ1.jpg` & `ANZ2.jpg`

* Found multiple JPEG markers (FFD8–FFD9)
* Possible steganographic data
* Flags covert communication methods

### 📄 Sub-task 3: Suspicious DOCX file (`how-to-commit-crimes.docx`)

* Not a valid Word doc; actually plain text
* Contained malicious guidance
* Transmitted via insecure HTTP

### 📑 Sub-task 4: PDF Extraction (`ANZ_Document.pdf`, `ANZ_Document2.pdf`, `evil.pdf`)

* Reconstructed using hex signature `%PDF-` (25 50 44 46)
* Full extraction using HxD + Wireshark streams
* Saved as working PDFs

### 🧾 Sub-task 5: `hiddenmessage2.txt`

* Image hidden inside a text file
* Extracted by identifying JPEG markers in content
* Illustrates obfuscation techniques

### 🏧 Sub-task 6: `atm-image.jpg`

* Single GET request downloaded two files
* Image content shows cartoon ATMs
* Confirmed valid JPEG with no tampering

### 📦 Sub-task 7: `broken.png` (Base64-encoded)

* No file signature in hex
* Identified ASCII Base64 string (`iVBORw0KGgo...`)
* Decoded online and saved as `.png`

### 🔐 Sub-task 8: `securepdf.pdf` (ZIP → PDF)

* Started with `PK` (50 4B) indicating ZIP
* Extracted with HxD, saved as ZIP
* Unzipped to reveal `securepdf.pdf`, password: `secure`

---

## ✉️ Phishing Email Analysis

I reviewed **7 emails** and analyzed headers, links, urgency, sender reputation, and spoofing techniques.

| Email | Verdict     | Reasoning                                          |
| ----- | ----------- | -------------------------------------------------- |
| 1     | ❌ Malicious | From `.ru` domain, urgency, vague file download    |
| 2     | ✅ Safe      | Personal email, no links, casual context           |
| 3     | ❌ Malicious | Typo-squatting (`facebⓈook`), fake domain          |
| 4     | ✅ Safe      | Marketing email with valid product links           |
| 5     | ❌ Malicious | Fake FBI agent, dramatic scam narrative            |
| 6     | ✅ Safe      | Internal ANZ employee communication                |
| 7     | ❌ Malicious | Phishing insurance promo, fake domain, "hxxp" link |

---

## 🧠 Online Safety & Awareness Takeaways

### Banking & Browsing Tips

* Use **MFA**, avoid public Wi-Fi, and log out after sessions
* Only visit `https://www.anz.com.au` by typing it manually

### Strong Password Hygiene

* Use **12+ char passphrases** (e.g., `PurplePearPrincess`)
* Use a **password manager**
* Never reuse passwords across sites

### Secure Shopping Habits

* Check for **padlock** icon (`https://`)
* Avoid sharing card info via messages
* Verify sellers via **Trustpilot** or reviews

### Identity Theft Red Flags

* Unknown services, credit score drops, rebate notifications
* Spike in spam or scam calls

### Reporting Scams

* [ReportCyber](https://www.cyber.gov.au/report)
* [Scamwatch](https://www.scamwatch.gov.au/)
* [IDCare](https://www.idcare.org/)

---

## 🧭 Why I’m Interested in Cybersecurity

> I recently participated in ANZ's virtual job simulation on Forage, which deepened my interest in cybersecurity.
> I enjoyed identifying phishing emails and decoding PCAP files to find hidden threats.
> This project confirmed that I love investigating complex security problems and want to grow as a cybersecurity professional.

---

## ✅ Status

> **✔ All 8 technical tasks completed**
> **✔ Phishing emails analyzed**
> **✔ Awareness best practices documented**
> **📂 Repo:** [ANZ-Cyber-Security-Virtual-Experience](https://github.com/Poken-ninja/ANZ-Cyber-Security-Virtual-Experience)

