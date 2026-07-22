---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fantasmo.io
  spf: false
hosts:
- cert_expires: Sep 23 07:18:42 2026 GMT
  host: fantasmo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fantasmo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fantasmo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Fantasmo
provider_slug: fantasmo
slug: fantasmo-domain-security
source_filename: fantasmo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fantasmo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:18:42 2026 GMT\n  hsts: false\ndomains:\n- domain: fantasmo.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fantasmo/refs/heads/main/security/fantasmo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Camera Positioning
- Computer Vision
- Spatial Computing
- Geolocation
- Positioning
- Micromobility
- Robotics
- Augmented Reality
---
