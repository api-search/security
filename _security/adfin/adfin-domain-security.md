---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: adfin.com
  spf: true
hosts:
- cert_expires: Oct 14 04:20:37 2026 GMT
  host: adfin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adfin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adfin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Adfin
provider_slug: adfin
slug: adfin-domain-security
source_filename: adfin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adfin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 04:20:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adfin.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adfin/refs/heads/main/security/adfin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Payments
- Invoicing
- Credit Control
- Direct Debit
- Billing
- Accounts Receivable
- United Kingdom
---
