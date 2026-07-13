---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: waymo.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:04 2026 GMT
  host: waymo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Waymo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Waymo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Waymo
provider_slug: waymo
slug: waymo-domain-security
source_filename: waymo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: waymo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: waymo.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waymo/refs/heads/main/security/waymo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Autonomous Vehicles
- Self-Driving
- Robotaxi
- Ride-Hailing
- Alphabet
- Lidar
- Computer Vision
- Open Dataset
- Simulation
---
