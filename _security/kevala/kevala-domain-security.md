---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kevala.com
  spf: true
hosts:
- cert_expires: Sep 30 21:28:17 2026 GMT
  host: www.kevala.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 04:19:24 2026 GMT
  host: api.kevala.com
  hsts: true
  hsts_max_age: 31536000
  hsts_note: 'Corrected by hand 2026-08-23. The automated probe recorded null because the API host answers 404 (nginx) at "/" with no body to score; a direct HEAD on https://api.kevala.com/ returns `strict-transport-security: max-age=31536000; includeSubDomains; preload`.'
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kevala Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kevala, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kevala
provider_slug: kevala
slug: kevala-domain-security
source_filename: kevala-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kevala.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:28:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kevala.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 04:19:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_note: >-\n    Corrected by hand 2026-08-23. The automated probe recorded null because the API host answers\n    404 (nginx) at \"/\" with no body to score; a direct HEAD on https://api.kevala.com/ returns\n    `strict-transport-security: max-age=31536000; includeSubDomains; preload`.\ndomains:\n- domain: kevala.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kevala/refs/heads/main/security/kevala-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Electricity
- Electric Grid
- Grid Analytics
- Distributed Energy Resources
- Utilities
- Geospatial
- Analytics
- Carbon Accounting
- Electric Vehicles
- Sustainability
---
