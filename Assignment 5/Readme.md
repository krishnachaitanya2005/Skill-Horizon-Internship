# Assignment 5 – Automated Web Application Scanning

This assignment demonstrates automated vulnerability discovery on an authorised target.

## Target
- **testfire.net** (publicly approved test application)

## Objective
Perform safe, legal vulnerability scanning of a web application using automated tools, then produce a professional vulnerability report with remediation advice.

## Steps Performed
1. **Recon & Discovery:** Identified open ports, services and technologies using Nmap, WhatWeb, and Dirb.
2. **Light Automated Scans:** Ran Nikto, Nuclei, and OWASP ZAP (GUI baseline scan). Ran WPScan if WordPress was detected.
3. **Validation:** Reviewed scanner results and removed false positives.
4. **Reporting:** Compiled findings and generated a report.

## Tools Used
- Nmap  
- WhatWeb  
- Dirb  
- Nikto  
- Nuclei  
- OWASP ZAP GUI  
- WPScan

## Deliverables
- Scan outputs (Nmap.txt, Whatweb.txt, Dirb.txt, Nikto.txt, Nuclei.txt, Wpscan.txt, Zap.csv)
- Final vulnerability report summarising confirmed issues.
