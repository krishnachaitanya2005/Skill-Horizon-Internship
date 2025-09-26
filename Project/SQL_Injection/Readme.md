# DVWA SQL Injection Testing

## Objective
To test how SQL Injection behaves at different DVWA security levels (Low, Medium, High) and demonstrate interception/modification of requests using Burp Suite.

## Environment
- Application: DVWA (Damn Vulnerable Web Application)
- Security Levels Tested: Low, Medium, High
- Tools Used:
  - Web browser Firefox
  - **Burp Suite** (for intercepting and modifying HTTP requests)

## Steps Performed
### Low Security
1. Set DVWA security to **Low**.
2. Opened **SQL Injection** page in the browser.
3. Entered payload `' OR '1'='1` directly into the input field.
4. Submission returned full list of users (SQL injection worked). Took screenshots.

### Medium Security
1. Set DVWA security to **Medium**.
2. Entered the same payload in the browser – attack failed / input sanitised.
3. Enabled **Burp Suite** proxy, intercepted the HTTP request.
4. Modified the parameter to `OR 1=1%23` (URL-encoded “OR 1=1#”) to bypass filtering.
5. Forwarded the modified request – additional records were retrieved, confirming SQLi worked with adjusted payload.

### High Security
1. Set DVWA security to **High**.
2. Tried the previous payloads both directly and via Burp Suite.
3. All attempts blocked; only normal responses shown.

## Conclusion
- **Low:** No input validation or parameterization – raw SQL query executed with attacker input.
- **Medium:** Basic sanitization blocks trivial payloads in browser, but a slightly modified payload via Burp Suite still works.
- **High:** Proper parameterized queries implemented – no SQLi possible even with modified payloads.
