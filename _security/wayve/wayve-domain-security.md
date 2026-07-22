---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wayve.ai
  spf: true
hosts:
- cert_expires: Aug 27 12:34:12 2026 GMT
  host: wayve.ai
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wayve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wayve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wayve
provider_slug: wayve
slug: wayve-domain-security
source_filename: wayve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wayve.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 12:34:12 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: wayve.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wayve/refs/heads/main/security/wayve-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Autonomous Vehicles
- Embodied AI
- End-to-End Learning
- World Models
- Generative AI
- Self-Driving
- AV2.0
- GAIA
- LINGO
---
