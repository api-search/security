---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: true
  domain: fimi.com
  spf: true
hosts:
- cert_expires: Sep 14 15:27:13 2026 GMT
  host: fimi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fimi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FIMI Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present.'
provider_name: FIMI Technology
provider_slug: fimi
slug: fimi-domain-security
source_filename: fimi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fimi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 14 15:27:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fimi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fimi/refs/heads/main/security/fimi-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer Electronics
- Drones
- Cameras
- Gimbals
- Aerial Imaging
- Hardware
- Xiaomi Ecosystem
- Robotics
- China
---
