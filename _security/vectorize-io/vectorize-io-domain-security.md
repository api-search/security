---
api_specs:
- filename: vectorize-io-ai-platform-connectors-api-openapi.yml
  format: yaml
  label: Vectorize AI Platform Connectors API
  slug: vectorize-io-ai-platform-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-ai-platform-connectors-api-openapi.yml
- filename: vectorize-io-destination-connectors-api-openapi.yml
  format: yaml
  label: Vectorize Destination Connectors API
  slug: vectorize-io-destination-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-destination-connectors-api-openapi.yml
- filename: vectorize-io-extraction-api-openapi.yml
  format: yaml
  label: Vectorize Extraction API
  slug: vectorize-io-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-extraction-api-openapi.yml
- filename: vectorize-io-files-api-openapi.yml
  format: yaml
  label: Vectorize Files API
  slug: vectorize-io-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-files-api-openapi.yml
- filename: vectorize-io-pipelines-api-openapi.yml
  format: yaml
  label: Vectorize Pipelines API
  slug: vectorize-io-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-pipelines-api-openapi.yml
- filename: vectorize-io-source-connectors-api-openapi.yml
  format: yaml
  label: Vectorize Source Connectors API
  slug: vectorize-io-source-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-source-connectors-api-openapi.yml
- filename: vectorize-io-uploads-api-openapi.yml
  format: yaml
  label: Vectorize Uploads API
  slug: vectorize-io-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-uploads-api-openapi.yml
- filename: vectorize-io-workspaces-api-openapi.yml
  format: yaml
  label: Vectorize Workspaces API
  slug: vectorize-io-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectorize-io/refs/heads/main/openapi/vectorize-io-workspaces-api-openapi.yml
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
