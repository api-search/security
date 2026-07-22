---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: axionorbital.space
  spf: true
hosts:
- cert_expires: Sep  8 09:22:07 2026 GMT
  host: axionorbital.space
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axionorbital Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axionorbital Space, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Axionorbital Space
provider_slug: axionorbital-space
slug: axionorbital-space-domain-security
source_filename: axionorbital-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axionorbital.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 09:22:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: axionorbital.space\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axionorbital-space/refs/heads/main/security/axionorbital-space-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Earth Observation
- Satellite Imagery
- Artificial Intelligence
- Computer Vision
- Space Technology
- SAR
- Remote Sensing
- Machine Learning
- Defense and Intelligence
- Geospatial
---
