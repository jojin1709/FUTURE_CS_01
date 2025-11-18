🛡️ FUTURE_CS_01
A Future Interns Internship Program – Cyber Security Track
Task 1: Web Application Security Testing (OWASP Juice Shop)

Intern: Jojin John
Project: Future Interns — Cyber Security Internship
Date: 2025-11-18

🔍 Summary

Performed a hands-on web application security assessment on a local OWASP Juice Shop instance. Identified a stored input handling issue in the product review feature where a malicious payload was accepted and stored by the server. All findings, evidence, and remediation recommendations are included in this repository.

🧩 What I Did

● Deployed OWASP Juice Shop locally using Docker.

● Analyzed the product review submission workflow.

● Used Burp Suite (Proxy + Repeater) to intercept, modify, and replay HTTP requests.

● Injected a crafted payload and confirmed server-side acceptance (201 Created).

● Captured UI screenshots and complete HTTP request/response logs.

● Prepared a concise, actionable security report with impact analysis and remediation steps.

🛠️ Tools Used

● OWASP Juice Shop (Docker image)

● Burp Suite Community Edition — Proxy, HTTP History, Repeater

● Web Browsers: Chromium / Firefox (configured with Burp CA)

● Docker & basic Linux shell utilities

● Markdown → PDF for report creation

🧪 Lab: Quick Reproduction (Local, Safe Environment)

Note: All testing was performed in a controlled lab. Do not target external or production systems.

Start Juice Shop

    docker run --rm -d -p 3000:3000 bkimminich/juice-shop

Configure Browser

● Set proxy to 127.0.0.1:8080 (Burp Suite)

● Install Burp CA certificate for HTTPS interception

In Burp Suite

● Ensure Proxy → Options has listener on 127.0.0.1:8080

● Keep Intercept OFF

● Use HTTP History and Repeater for manipulation

Open Product Page


    http://localhost:3000/#/product/5

Modify Review Submission Payload

    {
    "message": "<script>alert('XSS-POC')</script>",
    "author": "you@example.com"
    }


● Send via Repeater

● Confirm 201 Created with { "status": "success" }

● Refresh UI to verify stored payload

📁 Evidence Included

All captured artifacts are available under the evidence/ folder:

● Screenshots of the UI

● Full HTTP request/response logs

● Burp Suite proxy captures

.Proof-of-Concept payload behavior
