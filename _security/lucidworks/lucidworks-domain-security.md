---
api_specs:
- filename: lucidworks-ai-platform-openapi.yml
  format: yaml
  label: Lucidworks AI Platform API
  slug: ai-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-ai-platform-openapi.yml
- filename: lucidworks-embeddings-openapi.yml
  format: yaml
  label: Lucidworks Embeddings and Classification API
  slug: embeddings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-embeddings-openapi.yml
- filename: lucidworks-signals-openapi.yml
  format: yaml
  label: Lucidworks Signals API
  slug: signals
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-signals-openapi.yml
- filename: lucidworks-rules-openapi.yml
  format: yaml
  label: Lucidworks Rules and Query Rewrites API
  slug: rules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-rules-openapi.yml
- filename: lucidworks-chunking-openapi.yml
  format: yaml
  label: Lucidworks Content Chunking API
  slug: chunking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-chunking-openapi.yml
- filename: lucidworks-models-openapi.yml
  format: yaml
  label: Lucidworks Model Management API
  slug: models
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/openapi/lucidworks-models-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lucidworks.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: lucidworks.ai
  spf: false
hosts:
- cert_expires: Sep  3 17:23:24 2026 GMT
  host: lucidworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 03:14:21 2026 GMT
  host: doc.lucidworks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.lucidworks.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Lucidworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lucidworks, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lucidworks
provider_slug: lucidworks
slug: lucidworks-domain-security
source_filename: lucidworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lucidworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 17:23:24 2026 GMT\n  hsts: null\n- host: doc.lucidworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 03:14:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.lucidworks.ai\n  https: false\ndomains:\n- domain: lucidworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: lucidworks.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucidworks/refs/heads/main/security/lucidworks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Artificial Intelligence
- Enterprise Search
- Vector Search
- RAG
- Commerce
---
