---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: antechdiagnostics.com
  spf: true
hosts:
- cert_expires: Oct  8 18:32:32 2026 GMT
  host: www.antechdiagnostics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 16:21:34 2026 GMT
  host: online.antechdiagnostics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Antech Diagnostics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Antech Diagnostics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Antech Diagnostics
provider_slug: antech-diagnostics
slug: antech-diagnostics-domain-security
source_filename: antech-diagnostics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.antechdiagnostics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:32:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: online.antechdiagnostics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:21:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: antechdiagnostics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antech-diagnostics/refs/heads/main/security/antech-diagnostics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Veterinary
- Diagnostics
- Laboratory
- Reference Lab
- Lab Results
- Animal Health
- PIMS Integration
- Mars Petcare
---
