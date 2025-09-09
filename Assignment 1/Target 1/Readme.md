# Target 1 – vulnweb.com

This folder contains the subdomain enumeration results for **[vulnweb.com](http://vulnweb.com)**.

---

## Files

- **vulnweb_subdomain.txt** → Subdomains discovered using `subfinder`.  
- **vulnweb_assetfinder.txt** → Subdomains discovered using `assetfinder`.  
- **vulnweb_alterx.txt** → Mutations/permutations of discovered subdomains generated with `alterx`.

---

## Methodology

1. Collected subdomains with **subfinder**:
   ```
   subfinder -d vulnweb.com >> vulnweb_subdomain.txt
   ```
2. Collected additional subdomains with **assetfinder**:
   ```
   assetfinder -d vulnweb.com >> vulnweb_assetfinder.txt
   ```
3. Generated permutations of discovered subdomains using **alterx**:
   ```
   cat vulnweb_subdomain.txt | alterx | tee vulnweb_alterx.txt
   ```
---

## Notes

The subfinder and assetfinder outputs are based on passive enumeration.

The alterx results include possible subdomain candidates, but they are not guaranteed to be valid.

Further validation with tools like *dnsx* or *httpx* is recommended.
