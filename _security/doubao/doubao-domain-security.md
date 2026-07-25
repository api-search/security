---
api_specs:
- filename: doubao-batch-api-openapi.yml
  format: yaml
  label: ByteDance Doubao Batch API
  slug: doubao-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/openapi/doubao-batch-api-openapi.yml
- filename: doubao-chat-api-openapi.yml
  format: yaml
  label: ByteDance Doubao Chat API
  slug: doubao-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/openapi/doubao-chat-api-openapi.yml
- filename: doubao-embeddings-api-openapi.yml
  format: yaml
  label: ByteDance Doubao Embeddings API
  slug: doubao-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/openapi/doubao-embeddings-api-openapi.yml
- filename: doubao-images-api-openapi.yml
  format: yaml
  label: ByteDance Doubao Images API
  slug: doubao-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/openapi/doubao-images-api-openapi.yml
- filename: doubao-videos-api-openapi.yml
  format: yaml
  label: ByteDance Doubao Videos API
  slug: doubao-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/openapi/doubao-videos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: volcengine.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: volces.com
  spf: false
hosts:
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: www.volcengine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: ark.cn-beijing.volces.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doubao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ByteDance Doubao, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ByteDance Doubao
provider_slug: doubao
slug: doubao-domain-security
source_filename: doubao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.volcengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ark.cn-beijing.volces.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: volcengine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: volces.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doubao/refs/heads/main/security/doubao-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Inference
- ByteDance
- Multimodal
- Volcano Engine
---
