---
api_specs:
- filename: buyapi-ai-openapi-generated.yml
  format: yaml
  label: BuyAPI API
  slug: buyapi-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buyapi-ai/openapi/_ae-authored/buyapi-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: buyapi.ai
  spf: true
hosts:
- cert_expires: Jan  8 12:40:16 2027 GMT
  host: buyapi.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BuyAPI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BuyAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: BuyAPI
provider_slug: buyapi-ai
slug: buyapi-ai-domain-security
source_filename: buyapi-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buyapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 12:40:16 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buyapi.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/buyapi-ai/security/buyapi-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Developer Tools
- MCP
- VendorIntelligence
- Platform
---
