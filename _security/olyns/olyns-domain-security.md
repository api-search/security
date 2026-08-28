---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: olyns.com
  spf: true
hosts:
- cert_expires: Nov 23 03:35:04 2026 GMT
  host: olyns.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Olyns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Olyns, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Olyns
provider_slug: olyns
slug: olyns-domain-security
source_filename: olyns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: olyns.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 03:35:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: olyns.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olyns/refs/heads/main/security/olyns-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Recycling
- Sustainability
- Circular Economy
- Retail Media
- Digital Out-of-Home
- Advertising
- Artificial Intelligence
- Reverse Vending
- Consumer
---
