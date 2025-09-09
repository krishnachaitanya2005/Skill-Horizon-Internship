# Step 1: Domain Information Gathering

**Tools used:** `whois`, `nslookup`

## WHOIS Results:

**Registrar:** Porkbun LLC (IANA ID: 1861)

**Creation Date:** 2003-08-10

**Expiry Date:** 2026-08-10

**Domain Status:** clientDeleteProhibited, clientTransferProhibited

**Nameservers:** c.ns.buddyns.com, f.ns.buddyns.com, g.ns.buddyns.com, h.ns.buddyns.com, j.ns.buddyns.com

## DNS Records (nslookup -type=ANY hackthissite.org):

**A Records:** 137.74.187.100–104

**MX Records:** Google Mail Servers (aspmx.l.google.com, alt1.aspmx.l.google.com, etc.)

**TXT Records:** SPF policy, verification tokens

**CAA Records:** Certificates allowed from Let’s Encrypt, Sectigo, Harica

**SOA Record:** Primary NS → c.ns.buddyns.com, admin → admin@hackthissite.org
