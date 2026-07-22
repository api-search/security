---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: waabi.ai
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: waabi.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Waabi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Waabi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Waabi
provider_slug: waabi
slug: waabi-domain-security
source_filename: waabi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: waabi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: waabi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waabi/refs/heads/main/security/waabi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Autonomous Vehicles
- Self Driving
- Trucking
- Robotics
- Simulation
- Physical Ai
---
