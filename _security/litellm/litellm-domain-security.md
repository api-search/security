---
api_specs:
- filename: litellm-assistants-api-openapi.yml
  format: yaml
  label: LiteLLM Assistants API
  slug: litellm-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/openapi/litellm-assistants-api-openapi.yml
- filename: litellm-audio-api-openapi.yml
  format: yaml
  label: LiteLLM Audio API
  slug: litellm-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/openapi/litellm-audio-api-openapi.yml
- filename: litellm-batches-api-openapi.yml
  format: yaml
  label: LiteLLM Batches API
  slug: litellm-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/openapi/litellm-batches-api-openapi.yml
- filename: litellm-chat-api-openapi.yml
  format: yaml
  label: LiteLLM Chat API
  slug: litellm-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/openapi/litellm-chat-api-openapi.yml
- filename: litellm-completions-api-openapi.yml
  format: yaml
  label: LiteLLM Completions API
  slug: litellm-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/openapi/litellm-completions-api-openapi.yml
- filename: litellm-embeddings-api-openapi.yml
  format: yaml
  label: LiteLLM Embeddings API
  slug: litellm-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/openapi/litellm-embeddings-api-openapi.yml
- filename: litellm-fine-tuning-api-openapi.yml
  format: yaml
  label: LiteLLM Fine Tuning API
  slug: litellm-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/openapi/litellm-fine-tuning-api-openapi.yml
- filename: litellm-images-api-openapi.yml
  format: yaml
  label: LiteLLM Images API
  slug: litellm-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/openapi/litellm-images-api-openapi.yml
- filename: litellm-messages-api-openapi.yml
  format: yaml
  label: LiteLLM Messages API
  slug: litellm-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/openapi/litellm-messages-api-openapi.yml
- filename: litellm-moderations-api-openapi.yml
  format: yaml
  label: LiteLLM Moderations API
  slug: litellm-moderations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/openapi/litellm-moderations-api-openapi.yml
- filename: litellm-ocr-api-openapi.yml
  format: yaml
  label: LiteLLM Ocr API
  slug: litellm-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/openapi/litellm-ocr-api-openapi.yml
- filename: litellm-rag-api-openapi.yml
  format: yaml
  label: LiteLLM Rag API
  slug: litellm-rag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/openapi/litellm-rag-api-openapi.yml
- filename: litellm-rerank-api-openapi.yml
  format: yaml
  label: LiteLLM Rerank API
  slug: litellm-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/openapi/litellm-rerank-api-openapi.yml
- filename: litellm-vector-stores-api-openapi.yml
  format: yaml
  label: LiteLLM Vector Stores API
  slug: litellm-vector-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/openapi/litellm-vector-stores-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: litellm.ai
  spf: true
hosts:
- cert_expires: Sep 12 18:35:09 2026 GMT
  host: www.litellm.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 19:15:58 2026 GMT
  host: docs.litellm.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Litellm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiteLLM, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LiteLLM
provider_slug: litellm
slug: litellm-domain-security
source_filename: litellm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.litellm.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 18:35:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.litellm.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 19:15:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: litellm.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/security/litellm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gateways
---
