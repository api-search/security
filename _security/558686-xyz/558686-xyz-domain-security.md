---
api_specs:
- filename: 558686-xyz-base-usdc-api-openapi.yml
  format: yaml
  label: gpt55-token-gateway Base Usdc API
  slug: 558686-xyz-base-usdc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-base-usdc-api-openapi.yml
- filename: 558686-xyz-chat-api-openapi.yml
  format: yaml
  label: gpt55-token-gateway Chat API
  slug: 558686-xyz-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-chat-api-openapi.yml
- filename: 558686-xyz-gpt55-model-gateway-api-openapi.yml
  format: yaml
  label: gpt55-token-gateway Gpt55 Model Gateway API
  slug: 558686-xyz-gpt55-model-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-gpt55-model-gateway-api-openapi.yml
- filename: 558686-xyz-gpt55-retained-high-intent-api-openapi.yml
  format: yaml
  label: gpt55-token-gateway Gpt55 Retained High Intent API
  slug: 558686-xyz-gpt55-retained-high-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-gpt55-retained-high-intent-api-openapi.yml
- filename: 558686-xyz-gpt55-retained-nonmodel-api-openapi.yml
  format: yaml
  label: gpt55-token-gateway Gpt55 Retained Nonmodel API
  slug: 558686-xyz-gpt55-retained-nonmodel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-gpt55-retained-nonmodel-api-openapi.yml
- filename: 558686-xyz-models-api-openapi.yml
  format: yaml
  label: gpt55-token-gateway Models API
  slug: 558686-xyz-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-models-api-openapi.yml
- filename: 558686-xyz-responses-api-openapi.yml
  format: yaml
  label: gpt55-token-gateway Responses API
  slug: 558686-xyz-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-responses-api-openapi.yml
- filename: 558686-xyz-utility-tools-api-openapi.yml
  format: yaml
  label: gpt55-token-gateway Utility Tools API
  slug: 558686-xyz-utility-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-utility-tools-api-openapi.yml
- filename: 558686-xyz-wallet-security-api-openapi.yml
  format: yaml
  label: gpt55-token-gateway Wallet Security API
  slug: 558686-xyz-wallet-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-wallet-security-api-openapi.yml
- filename: 558686-xyz-wallet-signing-safety-pack-api-openapi.yml
  format: yaml
  label: gpt55-token-gateway Wallet Signing Safety Pack API
  slug: 558686-xyz-wallet-signing-safety-pack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-wallet-signing-safety-pack-api-openapi.yml
- filename: 558686-xyz-x402-api-openapi.yml
  format: yaml
  label: gpt55-token-gateway X402 API
  slug: 558686-xyz-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/558686-xyz/refs/heads/main/openapi/558686-xyz-x402-api-openapi.yml
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
- Agentic Payments
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
