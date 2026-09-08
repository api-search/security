---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: senseglove.com
  spf: true
hosts:
- cert_expires: Oct  9 22:48:26 2026 GMT
  host: www.senseglove.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adjuvomotion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adjuvo Motion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adjuvo Motion
provider_slug: adjuvomotion
slug: adjuvomotion-domain-security
source_filename: adjuvomotion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.senseglove.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 22:48:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: senseglove.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adjuvomotion/refs/heads/main/security/adjuvomotion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Haptics
- Virtual Reality
- Extended Reality
- Robotics
- Hardware
- SDK
- Simulation
- Training
- Teleoperation
- Wearables
---
