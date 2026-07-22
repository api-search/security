---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: auterion.com
  spf: true
hosts:
- cert_expires: Sep  8 19:02:07 2026 GMT
  host: auterion.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Auterion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auterion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Auterion
provider_slug: auterion
slug: auterion-domain-security
source_filename: auterion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auterion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 19:02:07 2026 GMT\n  hsts: false\ndomains:\n- domain: auterion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auterion/refs/heads/main/security/auterion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Ml
- Drones
- UAV
- Robotics
- Autonomous Systems
- Aerospace
- Defense
- Fleet Management
- SDK
---
