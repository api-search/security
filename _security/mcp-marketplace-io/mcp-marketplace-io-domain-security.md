---
api_specs:
- filename: mcp-marketplace-io-openapi-generated.yml
  format: yaml
  label: MCP Marketplace API
  slug: mcp-marketplace-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcp-marketplace-io/openapi/_ae-authored/mcp-marketplace-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mcp-marketplace.io
  spf: true
hosts:
- cert_expires: Jan 27 03:22:03 2027 GMT
  host: mcp-marketplace.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MCP Marketplace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MCP Marketplace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MCP Marketplace
provider_slug: mcp-marketplace-io
slug: mcp-marketplace-io-domain-security
source_filename: mcp-marketplace-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcp-marketplace.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 03:22:03 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mcp-marketplace.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mcp-marketplace-io/security/mcp-marketplace-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Marketplace
- Tools
- Security
---
