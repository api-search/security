---
api_specs:
- filename: mistral-agents-api-openapi.yml
  format: yaml
  label: Mistral AI Agents API
  slug: mistral-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-agents-api-openapi.yml
- filename: mistral-audio-api-openapi.yml
  format: yaml
  label: Mistral AI Audio API
  slug: mistral-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-audio-api-openapi.yml
- filename: mistral-batch-jobs-api-openapi.yml
  format: yaml
  label: Mistral AI Batch Jobs API
  slug: mistral-batch-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-batch-jobs-api-openapi.yml
- filename: mistral-chat-api-openapi.yml
  format: yaml
  label: Mistral AI Chat API
  slug: mistral-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-chat-api-openapi.yml
- filename: mistral-embeddings-api-openapi.yml
  format: yaml
  label: Mistral AI Embeddings API
  slug: mistral-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-embeddings-api-openapi.yml
- filename: mistral-files-api-openapi.yml
  format: yaml
  label: Mistral AI Files API
  slug: mistral-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-files-api-openapi.yml
- filename: mistral-fim-api-openapi.yml
  format: yaml
  label: Mistral AI FIM API
  slug: mistral-fim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-fim-api-openapi.yml
- filename: mistral-fine-tuning-jobs-api-openapi.yml
  format: yaml
  label: Mistral AI Fine-Tuning Jobs API
  slug: mistral-fine-tuning-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-fine-tuning-jobs-api-openapi.yml
- filename: mistral-models-api-openapi.yml
  format: yaml
  label: Mistral AI Models API
  slug: mistral-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-models-api-openapi.yml
- filename: mistral-moderation-api-openapi.yml
  format: yaml
  label: Mistral AI Moderation API
  slug: mistral-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-moderation-api-openapi.yml
- filename: mistral-ocr-api-openapi.yml
  format: yaml
  label: Mistral AI OCR API
  slug: mistral-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral/refs/heads/main/openapi/mistral-ocr-api-openapi.yml
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
