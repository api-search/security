---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: podenergy.com
  spf: true
hosts:
- cert_expires: Sep  5 04:56:24 2026 GMT
  host: podenergy.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: ocpi.podenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pod Point Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pod Point, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pod Point
provider_slug: pod-point
slug: pod-point-domain-security
source_filename: pod-point-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: podenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 04:56:24 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: ocpi.podenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: podenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pod-point/refs/heads/main/security/pod-point-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- EV Charging
- Electric Vehicles
- Utilities
- Electricity
- OCPI
- Charge Point Operator
- Smart Charging
- Grid
---
