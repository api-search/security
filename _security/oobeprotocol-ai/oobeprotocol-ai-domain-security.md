---
api_specs:
- filename: oobeprotocol-ai-mcp-api-openapi.yml
  format: yaml
  label: OOBE Protocol MCP API
  slug: oobeprotocol-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oobeprotocol-ai/openapi/oobeprotocol-ai-mcp-api-openapi.yml
- filename: oobeprotocol-ai-premium-api-openapi.yml
  format: yaml
  label: OOBE Protocol Premium API
  slug: oobeprotocol-ai-premium-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oobeprotocol-ai/openapi/oobeprotocol-ai-premium-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oobeprotocol.ai
  spf: true
hosts:
- cert_expires: Jan 26 00:47:08 2027 GMT
  host: oobeprotocol.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OOBE Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OOBE Protocol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OOBE Protocol
provider_slug: oobeprotocol-ai
slug: oobeprotocol-ai-domain-security
source_filename: oobeprotocol-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oobeprotocol.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 00:47:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oobeprotocol.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/oobeprotocol-ai/security/oobeprotocol-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Infrastructure
- Autonomous Systems
- Protocol
- Developer Tools
- Blockchain
- Solana
- Agent Identity
- Payment Rails
---
