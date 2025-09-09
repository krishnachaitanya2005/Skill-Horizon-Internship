# Step 7: Collect URLs & Filter JS Files

**Tools used:** `gau`, `grep`

## Commands:
```
gau hackthissite.org | tee urls.txt
cat urls.txt | grep "\.js$" | sort -u > js_files.txt
```
Collected URLs archived in Wayback + live sources.

Extracted JavaScript files into `js_files.txt`.
