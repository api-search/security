---
api_specs:
- filename: chroma-db-openapi.yml
  format: yaml
  label: Chroma Collections API
  slug: chroma-db-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma-db/refs/heads/main/openapi/chroma-db-openapi.yml
- filename: chroma-db-openapi.yml
  format: yaml
  label: Chroma Records (Embeddings) API
  slug: chroma-db-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma-db/refs/heads/main/openapi/chroma-db-openapi.yml
- filename: chroma-db-openapi.yml
  format: yaml
  label: Chroma Query and Similarity Search API
  slug: chroma-db-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma-db/refs/heads/main/openapi/chroma-db-openapi.yml
- filename: chroma-db-openapi.yml
  format: yaml
  label: Chroma Tenants and Databases API
  slug: chroma-db-tenants-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma-db/refs/heads/main/openapi/chroma-db-openapi.yml
- filename: chroma-db-openapi.yml
  format: yaml
  label: Chroma System and Health API
  slug: chroma-db-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chroma-db/refs/heads/main/openapi/chroma-db-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trychroma.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all
hosts:
- cert_expires: Sep 20 00:20:16 2026 GMT
  host: trychroma.com
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
  hsts: false
  https: true
  note: Root path returns HTTP 404 (API base; v2 endpoints live under /api/v2). Valid TLS cert; HSTS header not observed on this host.
kind: domain-security
layout: security
method: probed
name: Chroma Db Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chroma, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chroma
provider_slug: chroma-db
slug: chroma-db-domain-security
source_filename: chroma-db-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trychroma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:20:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.trychroma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 19:05:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.trychroma.com\n  https: true\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: false\n  note: Root path returns HTTP 404 (API base; v2 endpoints live under /api/v2). Valid TLS cert; HSTS header not observed on this host.\ndomains:\n- domain: trychroma.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com ~all\n  dmarc: true\n  dmarc_policy: reject\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chroma-db/refs/heads/main/security/chroma-db-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Vector Database
- Vector Index
- Vector Search
- Vector Store
- Embeddings
- Similarity Search
- RAG
- Semantic Search
- AI
- AI Inference
- Machine Learning
- Open Source
---
