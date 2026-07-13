---
api_specs:
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Chat Completions API
  slug: together-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Completions API
  slug: together-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Embeddings API
  slug: together-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Rerank API
  slug: together-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Images API
  slug: together-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Video API
  slug: together-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Audio API
  slug: together-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Vision API
  slug: together-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Fine-Tuning API
  slug: together-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Files API
  slug: together-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Models API
  slug: together-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Batch API
  slug: together-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Code Interpreter API
  slug: together-code-interpreter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Evaluations API
  slug: together-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
- filename: together-ai-openapi.yml
  format: yaml
  label: Together Dedicated Endpoints API
  slug: together-dedicated-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/openapi/together-ai-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: together.ai
  spf: true
hosts:
- cert_expires: Oct  1 01:45:42 2026 GMT
  host: www.together.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 21:12:39 2026 GMT
  host: docs.together.ai
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 21:12:39 2026 GMT
  host: api.together.ai
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Together Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Together AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Together AI
provider_slug: together-ai
slug: together-ai-domain-security
source_filename: together-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.together.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 01:45:42 2026 GMT\n  hsts: false\n- host: docs.together.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:12:39 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.together.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:12:39 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: together.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/together-ai/refs/heads/main/security/together-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Inference
- Foundation Models
- GPU
- Open Source AI
---
