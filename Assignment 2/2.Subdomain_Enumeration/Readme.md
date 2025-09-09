# Step 2: Subdomain Enumeration

**Tools used:** `subfinder`, `assetfinder`, `amass`

## Commands:
```
subfinder -d hackthissite.org | tee subfinder.txt
assetfinder hackthissite.org | tee assetfinder.txt
amass enum -passive -d hackthissite.org
```
## Discovered subdomains included:
`forum.hackthissite.org`, `ctf.hackthissite.org`, `data.hackthissite.org`, `irc.hackthissite.org`, etc.
