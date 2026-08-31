---
api_specs:
- filename: marqo-documents-api-openapi.yml
  format: yaml
  label: Marqo Documents API
  slug: marqo-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/openapi/marqo-documents-api-openapi.yml
- filename: marqo-embeddings-api-openapi.yml
  format: yaml
  label: Marqo Embeddings API
  slug: marqo-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/openapi/marqo-embeddings-api-openapi.yml
- filename: marqo-indexes-api-openapi.yml
  format: yaml
  label: Marqo Indexes API
  slug: marqo-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/openapi/marqo-indexes-api-openapi.yml
- filename: marqo-models-api-openapi.yml
  format: yaml
  label: Marqo Models API
  slug: marqo-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/openapi/marqo-models-api-openapi.yml
- filename: marqo-recommendations-api-openapi.yml
  format: yaml
  label: Marqo Recommendations API
  slug: marqo-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/openapi/marqo-recommendations-api-openapi.yml
- filename: marqo-search-api-openapi.yml
  format: yaml
  label: Marqo Search API
  slug: marqo-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/openapi/marqo-search-api-openapi.yml
- filename: marqo-telemetry-api-openapi.yml
  format: yaml
  label: Marqo Telemetry API
  slug: marqo-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/openapi/marqo-telemetry-api-openapi.yml
description: ''
domains:
- caa:
  - marqo-ana-48a.pages.dev.
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: marqo.ai
  spf: true
hosts:
- cert_expires: Oct  3 00:27:09 2026 GMT
  host: www.marqo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 07:09:38 2026 GMT
  host: docs.marqo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: api.marqo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Marqo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marqo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Marqo
provider_slug: marqo
slug: marqo-domain-security
source_filename: marqo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marqo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:27:09 2026 GMT\n  hsts: false\n- host: docs.marqo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 07:09:38 2026 GMT\n  hsts: false\n- host: api.marqo.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: marqo.ai\n  dnssec: true\n  caa:\n  - marqo-ana-48a.pages.dev.\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marqo/refs/heads/main/security/marqo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Vector Database
- Vector Search
- Multimodal
- Semantic Search
- Embeddings
- Artificial Intelligence
- Machine-Learning
- Open-Source
- Ecommerce Search
---
