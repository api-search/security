---
description: ''
domains:
- caa:
  - 128 issue "certainly.com"
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: costco.com
  spf: true
hosts:
- cert_expires: Sep  6 23:59:59 2026 GMT
  host: www.costco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Costco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Costco Wholesale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Costco Wholesale
provider_slug: costco
slug: costco-domain-security
source_filename: costco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.costco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: costco.com\n  dnssec: false\n  caa:\n  - 128 issue \"certainly.com\"\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/costco/refs/heads/main/security/costco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Big-Box
- E-commerce
- EDI
- Fortune 500
- Grocery
- Membership
- Pharmacy
- Retail
- Supplier Portal
- Travel
- Warehouse Club
- Wholesale
---
