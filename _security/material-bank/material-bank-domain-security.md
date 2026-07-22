---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: materialbank.com
  spf: true
hosts:
- cert_expires: Dec 13 12:00:14 2026 GMT
  host: www.materialbank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Material Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Material Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Material Bank
provider_slug: material-bank
slug: material-bank-domain-security
source_filename: material-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.materialbank.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 12:00:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: materialbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/material-bank/refs/heads/main/security/material-bank-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Commerce
- Materials
- Marketplace
- Architecture
- Interior Design
- Samples
- Building Products
- Sustainability
---
