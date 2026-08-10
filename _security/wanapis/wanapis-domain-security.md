---
api_specs:
- filename: wanapis-audio-api-openapi.yml
  format: yaml
  label: WanAPIs Audio API
  slug: wanapis-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wanapis/refs/heads/main/openapi/wanapis-audio-api-openapi.yml
- filename: wanapis-chat-api-openapi.yml
  format: yaml
  label: WanAPIs Chat API
  slug: wanapis-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wanapis/refs/heads/main/openapi/wanapis-chat-api-openapi.yml
- filename: wanapis-completions-api-openapi.yml
  format: yaml
  label: WanAPIs Completions API
  slug: wanapis-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wanapis/refs/heads/main/openapi/wanapis-completions-api-openapi.yml
- filename: wanapis-embeddings-api-openapi.yml
  format: yaml
  label: WanAPIs Embeddings API
  slug: wanapis-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wanapis/refs/heads/main/openapi/wanapis-embeddings-api-openapi.yml
- filename: wanapis-images-api-openapi.yml
  format: yaml
  label: WanAPIs Images API
  slug: wanapis-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wanapis/refs/heads/main/openapi/wanapis-images-api-openapi.yml
- filename: wanapis-models-api-openapi.yml
  format: yaml
  label: WanAPIs Models API
  slug: wanapis-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wanapis/refs/heads/main/openapi/wanapis-models-api-openapi.yml
- filename: wanapis-responses-api-openapi.yml
  format: yaml
  label: WanAPIs Responses API
  slug: wanapis-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wanapis/refs/heads/main/openapi/wanapis-responses-api-openapi.yml
- filename: wanapis-tasks-api-openapi.yml
  format: yaml
  label: WanAPIs Tasks API
  slug: wanapis-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wanapis/refs/heads/main/openapi/wanapis-tasks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wanapis.com
  spf: true
hosts:
- cert_expires: Sep 30 06:59:43 2026 GMT
  host: wanapis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 06:59:43 2026 GMT
  host: api.wanapis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wanapis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WanAPIs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WanAPIs
provider_slug: wanapis
slug: wanapis-domain-security
source_filename: wanapis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wanapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:59:43 2026 GMT\n  hsts: false\n- host: api.wanapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:59:43 2026 GMT\n  hsts: false\ndomains:\n- domain: wanapis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wanapis/refs/heads/main/security/wanapis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- LLM Gateway
- AI API Gateway
- OpenAI Compatible
- Model Marketplace
- LLM
- GPT
- Claude
- Gemini
- DeepSeek
- Image Generation
- Video Generation
- Audio
- Multimodal
- Routing
- Failover
---
