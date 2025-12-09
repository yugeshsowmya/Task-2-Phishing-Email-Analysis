# Task-2-Phishing-Email-Analysis
Complete analysis of a phishing email sample: header extraction, MXToolbox analysis, identification of phishing indicators, and documentation for cybersecurity training.
# Task 2 – Phishing Email Analysis

This project contains a complete analysis of a phishing email sample for the internship submission.  
The objective of this task is to extract the phishing email headers and body, analyze the header information using an online tool, identify phishing indicators, and document the findings clearly.

1. Email Sample
The phishing email used in this task is designed to appear as a **UPS Failed Delivery Notification**.  
It includes:
- Fake UPS branding  
- Urgent delivery message  
- Suspicious tracking link  

The full email body is saved in:
  **phishing-email.txt**

2. Email Header Extraction
The email header was manually extracted and saved as:
   **email-header.txt**

These headers were later uploaded to an online email header analyzer.

3. Header Analysis (MXToolbox)
The header was analyzed using the online tool:

 https://mxtoolbox.com/EmailHeaders.aspx

Key Results:
- ❌ **DMARC Not Compliant**  
- ❌ **SPF Not Authenticated**  
- ❌ **DKIM Not Authenticated**  
- ❌ **DKIM Alignment Failed**  
- ✔ **SPF Alignment Passed (partially)**  

These authentication failures strongly indicate that the email was sent from an unauthorized or spoofed mail server.

The full analysis screenshot is uploaded as:
  **header-analysis.png**

4. Phishing Indicators Identified
A detailed list of suspicious elements was documented in:
 **phishing-indicators.txt**

Summary of Indicators:
- Suspicious sender email (`amazon@update-nt.com`)  
- Mismatched branding (Amazon email pretending to be UPS)  
- Urgent language (“48 hours”)  
- Suspicious tracking link  
- Generic greeting  
- Grammar issues  
- Failed SPF, DKIM, and DMARC  
- Unrelated domain (`update-nt.com`)  
- Unknown mail server IP address  

These indicators collectively confirm that the email is a phishing attempt.

5. Screenshots Included
  **email-screenshot.png** — Screenshot of the phishing email  
  **header-analysis.png** — Screenshot of the MXToolbox result  

 📁 Folder Structure
 
Final Notes
This repository contains all required files for Task 2 submission.  
The analysis demonstrates how to inspect email headers, identify suspicious patterns, and recognize phishing techniques.



