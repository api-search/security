---
api_specs:
- filename: delx-ai-protocol-openapi.json
  format: json
  label: Delx Protocol API
  slug: delx-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/openapi/delx-ai-protocol-openapi.json
- filename: delx-ai-commerce-x402-openapi.json
  format: json
  label: Delx Commerce x402 API
  slug: delx-commerce-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/openapi/delx-ai-commerce-x402-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: delx.ai
  spf: true
hosts:
- cert_expires: Nov 12 21:05:40 2026 GMT
  host: delx.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 22:37:38 2026 GMT
  host: ontology.delx.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 21:19:57 2026 GMT
  host: api.delx.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Delx Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delx, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Delx
provider_slug: delx-ai
slug: delx-ai-domain-security
source_filename: delx-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: delx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 21:05:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ontology.delx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 22:37:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.delx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 21:19:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: delx.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/security/delx-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- AI Agents
- MCP
- A2A
- x402
- Agentic Commerce
- Agent Continuity
- Agent Recovery
- Media Generation
- Web Intelligence
- Data Quality
- Utilities
- agent-native
---
