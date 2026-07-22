---
api_specs:
- filename: seltz-openapi-original.json
  format: json
  label: Seltz Web Knowledge API
  slug: seltz-web-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seltz/refs/heads/main/openapi/seltz-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: seltz.ai
  spf: true
hosts:
- cert_expires: Oct  4 20:24:18 2026 GMT
  host: docs.seltz.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:15:45 2026 GMT
  host: api.seltz.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seltz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seltz, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Seltz
provider_slug: seltz
slug: seltz-domain-security
source_filename: seltz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.seltz.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 20:24:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.seltz.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:15:45 2026 GMT\n  hsts: false\ndomains:\n- domain: seltz.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seltz/refs/heads/main/security/seltz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Web Search
- AI Infrastructure
- Retrieval
- RAG
- Agents
- LLM
- Knowledge API
- Developer Tools
- MCP
---
