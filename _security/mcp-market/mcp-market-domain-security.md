---
api_specs:
- filename: mcp-market-openapi-generated.yml
  format: yaml
  label: MCP Market API
  slug: mcp-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcp-market/openapi/_ae-authored/mcp-market-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mcp.market
  spf: true
hosts:
- cert_expires: Feb 13 16:58:02 2027 GMT
  host: mcp.market
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MCP Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MCP Market, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MCP Market
provider_slug: mcp-market
slug: mcp-market-domain-security
source_filename: mcp-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcp.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 16:58:02 2027 GMT\n  hsts: false\ndomains:\n- domain: mcp.market\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mcp-market/security/mcp-market-domain-security.yml
summary_line: TLSv1.3
tags:
- Marketplace
- Server Registry
- AI Agents
- Developer Tools
---
