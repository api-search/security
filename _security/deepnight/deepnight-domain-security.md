---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: deepnight.ai
  spf: true
hosts:
- cert_expires: Oct 10 23:46:32 2026 GMT
  host: deepnight.ai
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deepnight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deepnight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Deepnight
provider_slug: deepnight
slug: deepnight-domain-security
source_filename: deepnight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepnight.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:46:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: deepnight.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepnight/refs/heads/main/security/deepnight-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Frontier Tech
- Defense Technology
- Night Vision
- Computer Vision
- Artificial Intelligence
- Imaging
- Edge AI
---
