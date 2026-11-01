---
api_specs:
- filename: chunkr-ai-files-api-openapi.yml
  format: yaml
  label: Chunkr Files API
  slug: chunkr-ai-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chunkr-ai/openapi/chunkr-ai-files-api-openapi.yml
- filename: chunkr-ai-health-api-openapi.yml
  format: yaml
  label: Chunkr Health API
  slug: chunkr-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chunkr-ai/openapi/chunkr-ai-health-api-openapi.yml
- filename: chunkr-ai-tasks-api-openapi.yml
  format: yaml
  label: Chunkr Tasks API
  slug: chunkr-ai-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chunkr-ai/openapi/chunkr-ai-tasks-api-openapi.yml
- filename: chunkr-ai-chunkr-api-api-openapi.yml
  format: yaml
  label: Chunkr Chunkr API
  slug: chunkr-ai-chunkr-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chunkr-ai/openapi/chunkr-ai-chunkr-api-api-openapi.yml
- filename: chunkr-ai-extras-api-openapi.yml
  format: yaml
  label: Chunkr Extras API
  slug: chunkr-ai-extras-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chunkr-ai/openapi/chunkr-ai-extras-api-openapi.yml
- filename: chunkr-ai-webhook-api-openapi.yml
  format: yaml
  label: Chunkr Webhook API
  slug: chunkr-ai-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chunkr-ai/openapi/chunkr-ai-webhook-api-openapi.yml
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
hosts_probed: 3
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
source_yaml_url: https://artifacts.apis.io/chunkr-ai/security/chunkr-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Parsing
- OCR
- Chunking
- RAG
- Document Intelligence
---
