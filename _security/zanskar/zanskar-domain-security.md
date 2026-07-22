---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zanskar.com
  spf: false
hosts:
- cert_expires: Oct  8 21:15:23 2026 GMT
  host: zanskar.com
  hsts: true
  hsts_max_age: 2628000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zanskar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zanskar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Zanskar
provider_slug: zanskar
slug: zanskar-domain-security
source_filename: zanskar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zanskar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 21:15:23 2026 GMT\n  hsts: true\n  hsts_max_age: 2628000\ndomains:\n- domain: zanskar.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zanskar/refs/heads/main/security/zanskar-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Planetary Health
- Geothermal
- Energy
- Clean Energy
- Climate
- Artificial Intelligence
- Data
---
