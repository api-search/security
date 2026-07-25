---
api_specs:
- filename: langdb-analytics-api-openapi.yml
  format: yaml
  label: LangDB Analytics API
  slug: langdb-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-analytics-api-openapi.yml
- filename: langdb-chat-api-openapi.yml
  format: yaml
  label: LangDB Chat API
  slug: langdb-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-chat-api-openapi.yml
- filename: langdb-embeddings-api-openapi.yml
  format: yaml
  label: LangDB Embeddings API
  slug: langdb-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-embeddings-api-openapi.yml
- filename: langdb-images-api-openapi.yml
  format: yaml
  label: LangDB Images API
  slug: langdb-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-images-api-openapi.yml
- filename: langdb-models-api-openapi.yml
  format: yaml
  label: LangDB Models API
  slug: langdb-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-models-api-openapi.yml
- filename: langdb-threads-api-openapi.yml
  format: yaml
  label: LangDB Threads API
  slug: langdb-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/openapi/langdb-threads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: langdb.ai
  spf: true
hosts:
- cert_expires: Sep 20 10:18:38 2026 GMT
  host: langdb.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 07:20:37 2026 GMT
  host: docs.langdb.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.us-east-1.langdb.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Langdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LangDB, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LangDB
provider_slug: langdb
slug: langdb-domain-security
source_filename: langdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: langdb.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 10:18:38 2026 GMT\n  hsts: false\n- host: docs.langdb.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 07:20:37 2026 GMT\n  hsts: false\n- host: api.us-east-1.langdb.ai\n  https: false\ndomains:\n- domain: langdb.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langdb/refs/heads/main/security/langdb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- LLM
- AI Gateway
- Routing
- Governance
- MCP
---
