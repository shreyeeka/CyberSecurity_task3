# Task 3: Analyze a Phishing Email Sample

## Objective:
Identify phishing characteristics in a suspicious email sample

## Tools:
- **Email client or saved email file (text)**
- **Free online header analyzer (e.g. [MX toolbox](https://mxtoolbox.com/EmailHeaders.aspx))**

## Guide
1. Obtain a sample phishing email (many free samples online)
2. Examine sender's email address for spoofing
3. Check email headers for discrepancies (using online header analyzer)
4. Identify suspicious links or attachments
5. Look for urgent or threatening language in the email body
6. Note any mismatched URLs (hover to see real link)
7. Verify presence of spelling or grammar errors
8. Summarize phishing traits found in the email

---

## Sample Email
- **[phishing_sample.eml](phishing_sample.eml)**

![Alt Text](images/SampleEmail.PNG)

---

## Executive summary
This report analyzes a synthetic phishing email sample (phishing_sample.eml) created for training. The message simulates a PayPal-themed credential phishing attempt and exhibits multiple classic phishing indicators: spoofed sending domain, suspicious hosting IP, urgent/pressure language, and a mismatched suspicious link

---

## Raw header (extracted)
- **To extract headers, in my case (macOS), the mentioned command is used:**
    - sed -n '1,/^$/p' phishing_sample.eml > phishing_headers.txt
    - cat phishing_headers.txt ([Extracted header](phishing_headers.txt))

![Alt Text](images/HeaderExtract.PNG) 

---

## Header Analysis
1. Open [MXToolbox](https://mxtoolbox.com/EmailHeaders.aspx).
2. Inside email header analyzer, paste the contents of [phishing_headers.txt](phishing_headers.txt) (or the header block) into the box.
3. Click Analyze Header.

![Alt Text](images/HeaderAnalysis.png)

- **Analyzed Reports:**
![Alt Text](images/AnalysisReportI.png)
![Alt Text](images/AnalysisReportII.png)

