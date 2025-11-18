🛡️ FUTURE_CS_01
Web Application Security Testing – Task 1

Future Interns – Cyber Security Internship
Intern: Jojin John

📘 Overview

This repository contains the deliverables for Task 1: Web Application Security Testing completed as part of the Future Interns Cyber Security Internship Program.
The objective of this task was to assess a vulnerable web application, identify security weaknesses based on OWASP best practices, and prepare a detailed professional security report.

🎯 Objectives

Deploy and interact with an intentionally vulnerable web application (OWASP Juice Shop).

Perform manual and assisted testing using tools such as Burp Suite Community Edition.

Identify and validate security issues including Stored XSS, insecure input handling, and potential injection points.

Map findings to relevant categories from the OWASP Top 10 (2021).

Document technical evidence, HTTP traffic, risk assessment, and remediation recommendations.

🧰 Tools & Environment

OWASP Juice Shop (Local Docker deployment)

Burp Suite Community Edition (Proxy, HTTP History, Repeater)

Docker Engine

Chromium/Firefox with proxy configuration

Kali Linux (optional)

Microsoft Word / PDF for final report

🧪 Testing Scope

The assessment focused on evaluating the following areas:

Input validation and sanitization gaps

Stored Cross-Site Scripting (XSS) risks

Potential injection vectors

Unsafe output rendering

Application misconfigurations

Vulnerability exposure based on OWASP guidelines

📁 Repository Structure

    FUTURE_CS_01/
    │
    ├── report/
    │     └── Task_1_Report.docx        # Full professional security report
    │
    ├── evidence/
    │     ├── request-burp.xml          # Captured HTTP request (Base64)
    │     ├── response-burp.xml         # Captured HTTP response (Base64)
    │     └── screenshots/                # Visual PoC evidence
    │
    └── README.md                       # Summary of the project

📄 Security Report

The complete Security Assessment Report containing:

Executive summary

Vulnerability description

Reproduction steps

Technical evidence

Risk impact

OWASP mapping

Recommended remediation

is available here:
📌 /report/Task_1_Report.docx

🏁 Conclusion

This task provided end-to-end exposure to the workflow followed by cybersecurity analysts and penetration testers. It strengthened my understanding of vulnerability identification, documentation, and secure development practices.
