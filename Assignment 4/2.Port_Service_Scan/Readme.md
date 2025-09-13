# Step 2 – Port & Service Scan

## Objective
Identify open ports, running services, versions, and perform OS detection.

## Target
zero.webappsecurity.com

## Commands Used
```
# Quick SYN scan
nmap -sS -T4 zero.webappsecurity.com

# Service/version + NSE on common ports
nmap -sV -p 22,80,443 -sC zero.webappsecurity.com

# NSE scripts on all ports
nmap -sV -p 1-65535 -sC zero.webappsecurity.com

# Full port scan
nmap -sS -p- zero.webappsecurity.com

# OS detection
nmap -O --osscan-guess zero.webappsecurity.com

