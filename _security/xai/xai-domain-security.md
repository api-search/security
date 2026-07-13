---
api_specs:
- filename: xai-openapi.json
  format: json
  label: xAI Chat Completions API
  slug: xai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Responses API
  slug: xai-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Images API
  slug: xai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Video Generation API
  slug: xai-video-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Voice API
  slug: xai-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Embeddings API
  slug: xai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Models API
  slug: xai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
- filename: xai-openapi.json
  format: json
  label: xAI Batch API
  slug: xai-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/openapi/xai-openapi.json
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: x.ai
  spf: true
hosts:
- cert_expires: Sep 16 08:14:55 2026 GMT
  host: x.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 08:14:55 2026 GMT
  host: docs.x.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 08:14:55 2026 GMT
  host: api.x.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for xAI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: xAI
provider_slug: xai
slug: xai-domain-security
source_filename: xai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: x.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:14:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.x.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:14:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.x.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:14:55 2026 GMT\n  hsts: null\ndomains:\n- domain: x.ai\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xai/refs/heads/main/security/xai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Foundation Models
- Grok
- Generative AI
---
