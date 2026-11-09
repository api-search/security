---
api_specs:
- filename: alphabridge-mcp-com-openapi-generated.yml
  format: yaml
  label: AlphaBridge MCP API
  slug: alphabridge-mcp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphabridge-mcp-com/openapi/_ae-authored/alphabridge-mcp-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alphabridge-mcp.com
  spf: true
hosts:
- cert_expires: Dec 30 16:43:53 2026 GMT
  host: alphabridge-mcp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alphabridge Mcp Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AlphaBridge MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AlphaBridge MCP
provider_slug: alphabridge-mcp-com
slug: alphabridge-mcp-com-domain-security
source_filename: alphabridge-mcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alphabridge-mcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 16:43:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alphabridge-mcp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/alphabridge-mcp-com/security/alphabridge-mcp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- WordPress
- MCP
- Claude
- ChatGPT
- Pricing
- Documentation
---
