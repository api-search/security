---
api_specs:
- filename: rettfrabonden-com-a2a-api-openapi.yml
  format: yaml
  label: Rett fra Bonden A2a API
  slug: rettfrabonden-com-a2a-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rettfrabonden-com/refs/heads/main/openapi/rettfrabonden-com-a2a-api-openapi.yml
- filename: rettfrabonden-com-marketplace-api-openapi.yml
  format: yaml
  label: Rett fra Bonden Marketplace API
  slug: rettfrabonden-com-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rettfrabonden-com/refs/heads/main/openapi/rettfrabonden-com-marketplace-api-openapi.yml
- filename: rettfrabonden-com-mcp-api-openapi.yml
  format: yaml
  label: Rett fra Bonden MCP API
  slug: rettfrabonden-com-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rettfrabonden-com/refs/heads/main/openapi/rettfrabonden-com-mcp-api-openapi.yml
- filename: rettfrabonden-com-stats-api-openapi.yml
  format: yaml
  label: Rett fra Bonden Stats API
  slug: rettfrabonden-com-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rettfrabonden-com/refs/heads/main/openapi/rettfrabonden-com-stats-api-openapi.yml
- filename: rettfrabonden-com-well-known-api-openapi.yml
  format: yaml
  label: Rett fra Bonden .well Known API
  slug: rettfrabonden-com-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rettfrabonden-com/refs/heads/main/openapi/rettfrabonden-com-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rettfrabonden.com
  spf: false
hosts:
- cert_expires: Nov  9 23:55:15 2026 GMT
  host: rettfrabonden.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rettfrabonden Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rett fra Bonden, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Rett fra Bonden
provider_slug: rettfrabonden-com
slug: rettfrabonden-com-domain-security
source_filename: rettfrabonden-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rettfrabonden.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:55:15 2026 GMT\n  hsts: null\ndomains:\n- domain: rettfrabonden.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rettfrabonden-com/refs/heads/main/security/rettfrabonden-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Local Food
- Agriculture
- Food
- Marketplace
- Directory
- Search
- Geolocation
- A2A
- MCP
- Norway
- Open Source
- Company
---
