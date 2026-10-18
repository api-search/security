---
api_specs:
- filename: hasmcp-providers-api-openapi.yml
  format: yaml
  label: HasMCP Providers API
  slug: hasmcp-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasmcp/refs/heads/main/openapi/hasmcp-providers-api-openapi.yml
- filename: hasmcp-servers-api-openapi.yml
  format: yaml
  label: HasMCP Servers API
  slug: hasmcp-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasmcp/refs/heads/main/openapi/hasmcp-servers-api-openapi.yml
- filename: hasmcp-variables-api-openapi.yml
  format: yaml
  label: HasMCP Variables API
  slug: hasmcp-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hasmcp/refs/heads/main/openapi/hasmcp-variables-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hasmcp.com
  spf: true
hosts:
- cert_expires: Nov 22 09:48:14 2026 GMT
  host: hasmcp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hasmcp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HasMCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HasMCP
provider_slug: hasmcp
slug: hasmcp-domain-security
source_filename: hasmcp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hasmcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 09:48:14 2026 GMT\n  hsts: false\ndomains:\n- domain: hasmcp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hasmcp/refs/heads/main/security/hasmcp-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- No-code
- Low-code
- MCP
- API Gateway
---
