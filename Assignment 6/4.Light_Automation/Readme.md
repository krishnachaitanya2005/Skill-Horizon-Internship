# Step 4 – Light Automation
## Nikto
```
nikto -h http://127.0.0.1:42001/ -o Nikto.txt
```
Found server version, headers, and common misconfigurations.

## WhatWeb
```
whatweb http://127.0.0.1:42001/ | tee Whatweb.txt
```
Identified Apache, PHP, DVWA stack.

## Dirb
```
dirb http://127.0.0.1:42001/ /usr/share/dirb/wordlists/common.txt -o Dirb.txt
```
Enumerated hidden directories.

## Nuclei
```
nuclei -u http://127.0.0.1:42001/ -o Nuclei.txt
```
Template-based scan for known issues.

**Output files:** `Nikto.txt, Whatweb.txt, Dirb.txt, Nuclei.txt`.
