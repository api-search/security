---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eino.ai
  spf: true
hosts:
- cert_expires: Sep 25 19:28:45 2026 GMT
  host: eino.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eino Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EINO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EINO
provider_slug: eino
slug: eino-domain-security
source_filename: eino-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eino.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:28:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eino.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eino/refs/heads/main/security/eino-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Wireless
- Networking
- Digital Twin
- Network Design
- Network Monitoring
- Connectivity
- Artificial Intelligence
- 5G
- IoT
- Telecommunications
---
