---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: drover.ai
  spf: true
hosts:
- cert_expires: Oct 15 04:18:19 2026 GMT
  host: drover.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Drover Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drover AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Drover AI
provider_slug: drover-ai
slug: drover-ai-domain-security
source_filename: drover-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drover.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 04:18:19 2026 GMT\n  hsts: false\ndomains:\n- domain: drover.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drover-ai/refs/heads/main/security/drover-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Micromobility
- Computer Vision
- Artificial Intelligence
- IoT
- Fleet Management
- Regulatory Compliance
- Mobility Data Specification
---
