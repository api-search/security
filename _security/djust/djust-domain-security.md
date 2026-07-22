---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: djust.io
  spf: true
hosts:
- cert_expires: Sep  9 14:06:49 2026 GMT
  host: djust.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Djust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Djust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Djust
provider_slug: djust
slug: djust-domain-security
source_filename: djust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: djust.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 14:06:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: djust.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/djust/refs/heads/main/security/djust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- B2B
- eCommerce
- eProcurement
- Commerce
- Payments
- Order Management
- ERP Integration
- Retail
- France
---
