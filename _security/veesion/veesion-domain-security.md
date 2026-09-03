---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: veesion.io
  spf: true
hosts:
- cert_expires: Oct  1 05:24:48 2026 GMT
  host: veesion.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Veesion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veesion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Veesion
provider_slug: veesion
slug: veesion-domain-security
source_filename: veesion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: veesion.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:24:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: veesion.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veesion/refs/heads/main/security/veesion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Artificial Intelligence
- Computer Vision
- Video Surveillance
- Retail
- Loss Prevention
- Physical Security
- Gesture Recognition
- France
---
