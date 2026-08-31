---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lyte.ai
  spf: true
hosts:
- cert_expires: Sep 28 23:02:42 2026 GMT
  host: lyte.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lyte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lyte, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lyte
provider_slug: lyte
slug: lyte-domain-security
source_filename: lyte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lyte.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:02:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lyte.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lyte/refs/heads/main/security/lyte-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Computer-Vision
- Perception
- Sensors
- Physical AI
- Semiconductors
- Artificial Intelligence
- Advanced Mobility
- Hardware
---
