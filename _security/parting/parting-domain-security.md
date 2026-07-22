---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: parting.com
  spf: true
hosts:
- cert_expires: Sep  6 08:45:56 2026 GMT
  host: parting.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parting, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Parting
provider_slug: parting
slug: parting-domain-security
source_filename: parting-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parting.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 08:45:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: parting.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parting/refs/heads/main/security/parting-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Funeral Services
- Death Care
- Cremation
- Directory
- Price Comparison
- Consumer
- Los Angeles
---
