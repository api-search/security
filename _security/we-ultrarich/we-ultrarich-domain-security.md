---
api_specs:
- filename: 6a68bfdcf1d9df57e26c3545
  format: yaml
  label: We > Ultrarich MCP Server
  slug: we-ultrarich-mcp-server
  spec_type: Postman
  url: https://www.postman.com/wegtultrarich/we-ultrarich-extreme-wealth-api-mcp/collection/6a68bfdcf1d9df57e26c3545
- filename: we-ultrarich-comparison-api-openapi.yml
  format: yaml
  label: We > Ultrarich Comparison API
  slug: we-ultrarich-comparison-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/we-ultrarich/refs/heads/main/openapi/we-ultrarich-comparison-api-openapi.yml
- filename: we-ultrarich-discovery-api-openapi.yml
  format: yaml
  label: We > Ultrarich Discovery API
  slug: we-ultrarich-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/we-ultrarich/refs/heads/main/openapi/we-ultrarich-discovery-api-openapi.yml
- filename: we-ultrarich-wealth-expression-api-openapi.yml
  format: yaml
  label: We > Ultrarich Wealth Expression API
  slug: we-ultrarich-wealth-expression-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/we-ultrarich/refs/heads/main/openapi/we-ultrarich-wealth-expression-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wegtultrarich.org
  spf: true
hosts:
- cert_expires: Sep 25 19:37:00 2026 GMT
  host: api.wegtultrarich.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: We Ultrarich Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for We > Ultrarich, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: We > Ultrarich
provider_slug: we-ultrarich
slug: we-ultrarich-domain-security
source_filename: we-ultrarich-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.wegtultrarich.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:37:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wegtultrarich.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/we-ultrarich/refs/heads/main/security/we-ultrarich-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- wealth inequality
- economic inequality
- finance
- economics
- education
- journalism
- open data
- comparison
- mcp
- model context protocol
- agents
---
