---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: terawatt-technology.com
  spf: true
hosts:
- cert_expires: Nov  9 06:49:00 2026 GMT
  host: www.terawatt-technology.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terawatt Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TeraWatt Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TeraWatt Technology
provider_slug: terawatt-technology
slug: terawatt-technology-domain-security
source_filename: terawatt-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.terawatt-technology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 06:49:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: terawatt-technology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terawatt-technology/refs/heads/main/security/terawatt-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Batteries
- Energy Storage
- Lithium-Ion
- Electric Vehicles
- Manufacturing
- Clean Energy
- Hardware
---
