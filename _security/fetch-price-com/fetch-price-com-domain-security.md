---
api_specs:
- filename: fetch-price-com-openapi.yml
  format: yaml
  label: fetch-price API
  slug: fetch-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fetch-price-com/refs/heads/main/openapi/fetch-price-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fetch-price.com
  spf: false
hosts:
- cert_expires: Nov 30 22:55:26 2026 GMT
  host: fetch-price.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 22:55:26 2026 GMT
  host: api.fetch-price.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Fetch Price Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for POLICYANDPLAY LTD, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: POLICYANDPLAY LTD
provider_slug: fetch-price-com
slug: fetch-price-com-domain-security
source_filename: fetch-price-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fetch-price.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 22:55:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fetch-price.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 22:55:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fetch-price.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fetch-price-com/refs/heads/main/security/fetch-price-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Price Comparison
- Product Search
- E-Commerce
- Affiliates
- Marketplace
- Shopping
- eBay
- United Kingdom
- AI Agents
- A2A
- MCP
---
