---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: birdstop.io
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: birdstop.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Birdstop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Birdstop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Birdstop
provider_slug: birdstop
slug: birdstop-domain-security
source_filename: birdstop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: birdstop.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: birdstop.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/birdstop/refs/heads/main/security/birdstop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Drones
- UAV
- Remote Sensing
- Autonomous Systems
- Aerial Surveillance
- Critical Infrastructure
- Public Safety
- Robotics
- Computer Vision
---
