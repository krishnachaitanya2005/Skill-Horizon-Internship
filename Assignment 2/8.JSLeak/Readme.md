# Step 8: Analyze JS Files for Secrets

**Tool used:** `jsleak`

## Command:
```
cat js_files.txt | jsleak -s -l -c 20 -k > jsleak_reports.txt
```
**Result:** *No secrets or sensitive endpoints discovered.*

**Interpretation:** The target’s JS files are secure from common passive leaks.
