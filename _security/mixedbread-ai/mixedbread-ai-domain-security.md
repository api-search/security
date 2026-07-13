---
api_specs:
- filename: mixedbread-embeddings-api-openapi.yml
  format: yaml
  label: Mixedbread Embeddings API
  slug: mixedbread-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-embeddings-api-openapi.yml
- filename: mixedbread-reranking-api-openapi.yml
  format: yaml
  label: Mixedbread Reranking API
  slug: mixedbread-reranking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-reranking-api-openapi.yml
- filename: mixedbread-stores-api-openapi.yml
  format: yaml
  label: Mixedbread Stores API
  slug: mixedbread-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-stores-api-openapi.yml
- filename: mixedbread-parsing-api-openapi.yml
  format: yaml
  label: Mixedbread Parsing API
  slug: mixedbread-parsing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-parsing-api-openapi.yml
- filename: mixedbread-extractions-api-openapi.yml
  format: yaml
  label: Mixedbread Extractions API
  slug: mixedbread-extractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-extractions-api-openapi.yml
- filename: mixedbread-files-api-openapi.yml
  format: yaml
  label: Mixedbread Files API
  slug: mixedbread-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-files-api-openapi.yml
- filename: mixedbread-completions-api-openapi.yml
  format: yaml
  label: Mixedbread Chat Completions API
  slug: mixedbread-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-completions-api-openapi.yml
- filename: mixedbread-data-sources-api-openapi.yml
  format: yaml
  label: Mixedbread Data Sources API
  slug: mixedbread-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-data-sources-api-openapi.yml
- filename: mixedbread-api-keys-api-openapi.yml
  format: yaml
  label: Mixedbread API Keys API
  slug: mixedbread-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-api-keys-api-openapi.yml
- filename: mixedbread-billing-api-openapi.yml
  format: yaml
  label: Mixedbread Billing API
  slug: mixedbread-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-billing-api-openapi.yml
- filename: mixedbread-schemas-api-openapi.yml
  format: yaml
  label: Mixedbread Schemas API
  slug: mixedbread-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-schemas-api-openapi.yml
- filename: mixedbread-admin-api-openapi.yml
  format: yaml
  label: Mixedbread Admin API
  slug: mixedbread-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-admin-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mixedbread.com
  spf: true
hosts:
- cert_expires: Sep 27 17:04:03 2026 GMT
  host: www.mixedbread.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: api.mixedbread.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- host: api.dev.mixedbread.com
  https: false
kind: domain-security
layout: security
method: probed
name: Mixedbread Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mixedbread, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mixedbread
provider_slug: mixedbread-ai
slug: mixedbread-ai-domain-security
source_filename: mixedbread-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mixedbread.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:04:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mixedbread.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: null\n- host: api.dev.mixedbread.com\n  https: false\ndomains:\n- domain: mixedbread.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/security/mixedbread-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- Embeddings
- Reranking
- Search
- Retrieval
- RAG
- Vector Database
- Multimodal
- Parsing
- Open Weights
---
