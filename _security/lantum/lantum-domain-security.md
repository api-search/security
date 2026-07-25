---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lantum.com
  spf: true
hosts:
- cert_expires: Sep  8 20:41:17 2026 GMT
  host: www.lantum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lantum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lantum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lantum
provider_slug: lantum
slug: lantum-domain-security
source_filename: lantum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lantum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 20:41:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lantum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lantum/refs/heads/main/security/lantum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- United Kingdom
- Workforce Management
- NHS
- National Health System
- Staff Bank
- Rota Scheduling
- Primary Care
- Practice Management
- Healthcare Staffing
- Locum
---
