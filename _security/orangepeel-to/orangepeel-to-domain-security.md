---
api_specs:
- filename: orangepeel-to-health-api-openapi.yml
  format: yaml
  label: Orange Peel Health API
  slug: orangepeel-to-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orangepeel-to/openapi/orangepeel-to-health-api-openapi.yml
- filename: orangepeel-to-mcp-api-openapi.yml
  format: yaml
  label: Orange Peel MCP API
  slug: orangepeel-to-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orangepeel-to/openapi/orangepeel-to-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: orangepeel.to
  spf: true
hosts:
- cert_expires: Feb  5 05:38:00 2027 GMT
  host: orangepeel.to
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Orange Peel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orange Peel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Orange Peel
provider_slug: orangepeel-to
slug: orangepeel-to-domain-security
source_filename: orangepeel-to-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orangepeel.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 05:38:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: orangepeel.to\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/orangepeel-to/security/orangepeel-to-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Intelligence
- Fashion
- Hermès
- Scoring
- Markets
---
