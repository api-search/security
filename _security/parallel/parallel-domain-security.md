---
api_specs:
- filename: parallel-chat-api-beta-api-openapi.yml
  format: yaml
  label: Parallel Chat API (Beta) API
  slug: parallel-chat-api-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-chat-api-beta-api-openapi.yml
- filename: parallel-extract-api-openapi.yml
  format: yaml
  label: Parallel Extract API
  slug: parallel-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-extract-api-openapi.yml
- filename: parallel-findall-api-openapi.yml
  format: yaml
  label: Parallel FindAll API
  slug: parallel-findall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-findall-api-openapi.yml
- filename: parallel-monitor-api-openapi.yml
  format: yaml
  label: Parallel Monitor API
  slug: parallel-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-monitor-api-openapi.yml
- filename: parallel-search-api-openapi.yml
  format: yaml
  label: Parallel Search API
  slug: parallel-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-search-api-openapi.yml
- filename: parallel-tasks-api-openapi.yml
  format: yaml
  label: Parallel Tasks API
  slug: parallel-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-tasks-api-openapi.yml
- filename: parallel-memory-api-openapi.yml
  format: yaml
  label: Parallel Memory API
  slug: parallel-memory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-memory-api-openapi.yml
- filename: parallel-responses-api-api-openapi.yml
  format: yaml
  label: Parallel Responses API
  slug: parallel-responses-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/openapi/parallel-responses-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: parallel.ai
  spf: true
hosts:
- cert_expires: Oct 25 05:43:57 2026 GMT
  host: www.parallel.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 14:11:19 2026 GMT
  host: docs.parallel.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 19:46:36 2026 GMT
  host: api.parallel.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parallel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parallel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Parallel
provider_slug: parallel
slug: parallel-domain-security
source_filename: parallel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.parallel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 05:43:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.parallel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 14:11:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.parallel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 19:46:36 2026 GMT\n  hsts: null\ndomains:\n- domain: parallel.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallel/refs/heads/main/security/parallel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Web Search
- Agents
- Deep Research
- Web Extraction
- Data Enrichment
- Web Monitoring
- LLM Tools
---
