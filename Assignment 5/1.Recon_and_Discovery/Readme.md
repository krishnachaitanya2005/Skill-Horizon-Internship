# Step 1 – Reconnaissance & Discovery

This phase identified the target, its open ports, services, and technologies.

## Tools & Commands

- **Nmap** – scanned for live hosts, open ports and services  
  ```
  nmap -sV testfire.net -o nmap.txt
  ```
- **WhatWeb** – performed web application fingerprinting
  ```
  whatweb testfire.net | tee Whatweb.txt
  ```
- **Dirb** – performed directory and file discovery
  ```
  dirb http://testfire.net/ -o Dirb.txt
  ```
