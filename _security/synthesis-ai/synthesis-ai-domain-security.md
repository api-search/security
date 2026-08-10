---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: synthesis.ai
  mx:
  - ASPMX.L.GOOGLE.COM.
  - ALT1.ASPMX.L.GOOGLE.COM.
  - ALT2.ASPMX.L.GOOGLE.COM.
  - ALT3.ASPMX.L.GOOGLE.COM.
  - ALT4.ASPMX.L.GOOGLE.COM.
  registrar_dns: gandi.net
  spf: false
hosts:
- host: synthesis.ai
  hsts: false
  http: true
  http_body: Gandi "parked by the owner" holding page (2332 bytes)
  http_status: 200
  https: false
  https_error: connection refused on tcp/443
- cname: webredir.vip.gandi.net.
  host: www.synthesis.ai
  https: false
  https_error: connection refused on tcp/443
- host: docs.synthesis.ai
  note: no A/CNAME record; the former Human API documentation host is gone
  resolves: false
- host: api.synthesis.ai
  resolves: false
kind: domain-security
layout: security
method: probed
name: Synthesis Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synthesis AI, probed live across 4 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Synthesis AI
provider_slug: synthesis-ai
slug: synthesis-ai-domain-security
source_filename: synthesis-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: dig + TCP/TLS probe of synthesis.ai from the enrichment run\nnote: >-\n  synthesis.ai no longer serves HTTPS at all — TCP 443 is refused — and the\n  domain resolves to Gandi parking IPs. Mail (Google Workspace MX) is still\n  configured on a domain that publishes neither SPF nor DMARC, so the domain is\n  trivially spoofable. Absence of a record here is observed data, not a gap in\n  the probe.\nhosts:\n- host: synthesis.ai\n  https: false\n  https_error: connection refused on tcp/443\n  http: true\n  http_status: 200\n  http_body: Gandi \"parked by the owner\" holding page (2332 bytes)\n  hsts: false\n- host: www.synthesis.ai\n  cname: webredir.vip.gandi.net.\n  https: false\n  https_error: connection refused on tcp/443\n- host: docs.synthesis.ai\n  resolves: false\n  note: no A/CNAME record; the former Human API documentation host is gone\n- host: api.synthesis.ai\n  resolves: false\ndomains:\n- domain: synthesis.ai\n  registrar_dns:\
  \ gandi.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  mx:\n  - ASPMX.L.GOOGLE.COM.\n  - ALT1.ASPMX.L.GOOGLE.COM.\n  - ALT2.ASPMX.L.GOOGLE.COM.\n  - ALT3.ASPMX.L.GOOGLE.COM.\n  - ALT4.ASPMX.L.GOOGLE.COM.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthesis-ai/refs/heads/main/security/synthesis-ai-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Synthetic Data
- Computer Vision
- Machine Learning
- Artificial Intelligence
- Digital Humans
- Training Data
- 3D
---
