# Assignment 4 – Active Recon & Web Enumeration

## Target
- **Domain:** `zero.webappsecurity.com`  
- **IP:** `54.82.22.214`  

## Steps Performed
1. Checked if the host was alive and noted its IP address.  
2. Scanned the target for open ports and identified running services.  
3. Enumerated web directories and files.  
4. Identified web technologies and performed basic vulnerability checks.  

## Key Findings
- Host is up with Apache-Coyote/1.1 server.  
- Open ports include HTTP (80) and HTTPS (443).  
- Basic directories discovered (listed in attached output).  
- Missing security headers (X-Frame-Options, X-Content-Type-Options) and permissive CORS policy reported by Nikto.  

## Deliverables
- Scan outputs and enumeration results  
- Web fingerprinting and vulnerability scan results  
- Screenshots of relevant findings  

*All tests performed on an authorized target for educational purposes only.*
