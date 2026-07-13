---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: ChatGPT API
  slug: chatgpt-api
  spec_type: OpenAPI
  url: https://github.com/openai/openai-openapi/blob/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: OpenAI Responses API
  slug: openai-responses-api
  spec_type: OpenAPI
  url: https://github.com/openai/openai-openapi/blob/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: OpenAI Embeddings API
  slug: openai-embeddings-api
  spec_type: OpenAPI
  url: https://github.com/openai/openai-openapi/blob/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: OpenAI Images API
  slug: openai-images-api
  spec_type: OpenAPI
  url: https://github.com/openai/openai-openapi/blob/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: OpenAI Audio API
  slug: openai-audio-api
  spec_type: OpenAPI
  url: https://github.com/openai/openai-openapi/blob/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: OpenAI Moderations API
  slug: openai-moderations-api
  spec_type: OpenAPI
  url: https://github.com/openai/openai-openapi/blob/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: OpenAI Fine-Tuning API
  slug: openai-fine-tuning-api
  spec_type: OpenAPI
  url: https://github.com/openai/openai-openapi/blob/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: OpenAI Files API
  slug: openai-files-api
  spec_type: OpenAPI
  url: https://github.com/openai/openai-openapi/blob/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: OpenAI Batch API
  slug: openai-batch-api
  spec_type: OpenAPI
  url: https://github.com/openai/openai-openapi/blob/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: OpenAI Uploads API
  slug: openai-uploads-api
  spec_type: OpenAPI
  url: https://github.com/openai/openai-openapi/blob/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: OpenAI Vector Stores API
  slug: openai-vector-stores-api
  spec_type: OpenAPI
  url: https://github.com/openai/openai-openapi/blob/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: OpenAI Realtime API
  slug: openai-realtime-api
  spec_type: OpenAPI
  url: https://github.com/openai/openai-openapi/blob/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: OpenAI Models API
  slug: openai-models-api
  spec_type: OpenAPI
  url: https://github.com/openai/openai-openapi/blob/master/openapi.yaml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openai.com
  spf: true
hosts:
- cert_expires: Oct  6 21:51:17 2026 GMT
  host: platform.openai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 03:04:17 2026 GMT
  host: api.openai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chatgpt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChatGPT, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ChatGPT
provider_slug: chatgpt
slug: chatgpt-domain-security
source_filename: chatgpt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: platform.openai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:51:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:04:17 2026 GMT\n  hsts: null\ndomains:\n- domain: openai.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatgpt/refs/heads/main/security/chatgpt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- AI
- ChatGPT
- Embeddings
- Fine-Tuning
- GPT-4
- GPT-5
- Language Model
- OpenAI
- Realtime
---
