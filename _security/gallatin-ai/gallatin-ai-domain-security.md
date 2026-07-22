---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gallatin.ai
  spf: true
hosts:
- cert_expires: Sep  9 07:36:23 2026 GMT
  host: gallatin.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gallatin Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gallatin AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gallatin AI
provider_slug: gallatin-ai
slug: gallatin-ai-domain-security
source_filename: gallatin-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gallatin.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 07:36:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gallatin.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gallatin-ai/refs/heads/main/security/gallatin-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Defense
- Logistics
- Artificial Intelligence
- Supply Chain
- Decision Support
- Military
- GovTech
---
