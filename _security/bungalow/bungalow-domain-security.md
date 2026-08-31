---
api_specs:
- filename: bungalow-applications-api-openapi.yml
  format: yaml
  label: Bungalow Applications API
  slug: bungalow-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bungalow/refs/heads/main/openapi/bungalow-applications-api-openapi.yml
- filename: bungalow-listings-api-openapi.yml
  format: yaml
  label: Bungalow Listings API
  slug: bungalow-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bungalow/refs/heads/main/openapi/bungalow-listings-api-openapi.yml
- filename: bungalow-markets-api-openapi.yml
  format: yaml
  label: Bungalow Markets API
  slug: bungalow-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bungalow/refs/heads/main/openapi/bungalow-markets-api-openapi.yml
- filename: bungalow-showings-api-openapi.yml
  format: yaml
  label: Bungalow Showings API
  slug: bungalow-showings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bungalow/refs/heads/main/openapi/bungalow-showings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bungalow.com
  spf: true
hosts:
- cert_expires: Sep 26 05:05:35 2026 GMT
  host: bungalow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: fieldstone.bungalow.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bungalow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bungalow, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bungalow
provider_slug: bungalow
slug: bungalow-domain-security
source_filename: bungalow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bungalow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:05:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fieldstone.bungalow.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bungalow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bungalow/refs/heads/main/security/bungalow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real-Estate
- Residential Real Estate
- Rental Listings
- Property Management
- Co-Living
- Single-Family Rental
- Listings Syndication
- Housing
- PropTech
- Marketplace
---
