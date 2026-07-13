---
api_specs:
- filename: nvidia-nim-chat-completions-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Chat Completions API
  slug: nvidia-nim-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-chat-completions-api-openapi.yml
- filename: nvidia-nim-completions-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Completions API
  slug: nvidia-nim-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-completions-api-openapi.yml
- filename: nvidia-nim-embeddings-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Embeddings API
  slug: nvidia-nim-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-embeddings-api-openapi.yml
- filename: nvidia-nim-reranking-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Reranking API
  slug: nvidia-nim-reranking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-reranking-api-openapi.yml
- filename: nvidia-nim-models-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Models API
  slug: nvidia-nim-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-models-api-openapi.yml
- filename: nvidia-nim-vision-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Vision Language Models API
  slug: nvidia-nim-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-vision-api-openapi.yml
- filename: nvidia-nim-health-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Health API
  slug: nvidia-nim-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-health-api-openapi.yml
- filename: nvidia-nim-image-generation-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Image Generation API
  slug: nvidia-nim-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-image-generation-api-openapi.yml
- filename: nvidia-nim-speech-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Speech API
  slug: nvidia-nim-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-speech-api-openapi.yml
- filename: nvidia-nim-biology-api-openapi.yml
  format: yaml
  label: NVIDIA NIM Biology (BioNeMo) API
  slug: nvidia-nim-biology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/openapi/nvidia-nim-biology-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nvidia.com
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: build.nvidia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 16:45:26 2026 GMT
  host: docs.api.nvidia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: integrate.api.nvidia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nvidia Nim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NVIDIA NIM, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NVIDIA NIM
provider_slug: nvidia-nim
slug: nvidia-nim-domain-security
source_filename: nvidia-nim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: build.nvidia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\n- host: docs.api.nvidia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:45:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: integrate.api.nvidia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nvidia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nvidia-nim/refs/heads/main/security/nvidia-nim-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- Inference
- Microservices
- LLM
- Foundation Models
- GPU
- Kubernetes
- NVIDIA
- OpenAI Compatible
---
