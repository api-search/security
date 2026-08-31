---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inmarsat.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.inmarsat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: developer.inmarsat.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inmarsat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inmarsat, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Inmarsat
provider_slug: inmarsat
slug: inmarsat-domain-security
source_filename: inmarsat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inmarsat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.inmarsat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: inmarsat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inmarsat/refs/heads/main/security/inmarsat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Satellite Communications
- SATCOM
- Maritime
- Aviation
- Government
- Enterprise
- IoT
- Machine to Machine
- M2M
- Broadband
- L-Band
- Ka-Band
- Global Xpress
- BGAN
- IsatData Pro
- Fleet Xpress
- NexusWave
- GMDSS
- Safety Services
- NB-NTN
- Non-Terrestrial Network
- Viasat
---
