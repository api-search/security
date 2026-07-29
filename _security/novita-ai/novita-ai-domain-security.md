---
api_specs:
- filename: novita-ai-openapi.json
  format: json
  label: Novita AI Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novita-ai/refs/heads/main/openapi/novita-ai-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: novita.ai
  spf: true
hosts:
- cert_expires: Aug 17 14:31:26 2026 GMT
  host: novita.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: api.novita.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Novita Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Novita AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Novita AI
provider_slug: novita-ai
slug: novita-ai-domain-security
source_filename: novita-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: novita.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 14:31:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.novita.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: novita.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novita-ai/refs/heads/main/security/novita-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Inference
- GPU
- OpenAI Compatible
- Image Generation
- Video Generation
- Audio
- Embeddings
- Sandbox
- MCP
---
