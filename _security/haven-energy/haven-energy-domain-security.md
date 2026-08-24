---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: havenenergy.com
  spf: true
hosts:
- cert_expires: Nov 12 22:43:53 2026 GMT
  host: havenenergy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Haven Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Haven Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Haven Energy
provider_slug: haven-energy
slug: haven-energy-domain-security
source_filename: haven-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: havenenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 22:43:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: havenenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haven-energy/refs/heads/main/security/haven-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Energy Storage
- Solar
- Virtual Power Plant
- Distributed Energy Resources
- Home Battery
- Clean Energy
- Utilities
- Climate Tech
- Company
---
