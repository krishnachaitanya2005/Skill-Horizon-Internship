# Project 1 – DVWA Security Level Comparison

## Objective
Compare how DVWA behaves at different security levels (Low, Medium, High) for two common vulnerabilities: **SQL Injection** and **Reflected XSS**.

## Environment
- DVWA (Damn Vulnerable Web Application)
- Kali Linux
- Browsers: Firefox

## Tasks Performed
- Tested **SQL Injection** at Low, Medium, High.
- Tested **Reflected XSS** at Low, Medium, High.
- Documented payloads, observations, and screenshots.

## Report
A detailed **Project Report** has been created alongside this README.  
It includes:
- Full methodology
- Screenshots of successful and failed attacks
- Analysis of defense mechanisms added at higher security levels
- Final conclusions and recommendations

## Summary of Findings
| Vulnerability | Low Security | Medium Security | High Security |
|---------------|--------------|-----------------|---------------|
| SQL Injection | Works (data dumped) | Works (data dumped) | Mitigated / escaped |
| Reflected XSS | Works (alert box) | Works (alert box) | Works (alert box) |

## Conclusion
DVWA at **Low** security level is intentionally vulnerable, but at **Medium** and **High** levels it implements defenses such as input validation, output encoding, and parameterized queries.  
This project demonstrates how basic security mechanisms can prevent common web vulnerabilities.
