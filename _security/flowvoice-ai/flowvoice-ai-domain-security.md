---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: '100'
  dnssec: true
  domain: flowvoice.ai
  spf: true
hosts:
- cert_expires: Jan 10 06:36:17 2027 GMT
  host: flowvoice.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flowvoice Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wispr Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=100).'
provider_name: Wispr Ai
provider_slug: flowvoice-ai
slug: flowvoice-ai-domain-security
source_filename: flowvoice-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flowvoice.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 06:36:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flowvoice.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: '100'\n"
source_yaml_url: https://artifacts.apis.io/flowvoice-ai/security/flowvoice-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Voice-to-Text
- AI
- Productivity
- Transcription
---
