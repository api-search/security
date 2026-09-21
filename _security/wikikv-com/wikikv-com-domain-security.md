---
api_specs:
- filename: wikikv-com-openapi.yml
  format: yaml
  label: WikiKV API
  slug: wikikv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikikv-com/refs/heads/main/openapi/wikikv-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wikikv.com
  spf: false
hosts:
- cert_expires: Nov 13 14:01:58 2026 GMT
  host: wikikv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wikikv Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WikiKV, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: WikiKV
provider_slug: wikikv-com
slug: wikikv-com-domain-security
source_filename: wikikv-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wikikv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 14:01:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wikikv.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wikikv-com/refs/heads/main/security/wikikv-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Knowledge-Management
- RAG
- AI Agents
- MCP
- A2A
- Retrieval
- Agent Memory
- Troubleshooting
- Developer Tools
- Open Knowledge
- agent-native
---
