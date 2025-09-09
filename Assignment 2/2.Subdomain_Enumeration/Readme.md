# Step 2: Subdomain Enumeration

**Tools used:** `subfinder`, `assetfinder`, `amass`

## Commands:
```
subfinder -d hackthissite.org -o subfinder.txt
assetfinder hackthissite.org | tee assetfinder.txt
amass enum -passive -d hackthissite.org -o amass.txt
cat subfinder.txt assetfinder.txt amass.txt | sort -u > subdomains.txt
```
## Discovered subdomains included:
`forum.hackthissite.org`, `ctf.hackthissite.org`, `data.hackthissite.org`, `irc.hackthissite.org`, etc.
