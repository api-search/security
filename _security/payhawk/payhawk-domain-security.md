---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: payhawk.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: payhawk.io
  spf: true
hosts:
- cert_expires: Oct  9 01:49:22 2026 GMT
  host: payhawk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 21:34:49 2026 GMT
  host: developers.payhawk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 21:34:49 2026 GMT
  host: api.payhawk.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payhawk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Payhawk, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Payhawk
provider_slug: payhawk
slug: payhawk-domain-security
source_filename: payhawk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: payhawk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 01:49:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.payhawk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:34:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.payhawk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:34:49 2026 GMT\n  hsts: null\ndomains:\n- domain: payhawk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: payhawk.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payhawk/refs/heads/main/security/payhawk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Spend Management
- Corporate Cards
- Expense Management
- Invoice Management
- Budget Controls
- ERP Integration
- Accounts Payable
- FinTech
- Finance Automation
- Webhooks
---
