---
api_specs:
- filename: 558686-xyz-gpt55-model-gateway-openapi.json
  format: json
  label: GPT55 Model Gateway API
  slug: gpt55-model-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-gpt55-model-gateway-openapi.json
- filename: 558686-xyz-api-market-utility-tools-openapi.json
  format: json
  label: GPT-5.5 Utility Tools for API.market
  slug: gpt55-utility-tools-api-market
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-api-market-utility-tools-openapi.json
- filename: 558686-xyz-sub2api-openapi.json
  format: json
  label: Sub2API OpenAI-compatible API
  slug: sub2api-openai-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-sub2api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 558686.xyz
  spf: true
hosts:
- cert_expires: Nov  1 07:22:08 2026 GMT
  host: 558686.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 07:22:08 2026 GMT
  host: gpt55.558686.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 07:22:08 2026 GMT
  host: sub2api.558686.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 558686 Xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for gpt55-token-gateway, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: gpt55-token-gateway
provider_slug: 558686-xyz
slug: 558686-xyz-domain-security
source_filename: 558686-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 558686.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 07:22:08 2026 GMT\n  hsts: false\n- host: gpt55.558686.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 07:22:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sub2api.558686.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 07:22:08 2026 GMT\n  hsts: false\ndomains:\n- domain: 558686.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/security/558686-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- x402
- Agent Payments
- MCP
- A2A
- AI Gateway
- OpenAI-Compatible
- LLM
- AI Agents
- USDC
- Base
- API Relay
- Developer Tools
---
