---
api_specs:
- filename: chroma-system-api-openapi.yml
  format: yaml
  label: Chroma System API
  slug: chroma-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chroma/openapi/chroma-system-api-openapi.yml
- filename: chroma-authentication-api-openapi.yml
  format: yaml
  label: Chroma Authentication API
  slug: chroma-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chroma/openapi/chroma-authentication-api-openapi.yml
- filename: chroma-collection-api-openapi.yml
  format: yaml
  label: Chroma Collection API
  slug: chroma-collection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chroma/openapi/chroma-collection-api-openapi.yml
- filename: chroma-database-api-openapi.yml
  format: yaml
  label: Chroma Database API
  slug: chroma-database-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chroma/openapi/chroma-database-api-openapi.yml
- filename: chroma-function-api-openapi.yml
  format: yaml
  label: Chroma Function API
  slug: chroma-function-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chroma/openapi/chroma-function-api-openapi.yml
- filename: chroma-record-api-openapi.yml
  format: yaml
  label: Chroma Record API
  slug: chroma-record-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chroma/openapi/chroma-record-api-openapi.yml
- filename: chroma-tenant-api-openapi.yml
  format: yaml
  label: Chroma Tenant API
  slug: chroma-tenant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chroma/openapi/chroma-tenant-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: trychroma.com
  spf: true
hosts:
- cert_expires: Sep 19 04:48:19 2026 GMT
  host: www.trychroma.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 19:05:27 2026 GMT
  host: docs.trychroma.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: api.trychroma.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Chroma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chroma, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Chroma
provider_slug: chroma
slug: chroma-domain-security
source_filename: chroma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trychroma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 04:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.trychroma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 19:05:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.trychroma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: trychroma.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/chroma/security/chroma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- AI-Native
- Apache 2.0
- Cloud
- Embeddings
- Hybrid Search
- JavaScript
- LLM
- Machine Learning
- Multi-Modal
- Open Source
- Python
- RAG
- Retrieval
- SDK
- Search
- Serverless
- TypeScript
- Vector Search
- Database
---
