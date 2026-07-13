---
api_specs:
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize Pipelines API
  slug: vectorize-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize Retrieval API
  slug: vectorize-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize Connectors API
  slug: vectorize-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize File Upload API
  slug: vectorize-file-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize Extraction (Iris) API
  slug: vectorize-extraction-iris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
- filename: vectorize-io-openapi.yml
  format: yaml
  label: Vectorize Deep Research API
  slug: vectorize-deep-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vectorize.io
  spf: true
hosts:
- cert_expires: Aug 22 16:38:12 2026 GMT
  host: vectorize.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 02:17:03 2026 GMT
  host: docs.vectorize.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: api.vectorize.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vectorize Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vectorize, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vectorize
provider_slug: vectorize-io
slug: vectorize-io-domain-security
source_filename: vectorize-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vectorize.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 16:38:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.vectorize.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 02:17:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vectorize.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: vectorize.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/security/vectorize-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- RAG
- Vectorization
- Embeddings
- Retrieval
- Vector Database
---
