---
api_specs:
- filename: mixedbread-ai-admin-api-openapi.yml
  format: yaml
  label: Mixedbread admin API
  slug: mixedbread-ai-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-admin-api-openapi.yml
- filename: mixedbread-ai-api-keys-api-openapi.yml
  format: yaml
  label: Mixedbread api_keys API
  slug: mixedbread-ai-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-api-keys-api-openapi.yml
- filename: mixedbread-ai-billing-api-openapi.yml
  format: yaml
  label: Mixedbread billing API
  slug: mixedbread-ai-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-billing-api-openapi.yml
- filename: mixedbread-ai-completions-api-openapi.yml
  format: yaml
  label: Mixedbread completions API
  slug: mixedbread-ai-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-completions-api-openapi.yml
- filename: mixedbread-ai-data-sources-api-openapi.yml
  format: yaml
  label: Mixedbread data_sources API
  slug: mixedbread-ai-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-data-sources-api-openapi.yml
- filename: mixedbread-ai-deprecated-vector-stores-api-openapi.yml
  format: yaml
  label: Mixedbread deprecated_vector_stores API
  slug: mixedbread-ai-deprecated-vector-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-deprecated-vector-stores-api-openapi.yml
- filename: mixedbread-ai-embeddings-api-openapi.yml
  format: yaml
  label: Mixedbread Embeddings API
  slug: mixedbread-ai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-embeddings-api-openapi.yml
- filename: mixedbread-ai-extractions-api-openapi.yml
  format: yaml
  label: Mixedbread extractions API
  slug: mixedbread-ai-extractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-extractions-api-openapi.yml
- filename: mixedbread-ai-files-api-openapi.yml
  format: yaml
  label: Mixedbread files API
  slug: mixedbread-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-files-api-openapi.yml
- filename: mixedbread-ai-mixedbread-embeddings-api-api-openapi.yml
  format: yaml
  label: Mixedbread Mixedbread Embeddings API API
  slug: mixedbread-ai-mixedbread-embeddings-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-mixedbread-embeddings-api-api-openapi.yml
- filename: mixedbread-ai-parsing-api-openapi.yml
  format: yaml
  label: Mixedbread parsing API
  slug: mixedbread-ai-parsing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-parsing-api-openapi.yml
- filename: mixedbread-ai-reranking-api-openapi.yml
  format: yaml
  label: Mixedbread Reranking API
  slug: mixedbread-ai-reranking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-reranking-api-openapi.yml
- filename: mixedbread-ai-schemas-api-openapi.yml
  format: yaml
  label: Mixedbread schemas API
  slug: mixedbread-ai-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-schemas-api-openapi.yml
- filename: mixedbread-ai-stores-api-openapi.yml
  format: yaml
  label: Mixedbread stores API
  slug: mixedbread-ai-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixedbread-ai/refs/heads/main/openapi/mixedbread-ai-stores-api-openapi.yml
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
- Artificial Intelligence
- Embeddings
- Reranking
- Search
- Retrieval
- RAG
- Vector Database
- Multi-Modal
- Parsing
- Open Weights
---
