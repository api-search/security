---
api_specs:
- filename: chunkr-ai-openapi.yml
  format: yaml
  label: Chunkr Parse Task API
  slug: chunkr-parse-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/openapi/chunkr-ai-openapi.yml
- filename: chunkr-ai-openapi.yml
  format: yaml
  label: Chunkr Extract Task API
  slug: chunkr-extract-task-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/openapi/chunkr-ai-openapi.yml
- filename: chunkr-ai-openapi.yml
  format: yaml
  label: Chunkr Task Management API
  slug: chunkr-task-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/openapi/chunkr-ai-openapi.yml
- filename: chunkr-ai-openapi.yml
  format: yaml
  label: Chunkr Files API
  slug: chunkr-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/openapi/chunkr-ai-openapi.yml
- filename: chunkr-ai-openapi.yml
  format: yaml
  label: Chunkr Health and Extras API
  slug: chunkr-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/openapi/chunkr-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chunkr.ai
  spf: true
hosts:
- cert_expires: Sep 22 11:08:57 2026 GMT
  host: chunkr.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 11:08:57 2026 GMT
  host: docs.chunkr.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 11:08:57 2026 GMT
  host: api.chunkr.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chunkr Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chunkr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chunkr
provider_slug: chunkr-ai
slug: chunkr-ai-domain-security
source_filename: chunkr-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chunkr.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:08:57 2026 GMT\n  hsts: false\n- host: docs.chunkr.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:08:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.chunkr.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:08:57 2026 GMT\n  hsts: null\ndomains:\n- domain: chunkr.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chunkr-ai/refs/heads/main/security/chunkr-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Parsing
- OCR
- Chunking
- RAG
- Document Intelligence
---
