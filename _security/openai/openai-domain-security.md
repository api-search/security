---
api_specs:
- filename: assistants-openapi-original.yml
  format: yaml
  label: OpenAI Assistants API
  slug: openai-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/assistants-openapi-original.yml
- filename: audio-openapi-original.yml
  format: yaml
  label: OpenAI Audio API
  slug: openai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/audio-openapi-original.yml
- filename: chat-openapi-original.yml
  format: yaml
  label: OpenAI Chat API
  slug: openai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/chat-openapi-original.yml
- filename: openai-chat-completions-api-openapi.yml
  format: yaml
  label: OpenAI Chat Completions API
  slug: openai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/properties/openai-chat-completions-api-openapi.yml
- filename: embeddings-openapi-original.yml
  format: yaml
  label: OpenAI Embeddings API
  slug: openai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/embeddings-openapi-original.yml
- filename: files-openapi-original.yml
  format: yaml
  label: OpenAI Files API
  slug: openai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/files-openapi-original.yml
- filename: fine-tuning-openapi-original.yml
  format: yaml
  label: OpenAI Fine Tuning API
  slug: openai-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/fine-tuning-openapi-original.yml
- filename: images-openapi-original.yml
  format: yaml
  label: OpenAI Images API
  slug: openai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/images-openapi-original.yml
- filename: models-openapi-original.yml
  format: yaml
  label: OpenAI Models API
  slug: openai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/models-openapi-original.yml
- filename: threads-openapi-original.yml
  format: yaml
  label: OpenAI Threads API
  slug: openai-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/threads-openapi-original.yml
- filename: openai-realtime-asyncapi.yml
  format: yaml
  label: OpenAI Realtime API
  slug: openai-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/asyncapi/openai-realtime-asyncapi.yml
- filename: completions-openapi-original.yml
  format: yaml
  label: OpenAI Completions API
  slug: openai-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/openapi/completions-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
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
- cert_expires: Sep 13 18:06:08 2026 GMT
  host: developers.openai.com
  hsts: true
  hsts_max_age: 63072000
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
name: Openai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenAI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenAI
provider_slug: openai
slug: openai-domain-security
source_filename: openai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: platform.openai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:51:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.openai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:06:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.openai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:04:17 2026 GMT\n  hsts: null\ndomains:\n- domain: openai.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/security/openai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
---
