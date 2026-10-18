---
api_specs:
- filename: aihubmix-aihubmix-unified-api-api-openapi.yml
  format: yaml
  label: AIHubMix AIHubMix Unified API
  slug: aihubmix-aihubmix-unified-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aihubmix/refs/heads/main/openapi/aihubmix-aihubmix-unified-api-api-openapi.yml
- filename: aihubmix-anthropic-compatible-api-openapi.yml
  format: yaml
  label: AIHubMix Anthropic Compatible API
  slug: aihubmix-anthropic-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aihubmix/refs/heads/main/openapi/aihubmix-anthropic-compatible-api-openapi.yml
- filename: aihubmix-google-vertex-ai-compatible-api-openapi.yml
  format: yaml
  label: AIHubMix Google Vertex AI Compatible API
  slug: aihubmix-google-vertex-ai-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aihubmix/refs/heads/main/openapi/aihubmix-google-vertex-ai-compatible-api-openapi.yml
- filename: aihubmix-openai-compatible-api-openapi.yml
  format: yaml
  label: AIHubMix OpenAI Compatible API
  slug: aihubmix-openai-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aihubmix/refs/heads/main/openapi/aihubmix-openai-compatible-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aihubmix.com
  spf: true
hosts:
- cert_expires: Dec  5 09:51:29 2026 GMT
  host: aihubmix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aihubmix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIHubMix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AIHubMix
provider_slug: aihubmix
slug: aihubmix-domain-security
source_filename: aihubmix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aihubmix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 09:51:29 2026 GMT\n  hsts: false\ndomains:\n- domain: aihubmix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aihubmix/refs/heads/main/security/aihubmix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- LLM
- Model Routing
- AI Gateway
- Generative AI
- MCP
---
