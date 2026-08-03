---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mojo.vision
  spf: true
hosts:
- cert_expires: Oct 29 01:44:15 2026 GMT
  host: www.mojo.vision
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mojo Vision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mojo Vision, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mojo Vision
provider_slug: mojo-vision
slug: mojo-vision-domain-security
source_filename: mojo-vision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mojo.vision\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 01:44:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mojo.vision\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mojo-vision/refs/heads/main/security/mojo-vision-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Semiconductors
- Displays
- Micro-LED
- Hardware
- Augmented Reality
- Extended Reality
- Optical Interconnect
- AI Infrastructure
- Quantum Dots
---
