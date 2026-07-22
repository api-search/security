---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: axera-tech.com
  spf: true
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: axera-tech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axera Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axera Tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Axera Tech
provider_slug: axera-tech
slug: axera-tech-domain-security
source_filename: axera-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axera-tech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: axera-tech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axera-tech/refs/heads/main/security/axera-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Semiconductor
- Artificial Intelligence
- Edge Computing
- NPU
- AI Inference
- Computer Vision
- Automotive
- Chips
- IoT
---
