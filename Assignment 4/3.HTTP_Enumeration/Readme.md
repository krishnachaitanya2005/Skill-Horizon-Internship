# Step 3 – HTTP Enumeration

## Objective
Brute-force directories and files on the web server.

## Target
zero.webappsecurity.com

## Commands Used
```
# Using Brute Force Directories
dirb https://zero.webappsecurity.com

# Using Common Files
dirb https://zero.webappsecurity.com /usr/share/wordlists/dirb/common.txt
