---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 99bill.com
  spf: true
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: www.99bill.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: 99Bill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 99Bill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 99Bill
provider_slug: 99bill
slug: 99bill-domain-security
source_filename: 99bill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.99bill.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 99bill.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/99bill/refs/heads/main/security/99bill-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Fintech
- Payments
- Payment Processing
- Online Payment
- Mobile Payment
- China
- Merchant Services
---
