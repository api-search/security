---
api_specs:
- filename: openai-chat-completions-openapi.yml
  format: yaml
  label: OpenAI Chat Completions API
  slug: openai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-chat-completions-openapi.yml
- filename: openai-completions-openapi.yml
  format: yaml
  label: OpenAI Completions API
  slug: openai-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-completions-openapi.yml
- filename: openai-images-openapi.yml
  format: yaml
  label: OpenAI Images API
  slug: openai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-images-openapi.yml
- filename: openai-embeddings-openapi.yml
  format: yaml
  label: OpenAI Embeddings API
  slug: openai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-embeddings-openapi.yml
- filename: openai-audio-openapi.yml
  format: yaml
  label: OpenAI Audio API
  slug: openai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-audio-openapi.yml
- filename: openai-moderations-openapi.yml
  format: yaml
  label: OpenAI Moderations API
  slug: openai-moderations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-moderations-openapi.yml
- filename: openai-assistants-openapi.yml
  format: yaml
  label: OpenAI Assistants API
  slug: openai-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-assistants-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
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
name: Openai Apis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenAI APIs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenAI APIs
provider_slug: openai-apis
slug: openai-apis-domain-security
source_filename: openai-apis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: platform.openai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:51:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:04:17 2026 GMT\n  hsts: null\ndomains:\n- domain: openai.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/security/openai-apis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Embeddings
- Image Generation
- Language Models
- Speech
---
