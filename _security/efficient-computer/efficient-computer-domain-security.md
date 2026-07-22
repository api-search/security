---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: efficient.computer
  spf: true
hosts:
- cert_expires: Sep 30 16:21:02 2026 GMT
  host: www.efficient.computer
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Efficient Computer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Efficient Computer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Efficient Computer
provider_slug: efficient-computer
slug: efficient-computer-domain-security
source_filename: efficient-computer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.efficient.computer\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:21:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: efficient.computer\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/efficient-computer/refs/heads/main/security/efficient-computer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Semiconductors
- Processors
- Edge AI
- Embedded Systems
- Energy Efficiency
- Compilers
- Dataflow Architecture
- RISC-V
- IoT
---
