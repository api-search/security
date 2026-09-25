---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: synsense.ai
  spf: true
hosts:
- cert_expires: Nov 17 06:43:24 2026 GMT
  host: www.synsense.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aictx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aiCTX (now SynSense), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: aiCTX (now SynSense)
provider_slug: aictx
slug: aictx-domain-security
source_filename: aictx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.synsense.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 06:43:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: synsense.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aictx/refs/heads/main/security/aictx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Neuromorphic Computing
- Artificial Intelligence
- Semiconductors
- Edge Computing
- Machine Learning
- Sensors
- IoT
- Open Source
- Content
---
