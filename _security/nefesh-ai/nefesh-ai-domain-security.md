---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nefesh.ai
  spf: false
hosts:
- cert_expires: Nov 29 21:40:21 2026 GMT
  host: nefesh.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 21:40:21 2026 GMT
  host: api.nefesh.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 21:40:21 2026 GMT
  host: gateway.nefesh.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Nefesh Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nefesh AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Nefesh AI
provider_slug: nefesh-ai
slug: nefesh-ai-domain-security
source_filename: nefesh-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nefesh.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 21:40:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nefesh.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 21:40:21 2026 GMT\n  hsts: null\n- host: gateway.nefesh.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 21:40:21 2026 GMT\n  hsts: null\ndomains:\n- domain: nefesh.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nefesh-ai/refs/heads/main/security/nefesh-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biometrics
- Human State
- Stress Detection
- Affective Computing
- AI Agents
- MCP
- A2A
- LLM Gateway
- Wearables
- Digital Health
- Middleware
---
