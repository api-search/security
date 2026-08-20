---
api_specs:
- filename: siliconflow-audio-api-openapi.yml
  format: yaml
  label: SiliconFlow Audio API
  slug: siliconflow-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siliconflow/refs/heads/main/openapi/siliconflow-audio-api-openapi.yml
- filename: siliconflow-chat-api-openapi.yml
  format: yaml
  label: SiliconFlow Chat API
  slug: siliconflow-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siliconflow/refs/heads/main/openapi/siliconflow-chat-api-openapi.yml
- filename: siliconflow-completions-api-openapi.yml
  format: yaml
  label: SiliconFlow Completions API
  slug: siliconflow-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siliconflow/refs/heads/main/openapi/siliconflow-completions-api-openapi.yml
- filename: siliconflow-embeddings-api-openapi.yml
  format: yaml
  label: SiliconFlow Embeddings API
  slug: siliconflow-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siliconflow/refs/heads/main/openapi/siliconflow-embeddings-api-openapi.yml
- filename: siliconflow-images-api-openapi.yml
  format: yaml
  label: SiliconFlow Images API
  slug: siliconflow-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siliconflow/refs/heads/main/openapi/siliconflow-images-api-openapi.yml
- filename: siliconflow-messages-api-openapi.yml
  format: yaml
  label: SiliconFlow Messages API
  slug: siliconflow-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siliconflow/refs/heads/main/openapi/siliconflow-messages-api-openapi.yml
- filename: siliconflow-models-api-openapi.yml
  format: yaml
  label: SiliconFlow Models API
  slug: siliconflow-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siliconflow/refs/heads/main/openapi/siliconflow-models-api-openapi.yml
- filename: siliconflow-rerank-api-openapi.yml
  format: yaml
  label: SiliconFlow Rerank API
  slug: siliconflow-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siliconflow/refs/heads/main/openapi/siliconflow-rerank-api-openapi.yml
- filename: siliconflow-user-api-openapi.yml
  format: yaml
  label: SiliconFlow User API
  slug: siliconflow-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siliconflow/refs/heads/main/openapi/siliconflow-user-api-openapi.yml
- filename: siliconflow-videos-api-openapi.yml
  format: yaml
  label: SiliconFlow Videos API
  slug: siliconflow-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/siliconflow/refs/heads/main/openapi/siliconflow-videos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: siliconflow.com
  spf: true
hosts:
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: siliconflow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 19:44:10 2026 GMT
  host: docs.siliconflow.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 10:12:23 2026 GMT
  host: api.siliconflow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Siliconflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SiliconFlow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: SiliconFlow
provider_slug: siliconflow
slug: siliconflow-domain-security
source_filename: siliconflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: siliconflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.siliconflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:44:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.siliconflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 10:12:23 2026 GMT\n  hsts: null\ndomains:\n- domain: siliconflow.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siliconflow/refs/heads/main/security/siliconflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- LLM
- Inference
- Open-Source
- OpenAI-Compatible
- Anthropic Compatible
- Image-Generation
- Audio
- Video
---
