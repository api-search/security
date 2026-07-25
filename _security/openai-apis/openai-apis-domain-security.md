---
api_specs:
- filename: openai-apis-assistants-api-openapi.yml
  format: yaml
  label: OpenAI APIs Assistants API
  slug: openai-apis-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-assistants-api-openapi.yml
- filename: openai-apis-chat-api-openapi.yml
  format: yaml
  label: OpenAI APIs Chat API
  slug: openai-apis-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-chat-api-openapi.yml
- filename: openai-apis-completions-api-openapi.yml
  format: yaml
  label: OpenAI APIs Completions API
  slug: openai-apis-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-completions-api-openapi.yml
- filename: openai-apis-embeddings-api-openapi.yml
  format: yaml
  label: OpenAI APIs Embeddings API
  slug: openai-apis-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-embeddings-api-openapi.yml
- filename: openai-apis-images-api-openapi.yml
  format: yaml
  label: OpenAI APIs Images API
  slug: openai-apis-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-images-api-openapi.yml
- filename: openai-apis-messages-api-openapi.yml
  format: yaml
  label: OpenAI APIs Messages API
  slug: openai-apis-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-messages-api-openapi.yml
- filename: openai-apis-moderations-api-openapi.yml
  format: yaml
  label: OpenAI APIs Moderations API
  slug: openai-apis-moderations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-moderations-api-openapi.yml
- filename: openai-apis-runs-api-openapi.yml
  format: yaml
  label: OpenAI APIs Runs API
  slug: openai-apis-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-runs-api-openapi.yml
- filename: openai-apis-speech-api-openapi.yml
  format: yaml
  label: OpenAI APIs Speech API
  slug: openai-apis-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-speech-api-openapi.yml
- filename: openai-apis-threads-api-openapi.yml
  format: yaml
  label: OpenAI APIs Threads API
  slug: openai-apis-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-threads-api-openapi.yml
- filename: openai-apis-transcription-api-openapi.yml
  format: yaml
  label: OpenAI APIs Transcription API
  slug: openai-apis-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-transcription-api-openapi.yml
- filename: openai-apis-translation-api-openapi.yml
  format: yaml
  label: OpenAI APIs Translation API
  slug: openai-apis-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openai-apis/refs/heads/main/openapi/openai-apis-translation-api-openapi.yml
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
