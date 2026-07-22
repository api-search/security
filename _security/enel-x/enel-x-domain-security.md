---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: enelx.com
  spf: true
hosts:
- cert_expires: Aug 12 02:23:43 2026 GMT
  host: www.enelx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enel X Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enel X, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Enel X
provider_slug: enel-x
slug: enel-x-domain-security
source_filename: enel-x-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enelx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 02:23:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: enelx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enel-x/refs/heads/main/security/enel-x-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Smart Energy
- Distributed Energy Resources
- DER Management
- Virtual Power Plant
- Demand Response
- Flexibility
- Grid Services
- Electric Vehicle Charging
- EV Charging
- Electrification
- E-Mobility
- JuiceBox
- JuiceNet
- Enel X Way
- VPP Connect
- oADR
- OpenADR
- Battery Storage
- Heat Pumps
- HVAC
- Sustainable Mobility
- Utility
- Enel Group
---
