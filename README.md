# Day-6-100-Days-challenge-in-cybersecurity-
# Day 06: Recovering Deleted Evidence via Web Archiving

**Topic:** Open Source Intelligence (OSINT), Digital Forensics, Web Archiving  
**Date:** January 2, 2026  
**Tools:** [Wayback Machine](https://archive.org/web/)

---

## 🚩 Challenge Scenario
A scammer executed an **"Exit Scam"**—a tactic where a malicious actor collects money or data from victims and then abruptly shuts down their operations. 

The website was deleted, DNS records were pulled, and visiting the URL resulted in a `404 Not Found` error. The goal of this challenge was to bypass this dead end and retrieve digital evidence of the fraud.

## 🧠 Key Concepts
* **Digital Permanence:** The concept that once information is published online, it is rarely completely erased. It is often cached, indexed, or archived by third parties.
* **Web Archiving:** The process of collecting portions of the World Wide Web to ensure the information is preserved in an archive for future researchers, historians, and investigators.
* **Artifacts:** Specific pieces of data (images, text, code) that serve as evidence.

## 🛠️ Tools Used
* **Wayback Machine (Internet Archive):** A digital library of internet sites that uses crawlers to take "snapshots" of web pages over time.

## 🕵️‍♂️ Investigation Methodology

### Step 1: Identification
I started with the target URL of the now-defunct scam website. Visiting the live link confirmed the server was offline (`404 Error`).

### Step 2: Temporal Analysis
I input the target URL into the **Wayback Machine**.
* **Observation:** The timeline showed activity (black bars) leading up to the exit scam, followed by a sudden cessation of snapshots.
* **Selection:** I selected a snapshot date just prior to the reported shutdown to see the site in its active state.

### Step 3: Retrieval & Extraction
The archived snapshot successfully loaded the deleted content. I extracted the following evidence:
1.  **Fraudulent Claims:** Banners promising "200% Guaranteed Returns" and "Risk-Free" investment.
2.  **Social Engineering:** Fake testimonials used to build trust.
3.  **Contact Indicators:** Support emails and footer addresses that were previously hidden.

## 📉 Findings
| Artifact | Status | Significance |
| :--- | :--- | :--- |
| **Home Page** | Recovered | Proves the site existed and solicited funds. |
| **"About Us"** | Recovered | Contained fake team profiles. |
| **Pricing Page** | Recovered | Detailed the specific financial tiers of the scam. |

## 🎓 Key Takeaways
1.  **Deleting is not erasing:** Taking a server offline does not scrub the internet's memory.
2.  **Time is a dimension in OSINT:** Investigators must look not just at *where* a site is, but *when* it was.
3.  **Preservation is key:** Archiving tools turn temporary web pages into permanent digital evidence.

---

### ⚖️ Disclaimer
*This project is for educational and ethical hacking purposes only. The techniques demonstrated here are intended to assist in legitimate investigations and cybersecurity research. Always adhere to legal guidelines when conducting OSINT.*
