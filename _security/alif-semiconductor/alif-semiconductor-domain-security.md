---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alifsemi.com
  spf: true
hosts:
- cert_expires: Sep  5 05:14:43 2026 GMT
  host: alifsemi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alif Semiconductor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alif Semiconductor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alif Semiconductor
provider_slug: alif-semiconductor
slug: alif-semiconductor-domain-security
source_filename: alif-semiconductor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alifsemi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:14:43 2026 GMT\n  hsts: false\ndomains:\n- domain: alifsemi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alif-semiconductor/refs/heads/main/security/alif-semiconductor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Semiconductors
- Microcontrollers
- Edge AI
- Machine Learning
- Embedded Systems
- IoT
- Hardware
- Arm Cortex-M55
- Neural Processing Unit
---
