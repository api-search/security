---
api_specs:
- filename: adapter-openapi.json
  format: json
  label: Adapter Cognition API
  slug: adapter
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapter/refs/heads/main/openapi/adapter-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: adapter.com
  spf: true
hosts:
- cert_expires: Oct 11 15:11:22 2026 GMT
  host: www.adapter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 05:15:09 2026 GMT
  host: api.adapter.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adapter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adapter, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Adapter
provider_slug: adapter
slug: adapter-domain-security
source_filename: adapter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adapter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 15:11:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.adapter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 05:15:09 2026 GMT\n  hsts: null\ndomains:\n- domain: adapter.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adapter/refs/heads/main/security/adapter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Cognition
- Knowledge Graph
- Memory
- Agents
- MCP
- LLM
---
