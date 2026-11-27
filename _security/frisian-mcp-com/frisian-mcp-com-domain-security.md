---
api_specs:
- filename: frisian-mcp-com-openapi-generated.yml
  format: yaml
  label: Frisian MCP API
  slug: frisian-mcp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frisian-mcp-com/openapi/_ae-authored/frisian-mcp-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: frisian-mcp.com
  spf: false
hosts:
- cert_expires: May 18 23:59:59 2027 GMT
  host: frisian-mcp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Frisian MCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frisian MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Frisian MCP
provider_slug: frisian-mcp-com
slug: frisian-mcp-com-domain-security
source_filename: frisian-mcp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frisian-mcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: frisian-mcp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/frisian-mcp-com/security/frisian-mcp-com-domain-security.yml
summary_line: TLSv1.3
tags:
- MCP
- Context-Aware
- Token Bloat
- SDK
---
