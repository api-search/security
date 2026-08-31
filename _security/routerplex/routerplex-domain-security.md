---
api_specs:
- filename: routerplex-chat-api-openapi.yml
  format: yaml
  label: RouterPlex Chat API
  slug: routerplex-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/openapi/routerplex-chat-api-openapi.yml
- filename: routerplex-images-api-openapi.yml
  format: yaml
  label: RouterPlex Images API
  slug: routerplex-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/openapi/routerplex-images-api-openapi.yml
- filename: routerplex-messages-api-openapi.yml
  format: yaml
  label: RouterPlex Messages API
  slug: routerplex-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/openapi/routerplex-messages-api-openapi.yml
- filename: routerplex-models-api-openapi.yml
  format: yaml
  label: RouterPlex Models API
  slug: routerplex-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/openapi/routerplex-models-api-openapi.yml
- filename: routerplex-responses-api-openapi.yml
  format: yaml
  label: RouterPlex Responses API
  slug: routerplex-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/openapi/routerplex-responses-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: routerplex.com
  spf: true
hosts:
- cert_expires: Oct  2 23:32:58 2026 GMT
  host: docs.routerplex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:32:58 2026 GMT
  host: api.routerplex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Routerplex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RouterPlex, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RouterPlex
provider_slug: routerplex
slug: routerplex-domain-security
source_filename: routerplex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.routerplex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:32:58 2026 GMT\n  hsts: false\n- host: api.routerplex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:32:58 2026 GMT\n  hsts: null\ndomains:\n- domain: routerplex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routerplex/refs/heads/main/security/routerplex-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- llm
- Artificial Intelligence
- ai-gateway
- Inference
- model-router
- openai-compatible
- anthropic-compatible
- claude
- gpt
- gemini
- api-gateway
- agent-infrastructure
- Developer Tools
- MCP
- llmops
---
