---
api_specs:
- filename: anyapi-gateway-openapi.json
  format: json
  label: AnyAPI Gateway API
  slug: anyapi-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anyapi/refs/heads/main/openapi/anyapi-gateway-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: getanyapi.com
  spf: true
hosts:
- cert_expires: Nov 26 06:55:56 2026 GMT
  host: getanyapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 04:24:23 2026 GMT
  host: api.getanyapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Anyapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AnyAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: AnyAPI
provider_slug: anyapi
slug: anyapi-domain-security
source_filename: anyapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getanyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 06:55:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getanyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 04:24:23 2026 GMT\n  hsts: null\ndomains:\n- domain: getanyapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anyapi/refs/heads/main/security/anyapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- developer_tools
- data
- search
- scraping
- social_media
- ecommerce
- seo
- enrichment
- mcp
- agent-native
- web-data
- api-marketplace
- agent-payments
- x402
---
