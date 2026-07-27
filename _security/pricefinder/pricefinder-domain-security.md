---
api_specs:
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder Property API
  slug: pricefinder-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder AVM & Valuation API
  slug: pricefinder-avm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder Sales, Rentals & Listings API
  slug: pricefinder-sales-rentals-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder Suburb & Market Statistics API
  slug: pricefinder-suburb-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder Title & Land Reference API
  slug: pricefinder-title-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder Search & Suggest API
  slug: pricefinder-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder Appraisals & CMA API
  slug: pricefinder-appraisals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder Property Event Subscriptions API
  slug: pricefinder-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder SSO API
  slug: pricefinder-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
- filename: pricefinder-api-swagger.json
  format: json
  label: Pricefinder OAuth 2.0 Token API
  slug: pricefinder-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/openapi/pricefinder-api-swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pricefinder.com.au
  spf: true
hosts:
- cert_expires: Aug  3 23:59:59 2026 GMT
  host: www.pricefinder.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  3 23:59:59 2026 GMT
  host: api.pricefinder.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pricefinder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pricefinder, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pricefinder
provider_slug: pricefinder
slug: pricefinder-domain-security
source_filename: pricefinder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pricefinder.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 23:59:59 2026 GMT\n  hsts: null\n- host: api.pricefinder.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: pricefinder.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pricefinder/refs/heads/main/security/pricefinder-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- Australia
- PropTech
- Property Data
- Valuation
- AVM
- Property Listings
- Rentals
- Land Registry
- Title
- Mortgage
- Market Data
---
