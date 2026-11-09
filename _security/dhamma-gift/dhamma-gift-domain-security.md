---
api_specs:
- filename: dhamma-gift-mcp-api-openapi.yml
  format: yaml
  label: Dhamma.Gift MCP API
  slug: dhamma-gift-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dhamma-gift/openapi/dhamma-gift-mcp-api-openapi.yml
- filename: dhamma-gift-search-api-openapi.yml
  format: yaml
  label: Dhamma.Gift Search API
  slug: dhamma-gift-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dhamma-gift/openapi/dhamma-gift-search-api-openapi.yml
- filename: dhamma-gift-text-api-openapi.yml
  format: yaml
  label: Dhamma.Gift Text API
  slug: dhamma-gift-text-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dhamma-gift/openapi/dhamma-gift-text-api-openapi.yml
- filename: dhamma-gift-toc-api-openapi.yml
  format: yaml
  label: Dhamma.Gift Toc API
  slug: dhamma-gift-toc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dhamma-gift/openapi/dhamma-gift-toc-api-openapi.yml
- filename: dhamma-gift-tts-api-openapi.yml
  format: yaml
  label: Dhamma.Gift Tts API
  slug: dhamma-gift-tts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dhamma-gift/openapi/dhamma-gift-tts-api-openapi.yml
- filename: dhamma-gift-uposatha-api-openapi.yml
  format: yaml
  label: Dhamma.Gift Uposatha API
  slug: dhamma-gift-uposatha-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dhamma-gift/openapi/dhamma-gift-uposatha-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dhamma.gift
  spf: true
hosts:
- cert_expires: Jan  6 12:19:41 2027 GMT
  host: dhamma.gift
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dhamma Gift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dhamma.Gift, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dhamma.Gift
provider_slug: dhamma-gift
slug: dhamma-gift-domain-security
source_filename: dhamma-gift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dhamma.gift\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 12:19:41 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dhamma.gift\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dhamma-gift/security/dhamma-gift-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Buddhism
- Pali Canon
- Texts
- Search
- Audio
---
