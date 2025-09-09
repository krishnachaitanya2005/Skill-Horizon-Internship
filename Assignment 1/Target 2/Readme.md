# Target 2 – testfire.net

This folder contains the subdomain enumeration results for **[testfire.net](http://testfire.net)**.

---

## Files

- **testfire_subdomain.txt** → Subdomains discovered using `subfinder`.  
- **testfire_assetfinder.txt** → Subdomains discovered using `assetfinder`.  
- **testfire_alterx.txt** → Mutations/permutations of discovered subdomains generated with `alterx`.

---

## Methodology

1. Collected subdomains with **subfinder**:
   ```
   subfinder -d testfire.net >> testfire_subdomain.txt
   ```
2. Collected additional subdomains with **assetfinder**:
   ```
   assetfinder -d testfire.net >> testfire_assetfinder.txt
   ```
3. Generated permutations of discovered subdomains using **alterx**:
   ```
   cat testfire_subdomain.txt | alterx | tee testfire_alterx.txt
   ```
   
---

## Notes

The subfinder and assetfinder outputs are based on passive enumeration.

The alterx results include possible subdomain candidates, but they are not guaranteed to be valid.

Further validation with tools like *dnsx* or *httpx* is recommended.
