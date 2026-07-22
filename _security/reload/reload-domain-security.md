---
api_specs:
- filename: reload-openapi-original.json
  format: json
  label: Reload API
  slug: reload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reload/refs/heads/main/openapi/reload-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: reload.team
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reload.chat
  spf: true
hosts:
- cert_expires: Sep 14 19:05:34 2026 GMT
  host: reload.team
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 05:11:29 2026 GMT
  host: docs.reload.chat
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 05:53:24 2026 GMT
  host: api.reload.chat
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reload Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reload, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Reload
provider_slug: reload
slug: reload-domain-security
source_filename: reload-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reload.team\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:05:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.reload.chat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 05:11:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.reload.chat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:53:24 2026 GMT\n  hsts: null\ndomains:\n- domain: reload.team\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: reload.chat\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reload/refs/heads/main/security/reload-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Agent Orchestration
- Team Chat
- Collaboration
- Memory
- Context Graph
- Model Context Protocol
- MCP
- Developer Tools
- Tasks
- Productivity
---
