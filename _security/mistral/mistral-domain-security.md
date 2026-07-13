---
api_specs:
- filename: openapi.json
  format: json
  label: Mistral AI Chat API
  slug: mistral-ai-chat-api
  spec_type: OpenAPI
  url: https://docs.mistral.ai/openapi.json
- filename: mistral-embeddings-openapi.yml
  format: yaml
  label: Mistral Embeddings API
  slug: mistral-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-embeddings-openapi.yml
- filename: mistral-moderation-openapi.yml
  format: yaml
  label: Mistral Moderation API
  slug: mistral-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-moderation-openapi.yml
- filename: mistral-agents-openapi.yml
  format: yaml
  label: Mistral AI Agents API
  slug: mistral-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-agents-openapi.yml
- filename: mistral-fim-openapi.yml
  format: yaml
  label: Mistral AI FIM API
  slug: mistral-ai-fim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-fim-openapi.yml
- filename: mistral-ocr-openapi.yml
  format: yaml
  label: Mistral AI OCR API
  slug: mistral-ai-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-ocr-openapi.yml
- filename: mistral-fine-tuning-openapi.yml
  format: yaml
  label: Mistral AI Fine-Tuning API
  slug: mistral-ai-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-fine-tuning-openapi.yml
- filename: mistral-files-openapi.yml
  format: yaml
  label: Mistral AI Files API
  slug: mistral-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-files-openapi.yml
- filename: mistral-models-openapi.yml
  format: yaml
  label: Mistral AI Models API
  slug: mistral-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-models-openapi.yml
- filename: mistral-batch-openapi.yml
  format: yaml
  label: Mistral AI Batch API
  slug: mistral-ai-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-batch-openapi.yml
- filename: mistral-audio-transcription-openapi.yml
  format: yaml
  label: Mistral AI Audio Transcription API
  slug: mistral-ai-audio-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-audio-transcription-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mistral.ai
  spf: true
hosts:
- cert_expires: Sep 11 21:38:58 2026 GMT
  host: mistral.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 16:46:55 2026 GMT
  host: docs.mistral.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 21:30:01 2026 GMT
  host: api.mistral.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mistral Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mistral AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mistral AI
provider_slug: mistral
slug: mistral-domain-security
source_filename: mistral-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mistral.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 21:38:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.mistral.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:46:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mistral.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 21:30:01 2026 GMT\n  hsts: null\ndomains:\n- domain: mistral.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/security/mistral-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
