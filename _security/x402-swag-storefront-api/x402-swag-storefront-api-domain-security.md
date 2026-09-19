---
api_specs:
- filename: x402-swag-storefront-api-openapi.json
  format: json
  label: x402 Swag storefront API
  slug: x402-swag-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/x402-swag-storefront-api/refs/heads/main/openapi/x402-swag-storefront-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: x402swag.com
  spf: true
hosts:
- cert_expires: Dec  1 00:46:00 2026 GMT
  host: x402swag.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: X402 Swag Storefront Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for x402 Swag storefront API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: x402 Swag storefront API
provider_slug: x402-swag-storefront-api
slug: x402-swag-storefront-api-domain-security
source_filename: x402-swag-storefront-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: x402swag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 00:46:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: x402swag.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/x402-swag-storefront-api/refs/heads/main/security/x402-swag-storefront-api-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- e-commerce
- retail
- merchandise
- agentic commerce
- x402
- crypto payments
- stablecoin
- USDC
- Base
- onchain
- machine-payable API
- print-on-demand
---
