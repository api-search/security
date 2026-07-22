---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: congruent.io
  spf: true
hosts:
- cert_expires: Oct  8 00:16:24 2026 GMT
  host: congruent.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Congruent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Congruent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Congruent
provider_slug: congruent
slug: congruent-domain-security
source_filename: congruent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: congruent.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 00:16:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: congruent.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/congruent/refs/heads/main/security/congruent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Radar
- Autonomous Vehicles
- Self-Driving Cars
- Sensors
- Simulation
- Robotics
- Hardware
- Y Combinator
- Automotive
---
