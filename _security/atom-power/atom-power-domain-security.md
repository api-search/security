---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atompower.com
  spf: true
hosts:
- cert_expires: Oct 31 09:21:07 2026 GMT
  host: www.atompower.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atom Power Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atom Power, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atom Power
provider_slug: atom-power
slug: atom-power-domain-security
source_filename: atom-power-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atompower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 09:21:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: atompower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atom-power/refs/heads/main/security/atom-power-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Electric Vehicle Charging
- EV Charging
- Circuit Protection
- Solid State Circuit Breaker
- Electrical Equipment
- Energy Management
- Hardware
---
