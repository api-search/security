---
api_specs:
- filename: eveoy-com-mcp-api-openapi.yml
  format: yaml
  label: Eveoy MCP API
  slug: eveoy-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eveoy-com/openapi/eveoy-com-mcp-api-openapi.yml
- filename: eveoy-com-order-api-openapi.yml
  format: yaml
  label: Eveoy Order API
  slug: eveoy-com-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eveoy-com/openapi/eveoy-com-order-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eveoy.com
  spf: true
hosts:
- cert_expires: Dec 12 21:45:22 2026 GMT
  host: eveoy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eveoy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eveoy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eveoy
provider_slug: eveoy-com
slug: eveoy-com-domain-security
source_filename: eveoy-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eveoy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 21:45:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eveoy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/eveoy-com/security/eveoy-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CustomerPhotos
- InStoreSampling
- BuyAndTry
- Marketing
- Retail
---
