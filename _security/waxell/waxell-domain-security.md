---
api_specs:
- filename: waxell-observe-openapi.yml
  format: yaml
  label: Waxell Observe API
  slug: observe
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waxell/refs/heads/main/openapi/waxell-observe-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: waxell.ai
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: waxell.dev
  spf: false
hosts:
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: waxell.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: dev-mcp.waxell.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Waxell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Waxell, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Waxell
provider_slug: waxell
slug: waxell-domain-security
source_filename: waxell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: waxell.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev-mcp.waxell.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: waxell.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: waxell.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waxell/refs/heads/main/security/waxell-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI Agent Governance
- Observability
- Policy Enforcement
- LLM Telemetry
- Cost Management
- MCP
- Agent Runtime
---
