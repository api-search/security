---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zapenergy.com
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: www.zapenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zap Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zap Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zap Energy
provider_slug: zap-energy
slug: zap-energy-domain-security
source_filename: zap-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zapenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: zapenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zap-energy/refs/heads/main/security/zap-energy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fusion
- Fusion Energy
- Nuclear Fusion
- Z-Pinch
- Sheared-Flow-Stabilized Z-Pinch
- Pulsed Power
- Plasma Physics
- FuZE
- FuZE-Q
- FuZE-3
- Century
- Fusion Pilot Plant
- Liquid Metal Walls
- Clean Energy
- Climate Tech
- DOE Milestone Program
- Energy
---
