# DVWA Reflected XSS Testing

## Objective
To test how Reflected XSS behaves at different DVWA security levels (Low, Medium, High) and demonstrate how payloads can be adapted.

## Environment
- Application: DVWA (Damn Vulnerable Web Application)
- Security Levels Tested: Low, Medium, High
- Tools Used:
  - Web browser Firefox

## Steps Performed
### Low Security
1. Set DVWA security to **Low**.
2. Opened **XSS (Reflected)** page.
3. Entered payload `<script>alert('XSS')</script>` directly into the input field.
4. Submission triggered a JavaScript alert box (XSS successful).

### Medium Security
1. Set DVWA security to **Medium**.
2. Entered `<script>alert('XSS')</script>` – blocked / encoded, no alert box.
3. Modified the payload to an image tag:
   ```html
   <img src=x onerror=alert('XSS')>
   ```
4. Submission triggered alert box (XSS successful with img tag).

### High Security
1. Set DVWA security to **High**.
2. Tried `<script>` payload – blocked / encoded, no alert box.
3. Tried the same <img src=x onerror=alert('XSS')> payload again.
4. Submission triggered alert box (XSS still worked).

## Conclusion
**Low:** No sanitization; raw input rendered; <script> executed.  
**Medium:** <script> tags filtered/encoded but event handlers on other HTML elements (like <img>) not fully sanitized.  
**High:** <script> blocked, but <img> payload still executed — filter insufficient to prevent all XSS vectors.  
