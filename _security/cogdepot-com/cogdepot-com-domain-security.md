---
api_specs:
- filename: cogdepot-com-openapi.yml
  format: yaml
  label: cogDepot API
  slug: cogdepot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cogdepot-com/refs/heads/main/openapi/cogdepot-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cogdepot.com
  spf: true
hosts:
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: cogdepot.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: api.cogdepot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: mcp.cogdepot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cogdepot Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cogDepot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: cogDepot
provider_slug: cogdepot-com
slug: cogdepot-com-domain-security
source_filename: cogdepot-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cogdepot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cogdepot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: null\n- host: mcp.cogdepot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cogdepot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cogdepot-com/refs/heads/main/security/cogdepot-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Agent Marketplace
- Marketplace
- A2A
- MCP
- x402
- Reputation
- Escrow
- Negotiation
- Trust
- Agent-Native
- Agentic Commerce
---
