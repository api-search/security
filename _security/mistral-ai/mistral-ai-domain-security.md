---
api_specs:
- filename: mistral-ai-agents-api-openapi.yml
  format: yaml
  label: Mistral AI Agents API
  slug: mistral-ai-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-agents-api-openapi.yml
- filename: mistral-ai-batch-jobs-api-openapi.yml
  format: yaml
  label: Mistral AI Batch Jobs API
  slug: mistral-ai-batch-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-batch-jobs-api-openapi.yml
- filename: mistral-ai-chat-completions-api-openapi.yml
  format: yaml
  label: Mistral AI Chat Completions API
  slug: mistral-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-chat-completions-api-openapi.yml
- filename: mistral-ai-embeddings-api-openapi.yml
  format: yaml
  label: Mistral AI Embeddings API
  slug: mistral-ai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-embeddings-api-openapi.yml
- filename: mistral-ai-fine-tuning-jobs-api-openapi.yml
  format: yaml
  label: Mistral AI Fine-Tuning Jobs API
  slug: mistral-ai-fine-tuning-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-fine-tuning-jobs-api-openapi.yml
- filename: mistral-ai-models-api-openapi.yml
  format: yaml
  label: Mistral AI Models API
  slug: mistral-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-models-api-openapi.yml
- filename: mistral-ai-ocr-api-openapi.yml
  format: yaml
  label: Mistral AI OCR API
  slug: mistral-ai-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-ocr-api-openapi.yml
- filename: mistral-ai-training-jobs-api-openapi.yml
  format: yaml
  label: Mistral AI Training Jobs API
  slug: mistral-ai-training-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/openapi/mistral-ai-training-jobs-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mistral.ai
  spf: true
hosts:
- cert_expires: Sep 21 23:33:27 2026 GMT
  host: console.mistral.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
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
kind: domain-security
layout: security
method: probed
name: Mistral Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mistral AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mistral AI
provider_slug: mistral-ai
slug: mistral-ai-domain-security
source_filename: mistral-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: console.mistral.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:33:27 2026 GMT\n  hsts: null\n- host: mistral.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 21:38:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.mistral.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:46:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mistral.ai\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mistral-ai/refs/heads/main/security/mistral-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- Artificial Intelligence
- Batch Processing
- Chat
- Embeddings
- Fine-Tuning
- Large Language Models
- OCR
---
