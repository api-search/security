---
api_specs:
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Chat Completions API
  slug: fireworks-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Completions API
  slug: fireworks-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Vision API
  slug: fireworks-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Embeddings API
  slug: fireworks-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Rerank API
  slug: fireworks-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Images API
  slug: fireworks-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Audio API
  slug: fireworks-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Batch Inference API
  slug: fireworks-batch-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Fine-Tuning API
  slug: fireworks-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Files API
  slug: fireworks-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Models API
  slug: fireworks-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Deployments API
  slug: fireworks-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
- filename: fireworks-ai-merged-openapi.yml
  format: yaml
  label: Fireworks Account API
  slug: fireworks-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/openapi/fireworks-ai-merged-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fireworks.ai
  spf: true
hosts:
- cert_expires: Sep 29 22:27:42 2026 GMT
  host: fireworks.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 15:49:44 2026 GMT
  host: docs.fireworks.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 01:51:07 2026 GMT
  host: api.fireworks.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fireworks Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fireworks AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fireworks AI
provider_slug: fireworks-ai
slug: fireworks-ai-domain-security
source_filename: fireworks-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fireworks.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:27:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.fireworks.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:49:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.fireworks.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:51:07 2026 GMT\n  hsts: null\ndomains:\n- domain: fireworks.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/security/fireworks-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Inference
- Multimodal
- Fine-tuning
- GPU
---
