# Step 2 – Light Automated Scans

Automated, non-destructive scanners run on the target to identify common issues.

## Tools & Commands

- **Nikto** – HTTP server misconfigurations  
  ```
  nikto -h http://testfire.net -output Nikto.txt
  ```
- **Nuclei** – template-based security checks
  ```
  nuclei -u http://testfire.net -as -o nuclei.txt -c 10
  ```
- **OWASP ZAP (Baseline)** – passive vulnerability scan

We used the ZAP GUI because the CLI script was not available. Steps:

1. **Launched ZAP GUI:**
    ```
    cd ~/zap-cli/ZAP_2.16.1
    ./zap.sh
    ```
2. Went to “Quick Start” → “Automated Scan”, entered `http://testfire.net`, and started the scan.

3. Exported the csv report from Report → Generate csv Report and saved it as Zap.csv.

- **WPScan** – only if WordPress detected
  ```
  wpscan --url testfire.net
  ```
