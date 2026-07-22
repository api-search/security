---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: earendil.io
  spf: true
hosts:
- cert_expires: Sep 28 12:20:47 2026 GMT
  host: earendil.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Earendil Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Earendil Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Earendil Robotics
provider_slug: earendil-robotics
slug: earendil-robotics-domain-security
source_filename: earendil-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: earendil.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:20:47 2026 GMT\n  hsts: false\ndomains:\n- domain: earendil.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earendil-robotics/refs/heads/main/security/earendil-robotics-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Robotics
- Defense
- Drones
- Counter-UAS
- Computer Vision
- Thermal Imaging
- Artificial Intelligence
- Hardware
---
