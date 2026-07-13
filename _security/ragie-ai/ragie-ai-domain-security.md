---
api_specs:
- filename: ragie-ai-openapi.yml
  format: yaml
  label: Ragie Documents API
  slug: ragie-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ragie-ai/refs/heads/main/openapi/ragie-ai-openapi.yml
- filename: ragie-ai-openapi.yml
  format: yaml
  label: Ragie Retrievals API
  slug: ragie-retrievals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ragie-ai/refs/heads/main/openapi/ragie-ai-openapi.yml
- filename: ragie-ai-openapi.yml
  format: yaml
  label: Ragie Connections API
  slug: ragie-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ragie-ai/refs/heads/main/openapi/ragie-ai-openapi.yml
- filename: ragie-ai-openapi.yml
  format: yaml
  label: Ragie Entities and Extraction API
  slug: ragie-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ragie-ai/refs/heads/main/openapi/ragie-ai-openapi.yml
- filename: ragie-ai-openapi.yml
  format: yaml
  label: Ragie Partitions API
  slug: ragie-partitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ragie-ai/refs/heads/main/openapi/ragie-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ragie.ai
  spf: true
hosts:
- cert_expires: Sep 15 03:30:57 2026 GMT
  host: www.ragie.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 22:04:32 2026 GMT
  host: docs.ragie.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 03:24:40 2026 GMT
  host: api.ragie.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ragie Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ragie, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ragie
provider_slug: ragie-ai
slug: ragie-ai-domain-security
source_filename: ragie-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ragie.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 03:30:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ragie.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 22:04:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ragie.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 03:24:40 2026 GMT\n  hsts: null\ndomains:\n- domain: ragie.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ragie-ai/refs/heads/main/security/ragie-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- RAG
- Retrieval
- Vector Search
- Document Ingestion
---
