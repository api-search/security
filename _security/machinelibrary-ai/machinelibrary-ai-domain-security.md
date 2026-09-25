---
api_specs:
- filename: machinelibrary-ai-openapi.yml
  format: yaml
  label: Machine Library API
  slug: machine-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/openapi/machinelibrary-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: machinelibrary.ai
  spf: true
hosts:
- cert_expires: Dec 11 05:29:39 2026 GMT
  host: machinelibrary.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 05:29:39 2026 GMT
  host: api.machinelibrary.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 05:29:39 2026 GMT
  host: mcp.machinelibrary.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Machinelibrary Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Space Frontiers, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Space Frontiers
provider_slug: machinelibrary-ai
slug: machinelibrary-ai-domain-security
source_filename: machinelibrary-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: machinelibrary.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 05:29:39 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.machinelibrary.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 05:29:39 2026 GMT\n  hsts: null\n- host: mcp.machinelibrary.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 05:29:39 2026 GMT\n  hsts: null\ndomains:\n- domain: machinelibrary.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/machinelibrary-ai/refs/heads/main/security/machinelibrary-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Research
- Scholarly Search
- Full-Text Search
- Retrieval
- RAG
- Patents
- Documents
- OCR
- Document Recognition
- MCP
- A2A
- Agent-Native
- AI Agents
- Data
- Search
---
