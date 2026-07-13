---
api_specs:
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Pipes API
  slug: langbase-pipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Agent API
  slug: langbase-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Memory API
  slug: langbase-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Threads API
  slug: langbase-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Tools API
  slug: langbase-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Parser API
  slug: langbase-parser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Chunker API
  slug: langbase-chunker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Embed API
  slug: langbase-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
- filename: langbase-openapi.yml
  format: yaml
  label: Langbase Workflows API
  slug: langbase-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/openapi/langbase-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: langbase.com
  spf: true
hosts:
- cert_expires: Sep 28 16:58:25 2026 GMT
  host: langbase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 04:15:19 2026 GMT
  host: api.langbase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Langbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Langbase, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Langbase
provider_slug: langbase
slug: langbase-domain-security
source_filename: langbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: langbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:58:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.langbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 04:15:19 2026 GMT\n  hsts: false\ndomains:\n- domain: langbase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langbase/refs/heads/main/security/langbase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Agents
- RAG
- LLM
- Serverless
---
